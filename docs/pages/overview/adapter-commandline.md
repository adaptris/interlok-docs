# Running Interlok Using the Bundled Scripts

Starting Interlok will largely depend on your installation method.  If you have used our Java based installer, then you will have a "./bin" directory at the root of your installation which contains both a windows batch file and linux shell script.  Executing one of those will start your instance assuming your systems Java systems properties (JAVA_HOME) are set correctly.

If however you have chosen to install Interlok manually or using the gradle method, then you may need to create your own start scripts.  See below for your copy/paste convenience;

### Windows start-interlok.bat;
```
@rem
@rem Copyright 2015 the original author or authors.
@rem
@rem Licensed under the Apache License, Version 2.0 (the "License");
@rem you may not use this file except in compliance with the License.
@rem You may obtain a copy of the License at
@rem
@rem      https://www.apache.org/licenses/LICENSE-2.0
@rem
@rem Unless required by applicable law or agreed to in writing, software
@rem distributed under the License is distributed on an "AS IS" BASIS,
@rem WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
@rem See the License for the specific language governing permissions and
@rem limitations under the License.
@rem

@if "%DEBUG%" == "" @echo off
@rem ##########################################################################
@rem
@rem  Interlok startup script for Windows
@rem
@rem ##########################################################################

@rem Set local scope for the variables with windows NT shell
if "%OS%"=="Windows_NT" setlocal

set DIRNAME=%~dp0
if "%DIRNAME%" == "" set DIRNAME=.
set APP_BASE_NAME=%~n0
set APP_HOME=%DIRNAME%..

@rem Resolve any "." and ".." in APP_HOME to make it shorter.
for %%i in ("%APP_HOME%") do set APP_HOME=%%~fi

@rem Add default JVM options here. You can also use JAVA_OPTS and INTERLOK_OPTS to pass JVM options to this script.
set DEFAULT_JVM_OPTS=

@rem Find java.exe
if defined JAVA_HOME goto findJavaFromJavaHome

set JAVA_EXE=java.exe
%JAVA_EXE% -version >NUL 2>&1
if "%ERRORLEVEL%" == "0" goto execute

echo.
echo ERROR: JAVA_HOME is not set and no 'java' command could be found in your PATH.
echo.
echo Please set the JAVA_HOME variable in your environment to match the
echo location of your Java installation.

goto fail

:findJavaFromJavaHome
set JAVA_HOME=%JAVA_HOME:"=%
set JAVA_EXE=%JAVA_HOME%/bin/java.exe

if exist "%JAVA_EXE%" goto execute

echo.
echo ERROR: JAVA_HOME is set to an invalid directory: %JAVA_HOME%
echo.
echo Please set the JAVA_HOME variable in your environment to match the
echo location of your Java installation.

goto fail

:execute
@rem Setup the command line

set CLASSPATH=%APP_HOME%\lib\interlok-boot.jar

@rem Go to app home dir
cd %APP_HOME%
@rem Execute Interlok
"%JAVA_EXE%" %DEFAULT_JVM_OPTS% %JAVA_OPTS% %INTERLOK_OPTS%  -classpath "%CLASSPATH%" com.adaptris.interlok.boot.InterlokLauncher %*

:end
@rem End local scope for the variables with windows NT shell
if "%ERRORLEVEL%"=="0" goto mainEnd

:fail
rem Set variable INTERLOK_EXIT_CONSOLE if you need the _script_ return code instead of
rem the _cmd.exe /c_ return code!
if  not "" == "%INTERLOK_EXIT_CONSOLE%" exit 1
exit /b 1

:mainEnd
if "%OS%"=="Windows_NT" endlocal

:omega

```

### Linux start-interlok.sh;
```
#!/usr/bin/env sh

#
# Copyright 2015 the original author or authors.
#
# Licensed under the Apache License, Version 2.0 (the "License");
# you may not use this file except in compliance with the License.
# You may obtain a copy of the License at
#
#      https://www.apache.org/licenses/LICENSE-2.0
#
# Unless required by applicable law or agreed to in writing, software
# distributed under the License is distributed on an "AS IS" BASIS,
# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
# See the License for the specific language governing permissions and
# limitations under the License.
#

##############################################################################
##
##  Interlok start up script for UN*X
##
##############################################################################

# Attempt to set APP_HOME
# Resolve links: $0 may be a link
PRG="$0"
# Need this for relative symlinks.
while [ -h "$PRG" ] ; do
    ls=`ls -ld "$PRG"`
    link=`expr "$ls" : '.*-> \(.*\)$'`
    if expr "$link" : '/.*' > /dev/null; then
        PRG="$link"
    else
        PRG=`dirname "$PRG"`"/$link"
    fi
done
SAVED="`pwd`"
cd "`dirname \"$PRG\"`/.." >/dev/null
APP_HOME="`pwd -P`"
cd "$SAVED" >/dev/null

