CIS 520 Project 0
Chord Livingston
1/24/2020

Changes made to create alarm-mega test:

1. Created new alarm-mega.ck under src/tests/threads by copying from alarm-multiple.ck and changing the value to check_alarm(70)
2. Modified Make.tests to include "alarm-mega"
3. Modified tests.c to include "{"alarm-mega", test_alarm_mega},"
4. Modified tests.h to include "extern test_func test_alarm_mega;"
5. Modified alarm-wait.c to include the test_alarm_mega function with an iteration value of 70
