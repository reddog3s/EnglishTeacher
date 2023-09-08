# English Teacher
App allowing user to learn English vocabulary and take test. It's created in state machine architecture. Works under Labview 2022 Q3.

# Description of the app
## GUI
* Start Learning - starts learning mode.
* Start Test - starts test mode.
* Stop - stop current mode.
* Exit - exits app.
* Polish - control, displays polish words.
* English - control, displays english words and allows to type them.

## How it works?
After starting app, user chooses one of the available modes by clicking Start Learning or Start Test button. After clicking both buttons are grayed out unitl Stop or Exit are pressed or mode ends.<br>
In Learning mode, controls display Polish and English words automatically in following order:
1. Word in Polish shows up.
2. After 3 seconds translation to in English shows up.
3. After 2 seconds both words disappear and controls remain empty for 1 second.
4. Return to point 1.


In Test mode Polish words are displayed and user has to type English translation. It works in the following way:
1. Word in Polish shows up.
2. User has 5 seconds to type word in English.
3. Answer validation - font in English control is being bold out and:
	* if answer is correct background color changes to green,
	* if answer is incorrect background color changes to red,
4. Wait 1 second.
4. Return to point 1.

Words are loaded from words.txt encoded in ANSI (Windows default encoding).