APP_NAME="Interlok"
APP_BASE_NAME=`basename "$0"`

# Add default JVM options here. You can also use JAVA_OPTS and INTERLOK_OPTS to pass JVM options to this script.
DEFAULT_JVM_OPTS=""

# Use the maximum available, or set MAX_FD != -1 to use that value.
MAX_FD="maximum"

warn () {
    echo "$*"
}

die () {
    echo
    echo "$*"
    echo
    exit 1
}

# OS specific support (must be 'true' or 'false').
cygwin=false
msys=false
darwin=false
nonstop=false
case "`uname`" in
  CYGWIN* )
    cygwin=true
    ;;
  Darwin* )
    darwin=true
    ;;
  MINGW* )
    msys=true
    ;;
  NONSTOP* )
    nonstop=true
    ;;
esac

CLASSPATH=$APP_HOME/lib/interlok-boot.jar


# Determine the Java command to use to start the JVM.
if [ -n "$JAVA_HOME" ] ; then
    if [ -x "$JAVA_HOME/jre/sh/java" ] ; then
        # IBM's JDK on AIX uses strange locations for the executables
        JAVACMD="$JAVA_HOME/jre/sh/java"
    else
        JAVACMD="$JAVA_HOME/bin/java"
    fi
    if [ ! -x "$JAVACMD" ] ; then
        die "ERROR: JAVA_HOME is set to an invalid directory: $JAVA_HOME

Please set the JAVA_HOME variable in your environment to match the
location of your Java installation."
    fi
else
    JAVACMD="java"
    which java >/dev/null 2>&1 || die "ERROR: JAVA_HOME is not set and no 'java' command could be found in your PATH.

Please set the JAVA_HOME variable in your environment to match the
location of your Java installation."
fi

# Increase the maximum file descriptors if we can.
if [ "$cygwin" = "false" -a "$darwin" = "false" -a "$nonstop" = "false" ] ; then
    MAX_FD_LIMIT=`ulimit -H -n`
    if [ $? -eq 0 ] ; then
        if [ "$MAX_FD" = "maximum" -o "$MAX_FD" = "max" ] ; then
            MAX_FD="$MAX_FD_LIMIT"
        fi
        ulimit -n $MAX_FD
        if [ $? -ne 0 ] ; then
            warn "Could not set maximum file descriptor limit: $MAX_FD"
        fi
    else
        warn "Could not query maximum file descriptor limit: $MAX_FD_LIMIT"
    fi
fi

# For Darwin, add options to specify how the application appears in the dock
if $darwin; then
    GRADLE_OPTS="$GRADLE_OPTS \"-Xdock:name=$APP_NAME\" \"-Xdock:icon=$APP_HOME/media/gradle.icns\""
fi

# For Cygwin or MSYS, switch paths to Windows format before running java
if [ "$cygwin" = "true" -o "$msys" = "true" ] ; then
    APP_HOME=`cygpath --path --mixed "$APP_HOME"`
    CLASSPATH=`cygpath --path --mixed "$CLASSPATH"`

    JAVACMD=`cygpath --unix "$JAVACMD"`

    # We build the pattern for arguments to be converted via cygpath
    ROOTDIRSRAW=`find -L / -maxdepth 1 -mindepth 1 -type d 2>/dev/null`
    SEP=""
    for dir in $ROOTDIRSRAW ; do
        ROOTDIRS="$ROOTDIRS$SEP$dir"
        SEP="|"
    done
    OURCYGPATTERN="(^($ROOTDIRS))"
    # Add a user-defined pattern to the cygpath arguments
    if [ "$GRADLE_CYGPATTERN" != "" ] ; then
        OURCYGPATTERN="$OURCYGPATTERN|($GRADLE_CYGPATTERN)"
    fi
    # Now convert the arguments - kludge to limit ourselves to /bin/sh
    i=0
    for arg in "$@" ; do
        CHECK=`echo "$arg"|egrep -c "$OURCYGPATTERN" -`
        CHECK2=`echo "$arg"|egrep -c "^-"`                                 ### Determine if an option

        if [ $CHECK -ne 0 ] && [ $CHECK2 -eq 0 ] ; then                    ### Added a condition
            eval `echo args$i`=`cygpath --path --ignore --mixed "$arg"`
        else
            eval `echo args$i`="\"$arg\""
        fi
        i=`expr $i + 1`
    done
    case $i in
        0) set -- ;;
        1) set -- "$args0" ;;
        2) set -- "$args0" "$args1" ;;
        3) set -- "$args0" "$args1" "$args2" ;;
        4) set -- "$args0" "$args1" "$args2" "$args3" ;;
        5) set -- "$args0" "$args1" "$args2" "$args3" "$args4" ;;
        6) set -- "$args0" "$args1" "$args2" "$args3" "$args4" "$args5" ;;
        7) set -- "$args0" "$args1" "$args2" "$args3" "$args4" "$args5" "$args6" ;;
        8) set -- "$args0" "$args1" "$args2" "$args3" "$args4" "$args5" "$args6" "$args7" ;;
        9) set -- "$args0" "$args1" "$args2" "$args3" "$args4" "$args5" "$args6" "$args7" "$args8" ;;
    esac
