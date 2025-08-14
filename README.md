# Online Casino Simulator

This repository contains a simple online casino game with three different games: Blackjack, Slots, and Three Card Poker. The application is built using HTML, CSS, and vanilla JavaScript, and it uses Firebase Firestore for managing user funds.

🎲 Games

    Blackjack: Play against the dealer. Hit, Stand, or Double Down to get as close to 21 as possible without going over.

    Slots: Spin the reels and try to get three matching symbols for a jackpot.

    Three Card Poker: Bet against the dealer to see who has the best three-card hand.

💻 Setup and Installation

To get this project up and running, you'll need a web server like Apache2 to host the files. The game uses Firebase Firestore to save user data, but the Firebase configuration is dynamically injected, so you can host it as is for a local, in-browser experience.

1. Install Apache2

First, install Apache2 on your system.

    On Debian/Ubuntu:
    Bash

sudo apt update
sudo apt install apache2

On CentOS/RHEL:
Bash

sudo yum update
sudo yum install httpd
sudo systemctl start httpd
sudo systemctl enable httpd

On macOS (using Homebrew):
Bash

    brew install httpd
    sudo brew services start httpd

2. Locate the Apache2 Web Directory

The default web directory for Apache2 varies by operating system.

    Linux (Debian/Ubuntu): /var/www/html/

    Linux (CentOS/RHEL): /var/www/html/

    macOS (Homebrew): /usr/local/var/www/

3. Place the Game Files

Once you have Apache2 installed, move the index.html and style.css files from this repository into your Apache2 web directory.
Bash

# Example for Ubuntu/Debian
sudo cp index.html style.css /var/www/html/

4. Access the Game

After moving the files, open your web browser and navigate to http://localhost. The online casino should now be ready to play!

📝 Project Structure

    index.html: The main HTML file containing the game's user interface and all the JavaScript logic.

    style.css: The CSS file for styling the game.
