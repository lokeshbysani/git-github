

Instructions:

 



What is Stopwatch?



Stopwatch
is a timepiece that can be started or stopped for exact timing as of a race or
any activity

It is very
useful when you want to do some performance testing in your code or to get
timings for whatever reason.

It is
useful for micro-benchmarks in code optimization. It can perform routine and
continuous performance monitoring.

A Stopwatch instance
measures the elapsed time for one interval or the total of elapsed time across
multiple Intervals.

Normal scenario in
stopwatch includes call the start
method and then call stop method
then measure the time difference using elapsed
method.











//new Stopwatch Instance



Stopwatch watch = new
System.diagnostics.stopwatch();



ElapsedTime : This is the time difference between the start time when we initialized
the stopwatch instance and  current time.



ElapsedTime =
StartTime - CurrentTime



Activities:

1.    
StartNewStopwatch:

Stopwatch.Activities.StartNewStopWatch



Creates a New Stopwatch Instance and sets the elapsed time i.e time
difference to zero and starts measuring the time .



            Properties:



            Output:




            Stopwatch:
The Stopwatch variable to store the stopwatch instance returned.



Common:

DisplayName - The display
name of the activity.



Misc:

Private - If selected, the values of variables and arguments are no longer
logged at Verbose level.



 



 

 

 

2.StopStopwatch

Stopwatch.Activities.StopStopWatch



This tells
the Stopwatch to capture the current tick count of the system, also very
accurate.



Properties:



            Input:




            Stopwatch:
The Input is stopwatch instance (mandatory Field).



            Common:

DisplayName - The display name of the activity.



Misc:



Private - If selected, the values of variables and arguments are no longer
logged at Verbose level.



 



 



 



3.ResetStopwatch:

Stopwatch.Activities.ResetStopWatch



It will stops
measuring the time interval and resets the elapsed time(time difference) to
zero.



Properties:



            Input:




            Stopwatch:
The Input is stopwatch instance (mandatory Field).



            Common:

DisplayName - The display name of the activity.



Misc:



Private - If selected, the values of variables and arguments are no longer
logged at Verbose level.



 

 

4. RestartStopWatch:

Stopwatch.Activities.RestartStopWatch



Restart
sets the Elapsed Time  to zero. It then
calls Start again on the Stopwatch, so you can time further statements. This is
like calling Reset and Start.



Properties:



            Input:




            Stopwatch:
The Input is stopwatch instance (mandatory Field).



            Common:

DisplayName - The display name of the activity.



Misc:



Private - If selected, the values of variables and arguments are no longer
logged at Verbose level.



 

 

 

 

 

5. StartStopwatch:

Stopwatch.Activities.Start



The Start method tells the Stopwatch to store the current time. It
queries Windows to find the current tick count of the system



Properties:



            Input:




            Stopwatch:
The Input is stopwatch instance (mandatory Field).



            Common:

DisplayName - The display name of the activity.



Misc:



Private - If selected, the values of variables and arguments are no longer
logged at Verbose level.



6. IsStopwatchRunning:

Stopwatch.Activities.IsStopWatchRunning



A Stopwatch instance
is either running or stopped; use IsRunning to determine the current state of a
Stopwatch



Example:
watch.IsRunning() will give true or false if stopwatch instance is running or
stopped respectively.



Properties:



            Input:




            Stopwatch:
The Input is stopwatch instance (mandatory Field).



            Output:



            Bool: The output is Boolean variable which give
true or false based on the running state



            Common:

DisplayName - The display name of the activity.



Misc:



Private - If selected, the values of variables and arguments are no longer
logged at Verbose level.



 



 



 



7.GetStopWatchElapsedTime:



Stopwatch.Activities.GetStopWatchElapsedtime



 



This will return the total elapsed time in different formats



The stopwatch.Elapsed result is stored as a TimeSpan
Structure and is
formatted as dd.hh:mm:ss.ff: 



dd = days  



hh = hours



mm = minutes



ss = seconds



ff = fractions of a second



Properties:



            Input:




            Stopwatch:
The Input is stopwatch instance (mandatory Field).



            Output:



             Elapsed:Returns the total elaped time in Timespan format 00:00:02:5412



            ElapsedMilliseconds:Returns the
total elapsed milliseconds



ElapsedTicks:Returns the total timer ticks



               Hours: Returns the hours in Elapsed output Equivalent to
elapsed.Hours



               Minutes: Returns the
Minutes in Elapsed output Equivalent to elapsed.Minutes



               Seconds: Returns the
Seconds in Elapsed output Equivalent to elapsed.Seconds



               Milliseconds:
Retruns the Milliseconds in Elapsed output Equivalent to elapsed.Milliseconds



               ElapsedTicks: This is
internally a readonly signed System.Int64 value. When you capture ElapsedTicks,
you have to manually do the calculations to convert the values to seconds



Stopwatch ticks are far more accurate, when the
IsHighResolution property is true. Otherwise, they are equivalent.



            Common:

DisplayName - The display name of the activity.



Misc:



Private - If selected, the values of variables and arguments are no longer
logged at Verbose level.



 



 



 



