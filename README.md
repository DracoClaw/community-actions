# Atlas Community Actions Repository
Welcome to the **Atlas Community Action Repository**, a public resource for users of the [Atlas](https://atlasbot.xyz) Discord bot to share custom-made actions with others in the Atlas community. Although every attempt is made to scan all actions submitted to this repository for malicious content, we assume no responsibility for any damages incurred from importing actions from this source into your server.

## How To
### Import Actions From This Repository Into Your Server
If you're interested in importing one of the custom actions found within our repository into your server, here's how to do it:
* Ensure that Atlas is in your server and has the proper permissions to speak, read messages, moderate, etc. If it is not currently in your server, [click here](https://atlasbot.xyz/get) to invite it now. If you have never used Atlas before you may be asked to log in with your Discord account.
* Navigate to the [My Servers](https://atlasbot.xyz/@me/guilds) page and select the server you want to import the action into.
* Back on GitHub, navigate the repository files and find the action file you want to import.
* Open the action file and right click [![](https://i.imgur.com/98icse9.png)](https://www.youtube.com/watch?v=q5Dj5G1kaqI "It's Raw!")
* Click **Save link as** and save the file somewhere you will remember!
* Back on the Atlas dashboard, click on the **Actions** plugin and click the ![Import](https://i.imgur.com/cX5eSQ3.png) Import button. This will open a prompt for you to select the `.action` file you just downloaded. Find it and upload it.
* Congratulations! The imported action should now show up in the **Actions** sidebar.

### Contribute Actions to This Repository
Have an awesome action you want to share? Here's how to get it on this repository for everyone to see. Before uploading your action, you might want to take a look at our **[Guidelines for Contributing](https://github.com/doddsy/atlas-custom-actions#guidelines-for-contributing)** to see if it meets our standards.
* Fork this repository via the ![Fork](https://i.imgur.com/oazJQxh.png) button in the top-right of the screen.
* On the Atlas dashboard, select your action from the actions list on your [dashboard](https://atlasbot.xyz/).
* Click the ![Export](https://i.imgur.com/dvXMSce.png) Export button to save the `.action` file to your local computer.
* Rename your action file in correspondence to the **[Folder Format Requirements](https://github.com/doddsy/atlas-custom-actions#folder-format-requirements)** found at the bottom of this page.
* Navigate to the appropriate subcategory for your action (I.E. Fun folder for a dice-roll action.) and click ![Upload Files](https://i.imgur.com/PmO960X.png)
* Select your action file and commit the changes to your fork.
* Create a pull request and wait for it to be approved by the repository moderators.

## Guidelines for Contributing
**1.** - All uploaded actions  _must_  be submitted in fluent, understandable English. Any pull requests that are made in a language other than English or that contain excessive typos will be automatically denied.

**2.** - All submitted actions must be placed in a folder per the **[Folder Format Requirements](https://github.com/doddsy/atlas-custom-actions#folder-format-requirements)** along with a `README.md` file with a short (or long) description of what the action does. If you make a pull request comprised of multiple `.action` files (hereby referred to as a superaction), include any special setup required in the README.

**3.** - All submitted actions with a **Command** trigger type *must* include a [predefined embedded help menu](https://pastebin.com/raw/HiV8ZszK). There are two categories that all uploaded commands fall into; you must decide which category your command falls in and follow the requirements for either category accordingly:
*  **A. - Command with no subcommands** - If your action does not contain *any* subcommands (or outputs that are altered based upon user input) you must include an embedded help menu triggered by `a!<command> help` that displays the following:
	* A description of what the command does.
* **B. - Command with subcommands** - If your action *does* contain subcommands of any sort, you must include an embedded help menu triggered by **both** `a!<command> help` and `a!command` (no arguments provided) that displays the following:
	* A description of what the (super)action does.
	* A complete list of all valid subcommands.
	* At least one command example.

**4.** - If your (super)action requires static end-user input to function such as a specific channel name or ID, message ID, user ID, etc., to contribute to ease of use, you must declare variables at the beginning of your action code with a `{note}` tag explaining what the information will be used for so the end-user can populate it correctly. See [here](https://i.imgur.com/dVldQxo.png) for an example. You must also declare that there is end-user input required in your (super)action README.

**5.** - Wrappers or aliases for existing Atlas commands do not meet our requirements for contributing. Any action that is submitted in which its soul purpose is to execute a native Atlas command under a disguised name will be automatically denied.

## Folder Format Requirements
We impose restrictions on how files are uploaded and organized to keep the repository neat and tidy. Please remember to follow these requirements when you upload your (super)action or it may be denied.
* **All _standalone_ action files should adhere to the following naming format:**
>**Folder Name:**    
>`AuthorName-ActionName`    
>**Folder Contents:**    
>`ActionName-TriggerType.action`    
>`README.md`    
* **All superaction files should adhere to the following naming format:**
>**Folder Name:**    
>`AuthorName-SuperActionName`    
>**Folder Contents:**    
>`ActionName-TriggerType.action`    
>`...`    
>`README.md`    
* **If multiple people contributed to a (super)action's development, the other author(s) name should be appended to the original author's name:**
>`AuthorName-AuthorName-AuthorName-(Super)ActionName`
-----
#### Repository Moderators
All current moderators of this repository are Atlas staff members.
* doddsy - node#2153
* jam8608 - JaM#8608
* Cykreet - Cykreet#5758
