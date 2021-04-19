A shortcut application to open YouTube Music in app mode which is a browser window without menus or taps.
This runs in Ubuntu envioronment.
Make sure turn the shortcut file to excutable mode by right clicking this file and clicking "Allow Launching".
Also, place the shortcut file in desktop.
The specifics of keys in codes are as below.


[Desktop Entry]		# Code for Ubuntu to recognise this file as a desktop entry file.

Version=1.0			# Version of this application.

Terminal=false			# Whether to open terminal window when running this file.
				# true: open terminal    false: don't open terminal
				
Type=Application		# Define a type of this file.

Name=YouTube Music		# Name that you can see when turned to excutable mode by activating "Allow Launching".

Exec=chromium --app="https://music.youtube.com"
				# Code that open URL("https://music.youtube.com") following after "--app=".
				# "--app=" allows Chromium to open URL in a browser window in app mode.
				# App mode always opens in new window.
				# You can leave off '--app=' and keep ' "https://music.youtube.com" '
				# if you don't like app mode. 
				# In that case you can put "--new-window" before "https://music.youtube.com"
				# if you'd like to open YouTube Music in new window but not in app mode.
				
Icon=/home/user/pg/YouTubeMusic/icon.png
				# Specify the path of icon file.
