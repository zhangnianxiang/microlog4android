#Some discussion and thoughts about the configuration

# Introduction #

The existing configuration for microlog is not suitable for microlog4android. The reasons are:

  * There is a real Properties class on Android. In Java ME we use microproperties.
  * The conditions are different in Android than in Java ME (big surprise). Maybe we could use an xml resource for setup.
  * In Java ME we have added code to the appender classes that replaces the missing reflection capabilities in Java ME. This extra code is not necessary on Android.

All in all we expect the solution to be simpler and the footprint should be less.

# The New Configuration Solution #

Some  thoughts/ideas/questions?

  * Should we have automatic configuration? Configuration via a PropertyConfigurator?
  * Should the configuration be backward compatible with microlog? In other words should it be possible to use the simple setup with no Logger hierarchy. Many people have praised how simple it is to setup up Microlog.
  * We should use properties files stored as a resource. Read this investigation for more information: http://myossdevblog.blogspot.com/2010/02/reading-properties-files-on-android.html