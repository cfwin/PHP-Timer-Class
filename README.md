PHP-Timer
=========

Simple PHP script Timer

Usage:
``` php
$timer = new Timer();

// Start timer <-- COUNT
$timer->start();
usleep(1000000);

// Don't count this time <-- PAUSE
$timer->pause();
usleep(1000000);

// And start again <-- COUNT
$timer->resume();
usleep(5000000);

// Don't count this time <-- PAUSE
$timer->pause();
usleep(1000000);

// And start again <-- COUNT
$timer->resume();
usleep(1234567);

// <-- STOP
$timer->stop();
echo $timer->getTime();
```

Outputs: 
```
7.2406 seconds
```
