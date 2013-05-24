PHP-Timer
=========

Simple PHP script Timer

Usage:
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

// Should give me 5 seconds <-- STOP
$timer->stop();
echo $timer->getTime();
