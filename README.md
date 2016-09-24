# MACROLOG #
A simple head-only log system. 

You must include two directories, 'macrolog/include' and 'macrolog/iter/include'. 

## Requirements ##
Compile option: --std=c++11 

## Log settings ##
Some components might print logs to ```stderr```.

You can redirect the log destination of each level by using:
```
iter::SetLogDestination(iter::INFO, "notice.log");
iter::SetLogDestination(iter::WARN | iter::ERROR | iter::FATAL, "warning.log");
```

Compile options:
* ```-DDEBUG``` : Enable debug log.
* ```-DITER_LOG_DISABLE``` : Disable all of the logs.

