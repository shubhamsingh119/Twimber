Twimber – A Mini Twitter Clone 🐦

Twimber is a lightweight Twitter-style microblogging app built using HTML, CSS, and Vanilla JavaScript.
Users can post tweets, like, retweet, and view threaded replies — all rendered dynamically from a data file.

This project focuses on DOM manipulation, event handling, and modular JavaScript using ES modules.

🚀 Live Demo

👉Netlify link 

📁 Project Structure
📦 Twimber
 ┣ 📂images
 ┃ ┣ troll.jpg
 ┃ ┣ musk.png
 ┃ ┣ tcruise.png
 ┃ ┣ chucknorris.jpeg
 ┃ ┣ flower.png
 ┃ ┣ overflow.png
 ┃ ┣ love.png
 ┃ ┗ pfpp.jpg
 ┣ 📄 index.html
 ┣ 📄 index.css
 ┣ 📄 index.js
 ┗ 📄 data.js

🧠 Features
✅ Tweet Feed

Renders tweets dynamically from tweetsData

Displays profile picture, handle, text, likes, retweets, and replies

❤️ Like System

Click the heart icon to like/unlike a tweet

Counter updates instantly

Uses a .liked CSS class for visual animation

🔁 Retweet System

Click retweet icon to toggle retweet

Count updates dynamically

Uses .retweeted class for UI highlight

💬 View Replies

Click comment icon to open or hide the replies section

Replies are stored in each tweet's replies array

✍️ Create a Tweet

Enter text in the input box and click Tweet

New tweet is added to the top using unshift()

uuid is generated using JSPM’s UUID import

🛠️ Tech Used
Technology	Usage
HTML5	App structure
CSS3	UI styling and layout
JavaScript (ES Modules)	Logic, rendering, interactions
UUID (via jspm.dev)	Unique tweet IDs
Font Awesome	Icons for like, retweet, comment
Google Fonts	Typography
📜 data.js Structure

Tweets are stored as objects:

{
    handle: "@Elon",
    profilePic: "images/musk.png",
    likes: 6500,
    retweets: 234,
    tweetText: "I need volunteers for a one-way mission to Mars 🪐",
    replies: [
        {
            handle: "@TomCruise",
            profilePic: "images/tcruise.png",
            tweetText: "Yes! Sign me up!"
        }
    ],
    isLiked: false,
    isRetweeted: false,
    uuid: "some-unique-id"
}

🧩 Core Files
index.html

Contains layout structure

Loads Font Awesome and Google Fonts

Loads index.js as a module

index.css

Contains all UI styling

Styles tweets, buttons, profile pics, layout, and interactions

index.js

Handles:

Like / Retweet toggle

Showing replies

Adding new tweets

Rendering feed HTML

Event delegation with document.addEventListener("click")

data.js

Exports the tweetsData array

Contains initial tweets and replies

📸 Screenshots

(Add your own screenshots here)

🌐 How to Run Locally

Clone the repository:

git clone <repo-url>


Open the folder:

cd twimber


Run directly in your browser (no build tools needed):

Double-click index.html

or use Live Server (VS Code)

📌 Future Improvements

Dark mode 🌙

LocalStorage persistence

Image uploading

Hashtags & trends

User authentication mock

🙌 Credits

Inspired by Twitter UI
Icons from Font Awesome
UUID from jspm.dev
