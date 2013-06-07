(* 

This script will launch two terminal windows, one with your default settings and a second one, larger, with bigger font, black on white to present. Once launched, a screen session is created and both windows will display exactly the same thing.

This script was inspired by this article http://www.jaharmi.com/2013/05/27/demo_mirrored_terminal_sessions_with_screen

Once finished, you can quit screen using CTRL-D

*)

tell application "Terminal"
  activate
	
	do script "screen -S PRESO"
	tell window frontmost
		set title displays device name to false
		set title displays shell path to false
		set title displays window size to false
		set title displays custom title to true
		set custom title to "Preso"
	end tell
	
	do script "screen -x PRESO"
	tell window frontmost
		set number of rows to 24
		set number of columns to 80
		set font name to "Menlo"
		set font size to 32
		set normal text color to {0, 0, 0, 0}
		set background color to {65535, 65535, 65535, 65535}
		set cursor color to {0, 0, 0, 0}
		set title displays device name to false
		set title displays shell path to false
		set title displays window size to false
		set title displays custom title to true
		set custom title to "Demo"
	end tell
	
end tell
