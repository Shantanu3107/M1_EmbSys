
## TEST PLAN
## o For every feature,define a test case
## o How to run that feature
## o Define expected behaviour
## o Capture the actual result

## High Level Test Plan
|Test ID|Description|EXP I/P|EXP O/P|Result|
|--|--|--|--|--|
|HR_01|Turn on power supply|Power supply|Ultra-sonic sensor will turn ON/OFF|Passed|
|HR_02|Ultra-sonic should sense the ECHO or sound|There should be sound or a source of sound|Sensor will sense the sound|Passed|
|HR_03|LCD should display the distance|After sensing the micro controller will display the distance|Distance should be displayed|Passed|


## Low Level Test Plan
|Test ID|Description|Exp I/P|Exp O/P|Result|
|--|--|--|--|--|
|LR_01|Sensor should sense the sound when it is in a specified range|Sound in specified range|Sensor will sense the sound|Passed|
|LR_02|Sensor should not sense the sound when not in specified range|Sound is not in specified range|Sensor will not sense the sound|passed|
|LR_03|Distance should be displayed when sensor senses the sound|Taking input from controller|LCD will display distance |Passed|
|LR_04|Distance should not be displayed when sensor does not sese the sound|Taking input from the controller|LCD will not display distance|Passed|