fi

# Escape application args
save () {
    for i do printf %s\\n "$i" | sed "s/'/'\\\\''/g;1s/^/'/;\$s/\$/' \\\\/" ; done
    echo " "
}
APP_ARGS=`save "$@"`

# Collect all arguments for the java command, following the shell quoting and substitution rules
eval set -- $DEFAULT_JVM_OPTS $JAVA_OPTS $INTERLOK_OPTS -classpath "\"$CLASSPATH\"" com.adaptris.interlok.boot.InterlokLauncher "$APP_ARGS"

# Go to app home dir
cd "$APP_HOME"
exec "$JAVACMD" "$@"

```

## Running directly from the commandline ##

Provided the current working directory is the base directory of the installation, the adapter can simply be started using the standard `-jar` directive (since _3.6.5_ use `java -jar lib/interlok-boot.jar`,passing in any JVM properties and command-line arguments as appropriate. If the JVM classpath has been set manually prior to starting the adapter, then note that the `-jar` directive forces the JVM to ignore any classpath that might have been specified. If you’re happy with the manual classpath then use `com.adaptris.core.management.SimpleBootstrap` as the main class. This class will not cause any additional classpath initialisation to happen (i.e. `./config`, `./lib/*.jar` and `lib/*.zip` are not added to the classpath).

## Commandline Switches ##

It is possible to invoke the adapter with a number of different switches. These switches will cause the adapter to output some debugging information and then terminate.

|Switch | Description |
|----|----|
|-version| Prints out the version number of Interlok along with any optional sub-components|
|-configtest| Parses the property file, and the associated configuration to be unmarshalled. It also checks that the license is valid for the configuration. It does not check that the configuration is valid (e.g. Broker passwords) for what you're trying to do, it just asserts that the configuration is syntactically correct|

<br/>

```
$ java -jar lib/interlok-boot.jar -version
Bootstrap of Interlok 3.6-SNAPSHOT(2017-02-22) complete
Version Information
  Base Interlok: 3.6-SNAPSHOT(2017-02-22)
  Interlok Annotation Support: 3.6-SNAPSHOT(2017-02-22)
  Interlok Common Classes: 3.6-SNAPSHOT(2017-02-22)
  Interlok Config Pre-Processor: variable substitution support: 3.6-SNAPSHOT(2017-02-22)
  Interlok Config Pre-Processor: xinclude support: 3.6-SNAPSHOT(2017-02-22)
  Interlok Logging components: 3.6-SNAPSHOT(2017-02-22)
```

```
$ java -jar lib/interlok-boot.jar -configcheck bootstrap.properties
Bootstrap of Interlok 3.6-SNAPSHOT(2017-02-22) complete
TRACE [main] [BootstrapProperties] Properties resource is [bootstrap.properties]
TRACE [main] [PropertyResolver] Parsing PropertyResolver URL [jar:file:/C:/Users/lchan/work/runtime/v3-nightly/lib/adp-core.jar!/META-INF/com/adaptris/core/management/properties/resolver]
TRACE [main] [PropertyResolver] Registered Decoders : {password=com.adaptris.core.management.properties.PasswordDecoder}
TRACE [main] [BootstrapProperties] Adding org.jruby.embed.localcontext.scope=threadsafe to system properties
TRACE [main] [BootstrapProperties] Adding org.jboss.logging.provider=slf4j to system properties
INFO  [main] [RuntimeVersionControlLoader] No version control systems found.
INFO  [main] [RuntimeVersionControlLoader] No version control systems found.
TRACE [main] [RuntimeInfoComponentFactory] No RuntimeInfoComponent for class com.adaptris.core.NoRetries
TRACE [main] [RuntimeInfoComponentFactory] No RuntimeInfoComponent for class com.adaptris.core.NullProcessingExceptionHandler
TRACE [main] [RuntimeInfoComponentFactory] No RuntimeInfoComponent for class com.adaptris.core.NullLogHandler
INFO  [main] [UnifiedBootstrap] Adapter created
Config check only; terminating
```
