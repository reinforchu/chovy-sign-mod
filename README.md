#ChovyProject v2
Created by SquallATF, and Li! 

\- chovy-sign is an application to allow you to convert PSP and PS1 ISO's to be playable on unmodified PSVita's

Setups:
You need a valid (offical) PSP or PS1 license,
i recommend getting; Petz Saddle Club, LocoRoco Midnight Carnival, or Ape Quest Starter Pack
atleast one of these are free in *most* regions; 

however failing that, you can also use a PSP DLC license- 

-- if you don't have a hacked PSVita:
Note: If the game you are using to do this with any games besides PETZ SADDLE CLUB, LOCOROCO MIDNIGHT CARNIVAL or APE QUEST STARTER PACK; 
you will be limited to the same game type as the license is for,
i.e a PS1 game will only be usable to create a PS1 game,
and a PSP game will only be usable to create a PSP game
(this is different' if you use the henkaku method)

Copy the game to your PC using Content Manager,
open chovy-sign2 and click the "Get Keys" button
 -- if you are using "APE QUEST, LOCOROCO MIDNIGHT CARNIVAL, or PETZ SADDLE CLUB, and want to make a PS1 game select "KEYS.TXT" instead-)
select "EBOOT.PBP" method, click on the game
(note: there may be some issues if you try this while having DLC for the game installed ...)

you should see the RIF and KEY fields populate, and your good to go!

-- If you have a hacked PSVita:
note: you can still use the unhacked vita method if you would like 
(i.e if your only wanting to make PSP games, or are using PETZ SADDLE CLUB, LOCOROCO MIDNIGHT CARNIVAL or APE QUEST STARTER PACK)

note2: bubbles created using the hacked vita method will still *work* on any unhacked vita, 
using the same PSN Account; however it requires a hacked vita to *obtain* some of the files, 
that are required for this method;

the main advantage to doing it this way is you can use any psp license to create both ps1 and psp bubbles;

you will need: 
- Your ConsoleID/IDPS, Yoti has a tool to dump this availible [here](https://github.com/Yoti/psv_idpsdump/releases/)
- Your Consoles activation data file (located at tm0:/npdrm/act.dat)
- Any PSP/PS1 License file for your account (located at ux0:/pspemu/PSP/LICENSE/*.rif, or ux0:/bgdl/t/XXXXXX/temp.dat if you have a pending download)

YOUTUBERS: if you are planning on making a youtube tutorial on this, please note that your consoles IDPS is
also used to identify your console on the playstation network,
and sharing it would allow anyone to impersonate your console on the PSN!,
do not just blindly give this out to people.
(this would not give them access to your PSN Account however)

Open the CHOVY-SIGN2 application, under PSP click GET KEYS
put in your IDPS into the ConsoleID/IDPS field; in hex (if you used yotis tool, its in ux0:/data/idps.txt) 
browse to your act.dat file, and rif file, and click Generate.
this will populate the key and rif field; 
now do the same thing for the PS1 Option, using the same license and activation file as before.


a diagram explaining the 3 key obtaining methods is below:
![image](https://user-images.githubusercontent.com/39113159/100169414-55d2ae80-2f28-11eb-834b-5206388d20cd.png)

-- 


Credits:    
SquallATF		(for "PspCrypto" and "PBPResigner", and making PS1 Game signing possible,
				And discovering a bug in \_\_sce_ebootpbp handling that makes it possible to use multi-disc games.)

Li:             (for writing the original chovy-sign, 
				Developing the GUI, finding the original psp bubbles method and
				
                [Sfo.NET](https://github.com/KuromeSan/Sfo.NET/blob/master/README.md) A Simple SFO Parser.             
				Writing the PS1 Disc Compresison algorithm, making it possible to use custom ISOs
				Writing C# Implementation of PSVIMGTOOLS..
				
				Being transgender)

				
dots-tb			(for [chovy-gen](https://github.com/dots-tb/chovy-gen) (\_\_sce_ebootpbp signing)         


Sony Computer Enterainment: (For at3tool)

yifanlu & xyz for the original [psvimgtools](https://github.com/yifanlu/psvimgtools). 

Mathieulh (Found psp signing keys?)            

Motoharu (For helping dots with \_\_sce_ebootpbp)                 

Davee (For finding the PS1 Signing Key)

xlenore (For [PS1 Cover Art](https://github.com/xlenore/psx-covers))              

RupertAvery (For their fork of DiscUtils to add PS1 Support)  


SquallATF's PBPResigner and PSPCrypto were derived from :
RupertAvery (For [PSXPackager](https://github.com/RupertAvery/PSXPackager) and his fork of DiscUtils)                  
swarzesherz (For [sign_np](https://github.com/swarzesherz/sign_np))             
tpunix (For [kirk_engine](https://github.com/tpunix/kirk_engine))             
	