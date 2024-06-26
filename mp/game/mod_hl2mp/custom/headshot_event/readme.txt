1. Place this folder to your hl2mp\custom folder
2. Install csd.tff in system from "mp\game\mod_hl2mp\custom\headshot_event\resource\csd.ttf" or steal it from fresh install of Counter-Strike: Source
3. Add to your hud's "resource\clientscheme.res" text block after "HL2MPTypeDeath"
		"CSTypeDeath"
		{
		   "1"
		   {
				"name"  "csd" // csd.ttf
				"tall"  "32"
				"weight" "0"
				"additive" "1"
				"antialias" "1"
				"custom" "1" [$OSX]
		   }
		}	
		
4. Add to your hud's "scripts\mod_textures.txt" text block after "death_crowbar"
		"death_headshot"
		{
				"font"		"CSTypeDeath"
				"character"	"D"
		}
		
5. Place modified "client.dll" to your hl2mp\bin folder and run game with -insecure flag to prevent VAC ban.
