# The Philly Talk Podcast with YouTube API
Write a short sentence or two about this project and what it does. Be sure to include a link and a screenshot (we're front end devs so we can actually see our work!).

**Link to project:** https://phillytalkpodcast.netlify.app/

![alt tag](https://user-images.githubusercontent.com/47239035/156244083-f0deaedc-904b-4f9f-a6da-40b076d3ca34.png)

## How It's Made:

**Tech used:** HTML, CSS, JavaScript, Google/Youtube API
Authorize a request
Description: The auth.js script demonstrates how to use the Google APIs Client Library for JavaScript to provide API access and authorize user requests. All of the subsequent samples on this page use this script to authorize their requests.

For requests that do not require authentication, you could also use the key query parameter to specify an API key rather than using OAuth 2.0.

Note: You need to update the client ID in the auth.js file. You can obtain your own client ID by registering your application in the Google Developers Console.

Do resumable uploads with CORS
Method: youtube.videos.insert Description: This code sample demonstrates how to execute a resumable upload using XHR/CORS.

Create a playlist
Method: youtube.playlists.insert
Description: This JavaScript code creates a private playlist and adds videos to that playlist. (You could, of course, modify the code so that it creates a publicly visible playlist or so that it checks a form value to determine whether the playlist is public or private.) Note that you need to update the client ID in the auth.js file to run this code.

The HTML page uses JQuery, along with the auth.js and playlist_updates.js JavaScript files, to display a simple form for adding videos to the playlist.

Retrieve my uploads
Method: youtube.playlistItems.list
Description: The JavaScript sample code performs the following functions:

It retrieves the playlist ID for videos uploaded to the user's channel using the API's channels.list method. This API call also sets the mine parameter to true to retrieve channel information for the authorizing user.
It passes that ID to the playlistItems.list method to retrieve the videos in that list.
It displays the list of videos.
It constructs next and previous page buttons and sets their visibility based on the information in the API response.
The HTML page uses JQuery, the auth.js and my_uploads.js JavaScript files, and a CSS file to display the list of uploaded videos.

Search by keyword
Method: youtube.search.list
Description: This code sample calls the API's search.list method to retrieve search results associated with a particular keyword. The HTML page uses JQuery, along with the auth.js and search.js JavaScript files, to show a simple search form and display the list of search results.

Upload a video
Method: youtube.videos.insert
Description: This JavaScript sample performs the following functions:

It retrieves the channel name and thumbnail of the authenticated user's channel using the API's channels.list method.
It handles the video upload to YouTube using the resumable upload protocol.
It polls for the uploaded video's upload and processing status using the API's videos.list method by setting the part parameter value to status.
The HTML page uses JQuery, the cors_upload.js and upload_video.js JavaScript files, and the upload_video.css file to upload a video file to YouTube.

Note that if you use this code in your own application, you must replace the value of the data-clientid attribute in the code for the Sign-In Button with your project's client ID. The only valid JavaScript origin for the client ID in the sample code is http://localhost. This means that you could test the sample locally, but it would not work in your production application.

Calling the Analytics API
Method: youtubeAnalytics.reports.query
Description: This sample uses the YouTube Data and YouTube Analytics APIs to retrieve YouTube channel metrics. The samples use the Google APIs JavaScript client library to demonstrate API functionality. The Building a Sample Application document walks you through the steps of building this application and discusses different portions of this code in more detail.


In addition to the JavaScript file described above, the HTML page uses jQuery, which provides helper methods to simplify HTML document traversing, event handling, animating and Ajax interactions. It also uses the Google API loader (www.google.com/jsapi), which lets you easily import one or more Google APIs. This example uses the API loader to load the Google Visualization API, which is used to chart the retrieved Analytics data. Finally, the Google APIs Client Library for JavaScript helps you to implement OAuth 2.0 authentication and to call the YouTube Analytics API.



## Optimizations
*(optional)*

You don't have to include this section but interviewers *love* that you can not only deliver a final product that looks great but also functions efficiently. Did you write something then refactor it later and the result was 5x faster than the original implementation? Did you cache your assets? Things that you write in this section are **GREAT** to bring up in interviews and you can use this section as reference when studying for technical interviews!

## Lessons Learned:

No matter what your experience level, being an engineer means continuously learning. Every time you build something you always have those *whoa this is awesome* moments. This is where you should share those moments! Recruiters and interviewers love to see that you're self-aware and passionate about growing.

## Examples:
Take a look at these couple examples that I have in my own portfolio:

**Palettable:** https://github.com/alecortega/palettable

**Twitter Battle:** https://github.com/alecortega/twitter-battle

**Patch Panel:** https://github.com/alecortega/patch-panel



