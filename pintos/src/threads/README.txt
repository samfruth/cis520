-----------PROJECT 0-----------
OBJECTIVE:
	This project creates a new test, 'alarm-mega', that generates 70 alarms
	in order to test for a successful installation of pintos. In order to
	accomplish this, I needed to find all of the files that contained a 
	reference to 'alarm-multiple' since the functionality would be so similar. 

FILES CHANGED:
	"alarm-mega.ck": Created a new test file called "alarm-mega.ck" which is 
		nearly identical to the "alarm-multiple.ck" test, except generates
		ten times as many alarms.

	"tests.c": Added a line '{"alarm-mega", test_alarm_mega},'

	"tests.h": Added 'extern test_func test_alarm_mega;'

	"alarm-wait.c": Added functionality below.
		void
		test_alarm_mega (void)
		{
			test_sleep (5, 70);
		}

	