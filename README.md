# Ryujinx Games Compatibility List

Anyone is free to update or share their results here. But you need to follow some guidelines to ensure they're valid.
When you update or add some feedback, please, be as accurate as possible. Also, don't forget to enable `Logging_Enable_Debug = true` in the conf file of Ryujinx. In your pull request, add some lines of the logs, some screenshots, or anything useful to get your results validated. (We can't just accept every single pull request, Sorry!)

Thanks.

## Folder structure

A folder is the same name as a tested game. It's named something like this `new-amazing-ryu-game-supported`, no numbers, no extra characters, just text with spaces replaced with `-`. For now, there are three files in this folder:

* **boxart.png**

   A picture of the actual game case, in PNG format only please. Please do use a clean picture sized at 300px x 486px (or around that).

* **info.json**

   It's a JSON file which contains specific fields (Don't forget to remove comments if you Copy and Paste)
   
```javascript
 { 
	"title_id": 
	[ 
		"0100000000000000", // Game title ids who can be found on switchbrew or in your gamedump too.
		"0100000000000001", // You can add more of them if game is multi region.
		"0100000000000002", // Or if there is an update of the game.
		"XXXXXXXXXXXXXXXX", // If you can't found title id, use "XXXXXXXXXXXXXXXX" one.
		"etc..."
	],
	"name": "Cave Story+",           // Game name in a clean version (folder name is in a raw version).
	"state": "In Game",              // Current state of the game, be revelant or consistent here.
	"state_emu_version": "7ac5f40",  // Last Ryujinx commit of your current executable version (for now).
	"state_last_date": "19/05/2018", // Date of your test.
	"comment": "Explain what going on here.", // Be as precise and detailed as possible.
	"nickname": "YourNickname"       // We just need to know who made the changes, and also give credit.
}
```

* **screenshot.png** (Optional)

   Please ensure you have a full screenshot of the Ryujinx with the game displaying; please only use a `.png` format only. It must be  1280px x 720px (or around that). If the game don't show anything in the emulator, please don't provide anything for this file; and the `boxart.png` will be used instead.
