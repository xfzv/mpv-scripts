### SmartCopyPaste Detailed Explanation of Features
 - **URL Paste:** Copy any video URL from anywhere and play it by pressing **[ctrl]**+**[v]** directly into mpv
	- *Before accepting paste:*
		- It avoids accidental video change, **it only accepts pasting new video if there is no video already playing**
		- Supports youtube-dl extension, so pasting youtube page link should work immediately (no need to find the exact video link) this is for any supported site in youtube-dl extension. [List of youtube-dl supported sites](https://rg3.github.io/youtube-dl/supportedsites.html)
	- *Feature demonstration:*
	- ![URL pasted into mpv](https://media.giphy.com/media/uWczvTWFVcxwXG9zJI/giphy.gif)
 - **Powerful Paste:** Copy any video or its path from anywhere and play it by pressing **[ctrl]**+**[v]** directly into mpv
	 - Supports copying the video itself and pasting it inside mpv
	 - Supports copying the path of video and pasting it inside mpv
	 - Supports native windows copy as path feature for videos and pasting inside mpv
	- *Before accepting paste:*
		 - It checks if the pasted path ends with a supported video extension such as **.mkv**
		 - It checks if the pasted path is not an empty extension such as a file-named (**.mkv**) 
		 - It avoids accidental video change, **it only accepts pasting new video if there is no video already playing**
	 - *Feature demonstration:*
	 - ![Local videos pasted into mpv](https://media.giphy.com/media/2zcXmABJzxY4XZfSmg/giphy.gif)
 - **Copy Video Path WITH Time:** Copy the video path and time reached by **[ctrl]**+**[c]**
  	 - Enables opening and resuming the video the video by pasting 
	 - It also enables you to share path with people (such as video url) with your resume time
 - **Copy Video Path WITHOUT Time:** Copy the video path alone by **[ctrl]**+**[C]**
	 - Enables opening the video but without resuming by pasting
	 - It also enables you to share path with people (such as video url) without resume time
 - **Resume to Copied Time:** Copy the time of the video by **[ctrl]**+**[c]** in mpv then resume the video at any time
	 - Supports pasting in the player immediately to open copied video along with its seeking time
		 - It avoids accidental video change,  it checks if the pasted time was of the same video
	 - Supports automatic seeking to the time you copied when you open the copied video (even without pasting)
		 - It avoids seeking wrongly, it checks if the opened video was the copied video 
	 - Supports the mentioned features in both local files and URLs
		 - It enables you to share path with people (such as video url) with resume time
		 - Or to open the video again and resume it by pasting path into mpv 
	 - Feature demonstration
	 - ![Resume copied time by paste](https://thumbs.gfycat.com/LeanPepperyCopperbutterfly-size_restricted.gif)
 - **(PRO) Save Clipboard to a Log File:** The copies from mpv, and the pastes into mpv will be kept in a log for far more powerful copy paste experience, and a history that you can find useful.
	 - Copying your open video by **[ctrl]**+**[c]** copies the video and its time while saving it to a log file located in `%APPDATA%\mpv\mpvClipboard.log`
	 - Pasting a video into mpv plays the video and also saves it to a log file located in `%APPDATA%\mpv\mpvClipboard.log`
 - **(PRO) Powerful Bookmark:** Copy the time of multiple videos by **[ctrl]**+**[c]** in mpv then resume any video even after clipboard is overwritten or it is cleared.
	 - Using the log, copying videos adds a bookmark point, so you can resume to your copy position in any and all copied videos by **[ctrl]**+**[v]**
	 - Even for multiple videos you copy, their resume time will be saved. You can resume to exact position by pasting in each video
 - **(PRO) Remember Last Video Copied or Last Video Pasted:** The last copied or pasted video will remain even after device restarts or clipboard changes.
	 - If clipboard is replaced with anything such as 'random text', you can still paste the video ;)
	 - Paste to play and resume anything copied even if clipboard no longer contain the time
	 - If mpv is idle you can always paste your last copied mpv video or last pasted video into mpv to play it then paste again to resume. (this works even if you have different types of files in clipboard)
 - **(PRO) Quick access to Videos Clipboard History:** If mpv is idle, press **[ctrl]**+**[c]** to access your clipboard history
	 - This feature provides quick access to your videos clipboard history to find your previous copied or pasted videos and play or share them.