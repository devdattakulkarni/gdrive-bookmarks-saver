Bookmarks uploader Chrome extension
------------------------------------

Loading the extension:
----------------------

1) Clone this repository

2) Open Chrome

3) Browse to: "chrome://extensions" in the navigation bar

4) Check "Developer mode"

5) Click load unpacked extension

6) Browser to the directory where you have cloned this repository


Using the extension:
--------------------

1) Once the extension is loaded it should show as a icon on Chrome

2) Click it

3) You will see two buttons - "Authorize" and "Upload bookmarks"

4) Click "Authorize". You will be directed to a login screen where
   you provide your Google SSO to grant access to the extension to make
   read/write calls to your Google Drive account (The extension uses OAuth2).

5) Open drive.google.com

6) Now click the icon again. The buttons should be now "Deauthorize" and
   "Upload bookmarks"

7) Click "Upload bookmarks". You should see a progress bar indicating the
   bookmark upload is in progress.

8) When the upload completes you should see a file named "Bookmarks.txt"
   in your Google Drive. This file contains all of your bookmarks


(*) If the upload is taking more than a few seconds, click the "Upload bookmarks"
   button again. I have seen intermittent issue with uploading failing. Retrying
   should work

(**) You may need to refresh the Google Drive tab to see the uploaded Bookmarks.txt file.


Notes:
------
Starter code to upload files to gdrive taken from:
https://github.com/GoogleChrome/chrome-app-samples/samples/gdrive

Modified that code as follows:
- Converted the packaged app to an extension by changing manifest.json
- Added bookmarks permission in manifest.json
- Added a method 'uploadBookMarks' in app.js that reads the bookmarks
  and calls the upload method to upload them
- Modified upload.js to set the filename to a static name (Bookmarks.txt)
- Modified main.css to remove the background image css
- Modified main.html as follows:
  - removed the "doc in docs" list of elements
  - removed the "Refresh" button
  - changed "Google Drive Uploader" from heading and title


