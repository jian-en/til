# Define cronjob execution time

The setting of time for cronjob must be very tricky and hard to remember. Actually there are only 5 values:
	* minute
	* hour
	* day
	* month
	* day-of-week(0 ~ 7 both 0 and 7 are Sunday)

I think two example will illustrate the grammar clearly:

```bash
0 8 1,20 * *
```
It means to run a script at 8:00am every 1st and 20th.

```bash
* */2 * * * 
```
It means to to run a script every 2 hours.

[source](http://www.thesitewizard.com/general/set-cron-job.shtml)