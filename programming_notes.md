# Version 2.x.x common issues #


# Version 2.x.x Pascal issues #
  * When creating console application directly in Pascal, take notice of **BauglirSynchronizeThreads** variable in **BClasses** unit. This variable is responsible for synchronizing to main GUI thread, since console application does not have thread, than in case your main console thread is blocking, you should set this variable to `true`. Variable is automatically set to `true` in libraries. When using library, application should be responsible for threads synchronizing (simultaneous resource access)