A chrome extension to upload bookmarks to Google drive
-------------------------------------------------------

Loading the extension:
----------------------

1) Open Chrome

2) Browse to: "chrome://extensions" in the navigation bar

3) Check "Developer mode"

4) Click load unpacked extension

5) Browser to the directory where you have cloned this repository


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


