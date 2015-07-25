# Introduction #

The project is now in the startup phase and as such we do not have much to write here.


# Todo #

These are the things that is needed to be done within the microlog4android.

For V1.0:

  * Remove "reflection" methods found in the appenders that is used in Java ME to circumvent the missing reflection capabilities.
  * Implement configuration. A new PropertyConfigurator maybe? Automatic configuration?
  * Write a HTTPAppender

Future versions:
  * Add support for registering M4A as default uncaught exception handler.
  * Write an EmailAppender or similar. Should make it possible to e-mail your log files when the get to big and/or in an emergency situation.
  * Make the PatternFormatter support new features to make it compatible with the PatternLayout in Log4j. In other words implement features that was not possible in Java ME.
  * Write a Google App Engine Appender?
  * Write a Google App Engine server "thingie"

# Done #

These are the things that we have finished from out todo list.
  * Change the package name com.google.code.microlog4android
  * Write a new FileAppender
  * Write a DatagramAppender
  * Write SyslogAppender
  * Write build script (Gradle). This should at least create distributables.
  * Code cleanup
  * Optimize for use in a Java SE environment. For example replace Vector usage with a List implementation. Replace Hashtables with Map etc etc.