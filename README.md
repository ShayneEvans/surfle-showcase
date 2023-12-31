# [Surfle](https://surfle.xyz) Showcase
Showcasing my website: https://surfle.xyz

Surfle was created as derivative of [guessthe.game](guessthe.game) and [framed.wtf](framed.wtf) but specializing in the game mode Counter-Strike surf. There have been over 1,000 unique surf maps created over the 20+ year history of Counter-Strike surf and I have compiled their information in a database where one will be picked daily at random where users can attempt to guess it. This was a passion project for me because the surf game mode has brought me many great friendships and memories over the years, so getting to make something that surfers can play was pretty neat! Surfle utilizes browser local storage to save information such as the game state and player statistics. I will show the important parts of the site now

# The Game
<p align="center">
  <img src="https://github.com/ShayneEvans/surfle-showcase/blob/main/screenshots/surfle-game.PNG?raw=true" alt="Surfle Game"/>
</p>



Above shows what the user will see on a new Surfle game. The very top is the header which appears on all pages of the website which allows the user to go to previous days, gives instructions on how to play, individual stats, or more info about the website. Below the surfle game number is listed, in this screenshot it is the first day so it says 'Surfle Game #1'. Below this is the first hint image that the user must utilize to guess the surf map. The user can type what map they think it is in the search box and it will autofill some results based on what they typed in. if they guess wrong after hitting submit the 2nd hint image will be shown and so on until the final 6th image. At the bottom is a timer until the next Surfle game will be posted on the website, the arrow button to the right will let the user play the next day.

https://github.com/ShayneEvans/surfle-showcase/assets/70344759/c610f063-f751-4df8-a6ae-994be6c81e76

The above video showcases the autocomplete feature in the input box and what happens when the user clicks the 'Submit' button. Once the submit button is pressed if the guess is wrong the next hint will be shown (this can be seen above the input box when the 2 becomes highlighted going from hint image 1 to 2) as well as the incorrect guess below the input box. If the user enters the correct surf map the following image will be shown:

<p align="center">
  <img src="https://github.com/ShayneEvans/surfle-showcase/blob/main/screenshots/end-game.png?raw=true" alt="Surfle End Game"/>
</p>

Once the game has concluded by the user either guessing correctly or missing all their guesses the results will be shown below the hint image as seen above. A message congratulating the user will appear if they won, or saying "Unlucky" if they lose. Below this message 5 new buttons appear: 'Share Results', 'Show Guesses', 'Play Previous Days', 'See Stats', and 'Youtube Video'. The share results button allows the user to copy their results to clipboard where they can share it with their friends, this can be seen below:

<p align="center">
  <img src="https://github.com/ShayneEvans/surfle-showcase/blob/main/screenshots/surfle-share.png?raw=true" alt="Share Results"/>
</p>

The 'Show Guesses' button will show a list of user guesses with 'Skipped' appearing if the user pressed the skipped button. The 'Play Previous Days' button will send the user to the previous games page just like the button in the header. The 'See Stats' button will show complete user stats for the current Surfle day which is only accessible after the user has completed the game. The 'YouTube Video' button opens a seperate tab with a youtube video showcasing the most recent world record on the map.

# Statistics
<p align="center">
  <img src="https://github.com/ShayneEvans/surfle-showcase/blob/main/screenshots/daily-stats.PNG?raw=true" alt="Surfle Daily Stats"/>
</p>

The above image shows the statistics page for Surfle game #1 which includes a dougnut chart showing which guess the user correctly identified the map as well as how many users failed to guess the map. The top 5 correct guesses are shown as well as the number of games that have been concluded below that.

<p align="center">
  <img src="https://github.com/ShayneEvans/surfle-showcase/blob/main/screenshots/player-stats.png?raw=true" alt="Surfle User Stats"/>
</p>

The individual player statistics can be viewed by clicking on the 'Stats' button on the header. These stats show the number of games played, number of games won, win percentage, current winning streak, maximum winning streak, and a bar chart that displays the win distribution for each game. These stats are stored and obtained utilizing local storage in the browser.


## Technologies Used

### Backend
- **Python**: Version 3.11
- **Django**: A Python web framework.
- **DateTime**: Used for handling date and time operations.
- **psycopg2**: A PostgreSQL adapter for Python.
- **PostgreSQL**: A powerful open-source relational database system used to store daily statistics.
- **Digital Ocean Droplet**: A cloud hosting solution for hosting the PostgreSQL database and website code.

### Deployment
- **Nginx**: A web server used for serving web content.
- **Gunicorn**: A Python Web Server Gateway Interface (WSGI) HTTP server for deploying Django applications.

### Frontend
- **HTML, CSS, JavaScript**: Frontend technologies for building the user interface.
- **Local Storage**: Used for storing data on the client-side.

### Hosting
- **Digital Ocean Droplet**: Hosting the PostgreSQL database and the website.
