@echo off
@echo on
< savegame.sav (
    set /p whitecatname=
    set /p blackcatname=
    set /p savedcheckpoint=
    set /p weapon=
    set /p coins=
)
@echo off
cls

echo. 
echo ######## ##     ## ########     #######  ##     ## ########  ######  ########     #######  ########       
echo    ##    ##     ## ##          ##     ## ##     ## ##       ##    ##    ##       ##     ## ##             
echo    ##    ##     ## ##          ##     ## ##     ## ##       ##          ##       ##     ## ##             
echo    ##    ######### ######      ##     ## ##     ## ######    ######     ##       ##     ## ######         
echo    ##    ##     ## ##          ##  ## ## ##     ## ##             ##    ##       ##     ## ##             
echo    ##    ##     ## ##          ##    ##  ##     ## ##       ##    ##    ##       ##     ## ##             
echo    ##    ##     ## ########     ##### ##  #######  ########  ######     ##        #######  ##    
echo.
echo.         
echo ######## ##     ## ########    ##      ## ##     ## #### ######## ########     ######     ###    ######## 
echo    ##    ##     ## ##          ##  ##  ## ##     ##  ##     ##    ##          ##    ##   ## ##      ##    
echo    ##    ##     ## ##          ##  ##  ## ##     ##  ##     ##    ##          ##        ##   ##     ##    
echo    ##    ######### ######      ##  ##  ## #########  ##     ##    ######      ##       ##     ##    ##    
echo    ##    ##     ## ##          ##  ##  ## ##     ##  ##     ##    ##          ##       #########    ##    
echo    ##    ##     ## ##          ##  ##  ## ##     ##  ##     ##    ##          ##    ## ##     ##    ##    
echo    ##    ##     ## ########     ###  ###  ##     ## ####    ##    ########     ######  ##     ##    ##    
echo.
echo WELCOME BACK %whitecatname%! PRESS ENTER TO CONTINUE (You have %coins% coins)
echo ...
pause>nul

if %savedcheckpoint%==0 goto prologue
if %savedcheckpoint%==1 goto meowberne
if %savedcheckpoint%==2 goto darkforest
if %savedcheckpoint%==3 goto thedunes
if %savedcheckpoint%==4 goto checkpoint4
if %savedcheckpoint%==5 goto checkpoint5
if %savedcheckpoint%==6 goto checkpoint6

:prologue
cls
:: https://patorjk.com/software/taag/#p=display&f=Banner3&t=Chapter%202%3A%0ADark%20forest
echo.
echo ########  ########   #######  ##        #######   ######   ##     ## ######## 
echo ##     ## ##     ## ##     ## ##       ##     ## ##    ##  ##     ## ##       
echo ##     ## ##     ## ##     ## ##       ##     ## ##        ##     ## ##       
echo ########  ########  ##     ## ##       ##     ## ##   #### ##     ## ######   
echo ##        ##   ##   ##     ## ##       ##     ## ##    ##  ##     ## ##       
echo ##        ##    ##  ##     ## ##       ##     ## ##    ##  ##     ## ##       
echo ##        ##     ##  #######  ########  #######   ######    #######  ########
echo.
echo #############################################################################
echo ...
pause>nul
echo.
echo Once upon a time, there was a land where cats lived. There were cats of all colours, including a single
echo white cat and a single black cat. These two cats had been in love for a long time. They met just 2 days
echo before christmas, it was quite magical. The two cats had a nice house in the center of Meowberne, on the
echo west coast of Maustralia. Nothing could stand in the way of their love and happiness...
echo.
echo ...until, one day, an evil gang took the black cat into its hideout.
echo.
echo ...
pause>nul
echo.
echo The white cat was desperate and furious, as she couldn't do anything about it, but she knew she had to do
echo something. She decided to go on a quest to rescue him heroically, but she mustn't let her feelings to 
echo control her. The problem was, however, she didn't know anything about this gang. In reality, only
echo a selected few knew its name, even less cats knew about its customs and only a single cat knew where they
echo were hiding. The white cat knew the quest would be hard, but the black cat would do the same for her.
echo.
echo ...
pause>nul
echo.
echo So, our heroic white cat named...
PING -n 5 127.0.0.1>nul
echo.
echo Ehm... I must have forgotten...
PING -n 3 127.0.0.1>nul
echo.
echo Could you remind me please?
echo.
SET /p whitecatname=YOU: My name is 
echo.
echo Oh yeah right, right, %whitecatname%, how could I have not remembered, of course! ...Anyway, so
echo our heroic cat named %whitecatname%, went downstairs to pick up some gear for her journey.
echo.
echo END OF PROLOGUE. PRESS ENTER TO SAVE YOUR PROGRESS
echo ...
pause>nul
cls
SET savedcheckpoint=1
SET blackcatname=BlackCatName
SET weapon=none
SET coins=0
echo ##############################################
@echo on
(
    echo %whitecatname%
    echo %blackcatname%
    echo %savedcheckpoint%
    echo %weapon%
    echo %coins%
) > savegame.sav
@echo off
echo ##############################################
echo GAME HAS BEEN SAVED
echo.
echo ...
pause>nul

:meowberne
cls
:: https://patorjk.com/software/taag/#p=display&f=Banner3&t=Chapter%202%3A%0ADark%20forest
echo.
echo  ######  ##     ##    ###    ########  ######## ######## ########              ##  
echo ##    ## ##     ##   ## ##   ##     ##    ##    ##       ##     ##           ####
echo ##       ##     ##  ##   ##  ##     ##    ##    ##       ##     ##             ##    #  
echo ##       ######### ##     ## ########     ##    ######   ########              ##        
echo ##       ##     ## ######### ##           ##    ##       ##   ##               ##    # 
echo ##    ## ##     ## ##     ## ##           ##    ##       ##    ##              ##
echo  ######  ##     ## ##     ## ##           ##    ######## ##     ##           ######
echo.
echo.
echo ##     ## ########  #######  ##      ## ########  ######## ########  ##    ## ########   
echo ###   ### ##       ##     ## ##  ##  ## ##     ## ##       ##     ## ###   ## ##         
echo #### #### ##       ##     ## ##  ##  ## ##     ## ##       ##     ## ####  ## ##         
echo ## ### ## ######   ##     ## ##  ##  ## ########  ######   ########  ## ## ## ######     
echo ##     ## ##       ##     ## ##  ##  ## ##     ## ##       ##   ##   ##  #### ##         
echo ##     ## ##       ##     ## ##  ##  ## ##     ## ##       ##    ##  ##   ### ##         
echo ##     ## ########  #######   ###  ###  ########  ######## ##     ## ##    ## ########
echo.
echo ######################################################################################
echo.
echo ...
pause>nul
echo.
echo You went downstairs to pick up some gear. You aren't much of a fighter, so all this gear belonged to the
echo black cat. %whitecatname% looked at the weapon rack. There was one sword, one axe and a crossbow, sadly
echo with no ammo.
echo ...
pause>nul
start WeaponRack.bat
echo.
echo %whitecatname%: Hmm.. Okay, I'll have to choose a weapon if I want to rescue my love. Which weapon
echo        should I choose though? Crossbow is not an option, as I don't have any arrows and no money
echo        to buy more.
echo.
SET /p weapon=%whitecatname%: I think I'll take the 
echo.
echo ...
pause>nul
echo.
echo You take the %weapon% off the weapon rack and look at it with fear in your eyes.
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: I hope I won't have to use it. Ahh.. so, I'll surely need some armour too.
echo.
echo ...
pause>nul
echo.
echo You approach the armour stand. His armour is there, but something's missing. The helmet is not
echo there. There is only the chestpiece, leggings and boots, albeit in a good condition. Funnily enough,
echo because this is a game, the armour fits you perfectly, so no worries about being clunky in it.
echo.
echo ...
pause>nul
echo.
echo You go upstairs again. As you are passing the mirror, you admire your bravery and beauty. You are looking
echo at yourself, standing tall before the mirror, %weapon% in hand and almost fully in shiny armour. You grab
echo some last things before going out into the city, looking for clues as to where your lovely black cat has
echo gone.
echo.
echo ...
pause>nul
echo.
echo You step out of your house, thinking where to go next. Should you go first to the market, as there is a
echo large number of cats who might know something or should you go first to the bar, as there is a high
echo probability you could find... I'm sorry...
echo.
PING -n 1 127.0.0.1>nul
echo What is the name of your lost loved one?
echo.
SET /p blackcatname=His name is 
echo.
echo Oh sorry, I remember now, %blackcatname% obviously. Anyhow, in the bar there is a high chance you will
echo find %blackcatname%'s friend, Imhail, who was with him the moment %blackcatname% has been kidnapped.
echo.
echo %whitecatname%: Ok, I'll have to make a decision here, do I go to the market, or to the bar first?
echo.
echo (market / bar)
SET /p marketorbar=
if /i %marketorbar%==market goto marketfirst
if /i %marketorbar%==bar goto barfirst

:marketfirst
set firstvisit=market
goto market

:barfirst
set firstvisit=bar
goto bar

:market
cls
color d
echo.
echo =========================================================================================================
echo.
echo (First visit: %firstvisit%. THIS WILL CHANGE SOME DIALOGS)
start Market.bat
echo.
echo You enter the market. It is bustling and full of life. Cats shout, money gets thrown around as it was
echo nothing, you really did enter at the busiest possible time of day. As you walk around, you notice a
echo small house among all the kiosks with the sign "Thunderball" on the side. The windows are shut and the
echo blinds are making it impossible to see inside. As you pass the door, they open and soon you find
echo yourself inside, held by a strong manly paw.
echo.
echo ...
pause>nul
echo.
echo Unknown cat: Pssst! Be quiet! They are everywhere, everyone sees them, yet only a few recognise them.
echo        That's what makes them so good at their job.
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: Who? What the hell are you talking about? *you try to break free, to no avail* Let me
echo        go! Get off me!
echo.
echo ...
pause>nul
echo.
echo The cat drags you away from the door and slowly lets go. You are now free, but you aren't experienced
echo enough to start fighting. You are prepared to defend yourself, but listen first to what he has to say.
echo.
echo ...
pause>nul
echo.
echo Guomo: Hello %whitecatname%, I'm Guomo. Sorry for what happened to %blackcatname%. See, I would be glad
echo        to help you, but you know, I sadly got my leg broken the other day and we need to act quite fast.
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: How do you know my name? Do you know %blackcatname%?
echo.
echo ...
pause>nul
echo.
echo Guomo: Yes, I have met %blackcatname% during one of the hunts we went on. He is a nice bloke, quite a
echo        witty one too.
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: Hmmm... he never told me that, but I guess it was irrelevant at the time. And, sorry to
echo        change the subject, but who were you talking about at the beginning?
echo.
echo ...
pause>nul
echo.
echo Guomo: Ah yes, sorry, got carried away. 'Twas a few summers back when I first heard of the Umonidu. They
echo        are a gang that practise some kind of Voodoo. You know, they have these dolls that they make from
echo        the skin of cats that cross their ways, or from cats they want. Some folks say that they can
echo        sense a powerful life force in cats and that they kidnap them so they could harness their power.
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: Do you think they captured %blackcatname% for his life force?
echo.
echo ...
pause>nul
echo.
echo Guomo: Yes, I am almost sure they did. I too learned to sense the life force in cats while I was in the
echo        special forces. When I was with %blackcatname%... it was... unlike anything I had sensed before...
echo        He really posesses a great gift he probably doesn't even know about.
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: Wow, I didn't even know something like that existed. Can you tell me more about it?
echo.
echo ...
pause>nul
echo.
echo Guomo: Sadly, no. I can't explain it. I just feel it. It would be like explaining vision to a blind cat.
echo        All I can tell you is that it is an attribute of a cat you can feel. It tells me how strongly
echo        a cat can experience emotions such as love or anger or some other emotion.
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: Whoah! Is there any way a cat can utilize this force?
echo.
echo ...
pause>nul
echo.
echo Guomo: Yes, but it requires rigorous training and takes a few years to master. If your point was to tell
echo        %blackcatname% to use it to free himself once you get to him, it wouldn't be possible I'm afraid.
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: Bummer...
echo.
echo ...
pause>nul

:guomoquestion
echo.
echo Guomo: Sooo... do you have anything else on your mind? A question about me? About the gang? A favour perhaps?
echo.
echo (you / gang / favour)
SET /p guomoanswer=I would like to ask about 
if %guomoanswer%==you goto guomoyou
if %guomoanswer%==gang goto guomogang
if %guomoanswer%==favour goto guomofavour

:guomoyou
echo.
echo %whitecatname%: Tell me about yourself
echo.
echo ...
pause>nul
echo.
echo Guomo: I was born 41 years ago in Meowberne, went to elementary school and after that I was training to
echo        be a fighter. After that, since my 20s I was in the royal army fighting for Maustralia. Nothing
echo        super exreme gladly though, war is a terrible TERRIBLE thing. I wish it would never happen again.
echo        Than I left the army due to my age 6 years ago, standard practise. I started going hunting where
echo        I met %blackcatname% there, we talked a bit, got to know each other. And now I am concerned for
echo        him so here I am helping you.
echo.
echo ...
pause>nul
echo.
goto guomoquestion

:guomogang
echo.
echo Guomo: I don't know much. I only am sure they call themselves the Umonidu and, as I have explained before,
echo        they will stop at nothing to get more life force out of their enemies or just cats that posess
echo        large quantities of it.
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: How did you learn about them?
echo.
echo ...
pause>nul
echo.
echo Guomo: I... can't tell you just yet.
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: Why not?
echo.
echo ...
pause>nul
echo.
echo Guomo: It is crucial for us both you don't know about Kilinko... Ah crap... Well, the three of us,
echo        Me, Kilinko and %blackcatname% were chatting a lot on hunts while no game was present. We actually
echo        all met there. First me and Kilinko and then %blackcatname% joined us. %blackcatname% doesn't know
echo        about Umonidu though, we were talking about it a bit before we met him. There is no chance in hell
echo        %blackcatname% crossed their paths because of Kilinko.
echo.
echo ...
pause>nul
echo.
if %firstvisit%==market goto questionaboutgangappearance
if %firstvisit%==bar goto guomoquestion

:questionaboutgangappearance
echo %whitecatname%: I see. And what does the gang look like?
echo.
echo ...
pause>nul
echo.
echo Guomo: As I have said when you entered this house, nobody that hasn't seen them in action knows. Your
echo        best chance is to hope you meet someone who saw it happen that night. Maybe %blackcatname% wasn't
echo        wasn't alone that night?
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: Yeah, he was accompanied by one of his closest friends who now has a 48 hour drinking
echo        streak. I'll look for him at the bar after I leave the market.
echo.
echo ...
pause>nul
echo.
echo Guomo: Very well.
goto guomoquestion

:guomofavour
echo.
echo %whitecatname%: I may need to be taught how to fight. You can probably tell I'm not very comfortable in
echo        this armour carrying around this %weapon%.
echo.
echo ...
pause>nul
echo.
echo Guomo: Yes, I can tell. I can teach you the basics and theory of combat, after that it just takes practise.
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: That will have to do for now. Tell me all I need to know.
echo.
echo ...
pause>nul
goto fightingtutorial

:fightingtutorial
echo.
echo Guomo: Ok, so the combat in these realms is easy to grasp. You need to focus on weakpoints. Let's say you
echo        know that a lizard has a squishy belly. When the console prompts you with a question about where you
echo        want to strike, type in the target and hope you know what you are doing.
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: What console?
echo.
echo ...
pause>nul
echo.
echo Guomo: It's a game, don't overthink it. Bystrik wasn't capable of coding anything better without pouring
echo        at least 5'000'000 hours into it. This is as good as it gets for a text based game written in
echo        the core language of Windows... Or he may be just lazy, who knows.
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: Ok... nevermind... But what if the enemy is wearing an armour?
echo.
echo ...
pause>nul
echo.
echo Guomo: Ah, yes. That... will happen eventually. You will also have to utilize your knowledge to target
echo        weakspots in the target's armour to break it. Once you break it, you need to strike the fleshy
echo        weakspot to kill the creature. If, however, the armour is of higher quality it won't break at
echo        first hit. Cracks will spread to a particular part and you will need to strike that if you
echo        want to break it completely.
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: Ok, but what if I need to block or dodge enemy's attack? How do I do that?
echo.
echo ...
pause>nul
echo.
echo Guomo: That is quite simple, as there are just 4 types of attacks. Fronthand, backhand, stab and heavy.
echo.
echo ...
pause>nul
echo.
echo Guomo: Fronthand goes from the side of the attacking hand, so if the attacker is holding the weapon in
echo        their right hand, the attack will go from the right. You can dodge this by using the movement
echo        [DUCK], just as they do in boxing while dodging hooks.
echo.
echo ...
pause>nul
echo.
echo Guomo: Backhand is more difficult, but not impossible. It goes from the opposite side relative to
echo        attacker's used hand. So, if an enemy backends you with his right arm, the attack goes from the
echo        left. You must use the [JUMP] move to escape damage.
echo.
echo ...
pause>nul
echo.
echo Guomo: Stab is the easiest to dodge, as it goes directly into you. All you have to do, is [DASH] out of
echo        the way.
echo.
echo ...
pause>nul
echo.
echo Guomo: And finally, the heavy attacks. These are the real pain in the arse, as they are performed in a
echo        manner that can't be dodged with your skills. You will have to [BLOCK] the attacks and minimize
echo        the damage they inflict. No worries though, most creatures don't have the ability to heavy attack.
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: And what if I miss my strike or dodge the wrong way?
echo.
echo ...
pause>nul
echo.
echo Guomo: You die instantly and horribly. You see, it is very VERY complicated to implement health system into
echo        this kind of games so... you just die at first mistake. That was easy to code.
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: I hope I'll understand what you are talking about one day...
echo.
echo ...
pause>nul
echo.
echo Guomo: Now let's test if you have been listening. You will now fight me! No worries though, you can always
echo        try again and I will not really hurt you, I'll just say "You would have been killed".
echo.
echo ...
pause>nul
echo.
echo WARNING! SHOULD YOU FIGHT GUOMO NOW, THE STORY WILL PROGRESS FURTHER
echo (now / later)
set "/p shouldifight=%whitecatname%: I will fight you "
if "%shouldifight%"=="now" (goto :fightwithguomo)
if "%shouldifight%"=="later" (goto :guomoquestion)

:fightwithguomo
color d
cls
echo.
echo Guomo: Okay. I am wearing an armour with a weakspot on my left shoulder. I also have a weakspot on my neck
echo        which you can try to hit after you get my armour off. I know all types of attacks, so you will have
echo        a chance to try dodge allof them. Let's go!
echo.
echo ...
pause>nul
echo.
color c
echo You and Guomo stand face to face. He is holding a sword in his right hand. You are frightened, so Guomo
echo decides to attack first.
echo.
echo ...
pause>nul
echo.
echo Guomo attacks with a fronthand attack.
echo.
echo (duck / jump / dash / block)
set /p "combataction=Perform a "
if /i "%combataction%"=="duck" (goto :fightwithguomoone) else (goto :deathbyguomo)
echo.

:fightwithguomoone
echo.
echo You ducked under Guomo's sword. Now it is your time to attack. Choose a target to strike.
echo.
echo (head / neck / torso / leftshoulder / rightshoulder / lefthand / righthand / leftleg / rightleg)
set /p "combataction=Aim for the "
if /i "%combataction%"=="leftshoulder" (goto :fightwithguomotwo) else (goto :deathbyguomo)

:fightwithguomotwo
echo.
echo You hit Guomo's shoulder armour and it cracks, with damage spreading to his torso. He stumbles, his broken
echo leg clearly hurts. He now does a backhand attack.
echo.
echo (duck / jump / dash / block)
set /p "combataction=Perform a "
if /i "%combataction%"=="jump" (goto :fightwithguomothree) else (goto :deathbyguomo)
echo.

:fightwithguomothree
echo.
echo You jump like a scared cat, Guomo's sword passing under your legs. You look at your %weapon% and prepare
echo a strike. Where to?
echo.
echo (head / neck / torso / leftshoulder / rightshoulder / lefthand / righthand / leftleg / rightleg)
set /p "combataction=Aim for the "
if /i "%combataction%"=="torso" (goto :fightwithguomofour) else (goto :deathbyguomo)

:fightwithguomofour
echo.
echo Guomo's armour breaks completely and falls onto the floor. He is now only in his underclothes. As you heard
echo the ding of the armour touching the floor, Guomo attacks with a stab.
echo.
echo (duck / jump / dash / block)
set /p "combataction=Perform a "
if /i "%combataction%"=="dash" (goto :fightwithguomofive) else (goto :deathbyguomo)
echo.

:fightwithguomofive
echo.
echo You dash to the left, clearly seeing his neck exposed for your strike. Choose your target.
echo.
echo (head / neck / torso / leftshoulder / rightshoulder / lefthand / righthand / leftleg / rightleg)
set /p "combataction=Aim for the "
if /i "%combataction%"=="neck" (goto :fightwithguomosix) else (goto :deathbyguomo)

:fightwithguomosix
echo.
echo You swing your %weapon% hard, aiming for the neck, but Guomo dashes away.
echo.
echo ...
pause>nul
echo.
echo Guomo: Whoah! you could have killed me! Careful with that %weapon% of yours! We are just training!
echo.
echo ...
pause>nul
echo.
echo Guomo is now angry. He shows you what military training teaches you. He grabs his sword with both hands
echo and performs a heavy attack.
echo.
echo (duck / jump / dash / block)
set /p "combataction=Perform a "
if /i "%combataction%"=="block" (goto :fightwithguomoseven) else (goto :deathbyguomo)
echo.

:fightwithguomoseven
echo.
echo You block his attack with your hand, %blackcatname%'s armour stopping his sword. Let's show him you can be
echo careful and precise and only pretend to finish him.
echo.
echo (head / neck / torso / leftshoulder / rightshoulder / lefthand / righthand / leftleg / rightleg)
set /p "combataction=Aim for the "
if /i "%combataction%"=="neck" (goto :fightwithguomoeight) else (goto :deathbyguomo)

:fightwithguomoeight
echo.
echo You swing your %weapon% carefully and in a controlled manner. You stop just before his throat, which is
echo covered by his hand just to be sure.
echo.
echo ...
pause>nul
echo.
echo Guomo: Well done, I would have died now.
echo.
echo ...
pause>nul
color d
echo.
echo Your body loosens up. Your breath slows down. It's over now. Well done.
echo.
echo ...
pause>nul
echo.
echo Guomo: Most fights aren't as intense as this one, I just wanted to make sure you knew everything you
echo        you needed. You handled it really well though, even with some mistakes present.
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: Thank you, Guomo. I truly appreciate your help.
echo.
echo ...
pause>nul
echo.
echo Your sight gets drawn to the clock on the wall. It's time to leave if you want to save %blackcatname%.
echo.
echo ...
pause>nul
if %firstvisit%==market goto frommarkettobar
if %firstvisit%==bar goto chapteroneending

:deathbyguomo
echo.
echo Guomo: You would have died now. Let's try again.
pause>nul
echo.
goto fightwithguomo

:frommarkettobar
echo.
echo %whitecatname%: Well, it's about time I went to the bar. Thanks for everyting Guomo.
echo.
echo ...
pause>nul
echo.
echo Guomo: It's been a pleasure meeting you
echo.
echo ...
pause>nul
echo.
echo You pack your things, bid farewell to Guomo and head for the bar
echo.
echo ...
pause>nul
echo.
goto bar

:bar
cls
color 8
echo.
echo =========================================================================================================
echo.
echo (First visit: %firstvisit%. THIS WILL CHANGE SOME DIALOGS)
start Bar.bat
echo.
echo You enter the bar, drunkards sitting on high barstools drinking mostly beer and some are eating a food
echo of some sort, if it can be called food. Almost immediately after you enter, you hear a friendly, but
echo somewhat stereotypical "Welcome! Please, have a seat!".
echo.
echo ...
pause>nul
echo.
echo You look at the barman. Should you sit down randomly next to some drunkards? Or should you call %blackcatname%'s
echo friend's name?
echo.
echo (sit / shout)
set /p sitorshout=
if %sitorshout%==sit goto barsit
if %sitorshout%==shout goto barshout

:barsit
echo.
echo You sat down next to the most sober cat you could find.
echo.
echo ...
pause>nul
echo.
echo Sober cat: Hey there kitten. Did you know that dogs can be killed with a single blow to their head?
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: What?
echo.
echo ...
pause>nul
echo.
echo Sober cat: Just sayin' when you get into trouble with dogs, aim for the heads.
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: Thanks, that may be useful. Listen, you seem to know your way here, I'm looking for Dumkar,
echo        do you maybe know if he's here?
echo.
echo ...
pause>nul
echo.
echo Sober cat: Yes, you are in luck, he has arrived a few minutes prior. He probably isn't that drunk... yet.
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: Thanks, I need to ask him something, better go before he becomes unmanageable.
echo.
echo ...
pause>nul
echo.
echo Sober cat: Farewell my kitten.
echo.
echo ...
pause>nul
goto dumkar

:barshout
echo.
echo You call out %blackcatname%'s friend and soon after, you hear a drunk "Yeeeees..?"
echo.
echo ...
pause>nul
echo.
echo You approach the voice.
echo.
echo ...
pause>nul
goto dumkar

:dumkar
echo.
echo %whitecatname%: Dumkar! Found you at last! I need your help, please tell me you didn't have too many beers.
echo.
echo ...
pause>nul
echo.
echo Dumkar: Whaaat?! Of cou.. course I di.. didn't..! Do you t-h-i-n-k I'm some ki.. kind of a guz... g-u-z-z-l-e-r?
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: Oh Creator... give me strength...
echo.
echo ...
pause>nul
echo.
echo Dumkar: So.. w-h-a-d-d-y-a wanna kn... know?
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: I seriously need to know what happened the night %blackcatname% has gone missing. Tell. Me.
echo        Everything. You. Remember. Please.
echo.
echo ...
pause>nul
echo.
echo Dumkar: Nooooo.. noo... Dumkar doe... doesn't remember... Dumkar doesn't w-a-n-n-a!
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: Come on Dumkar! Just tell me, I want nothing more. I know it must have been depressing,
echo        I need your help. %blackcatname% needs your help.
echo.
echo ...
pause>nul
echo.
echo Dumkar: No... it's ju... just too t-e-r-r-i-b-l-e even to spe... speak about.
echo.
echo ...
pause>nul
echo.
echo You seriously think of using mild force to getting him to tell you what happened.
echo.
echo (violence / diplomacy)
set /p violenceorpeace=
if %violenceorpeace%==violence goto dumkarviolence
if %violenceorpeace%==diplomacy goto dumkardiplomacy

:dumkardiplomacy
echo.
echo %whitecatname%: Listen, without you %blackcatname% won't survive and there will be nothing we could do.
echo        Please, man up and tell me all you know. Prove to me you are not just a depressed drunken cat.
echo.
echo ...
pause>nul
goto dumkarreal

:dumkarviolence
echo.
echo You slap Dumkar quite hard.
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: Tell me now or I'll do it again!
echo.
echo ...
pause>nul
goto dumkarreal

:dumkarreal
echo.
echo Dumkar: Ok, I ca... can see I h-a-v-e no oth... other choice. Co... come with m-e.
echo.
echo ...
pause>nul
echo.
echo Dumkar takes you outside, into a dark alley where no other cats can be seen or heard.
echo.
echo ...
pause>nul
echo.
echo Dumkar: You see, I was just bluffing. I'm not actually drunk. I'm just ordering beers I end up giving to
echo        others and pretend to be drunk because I fear the gang may get me too because I know too much.
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: Tell me everything that happened that night.
echo.
echo ...
pause>nul
echo.
echo Dumkar: We were just walking to see if our fish nets had caught anything, but then the cats in red robes
echo        jumped us and kidnapped %blackcatname%, throwing me on the ground very fiercely. After I stood up
echo        to defend %blackcatname%, they were gone. No traces, nothing. I know it's not much, but no cat
echo        knows what they actually do, so I had better play it safe until I gather more information.
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: By drinking?
echo.
echo ...
pause>nul
echo.
echo Dumkar: Nooo, don't be silly. I don't drink. I Listen. I listen for anything the local cats may know.
echo        And where do cats meet at this time of year? The bar. Sadly, I don't even know their name. I
echo        know nothing apart from what happened that horrible night.
echo.
echo ...
pause>nul
if %firstvisit%==market goto infofordumkar
if %firstvisit%==bar goto dumkarrealtwo

:infofordumkar
echo.
echo %whitecatname%: They call themselves the Umonidu. They are a gang that practise some kind of Voodoo. 
echo        You know, they have these dolls that they make from the skin of cats that cross their ways, or
echo        from cats they want. Some folks say that they can sense a powerful life force in cats and that
echo        they kidnap them so they could harness their power.
echo.
echo ...
pause>nul
echo.
echo Dumkar: How do you know that?
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: One guy I met at the market told me that. He used to go hunting with %blackcatname%.
echo.
echo ...
pause>nul
echo.
echo: Dumkar: Oooh... I see.
goto dumkarrealtwo

:dumkarrealtwo
echo.
echo %whitecatname%: Well, it's a pity we don't know more.
echo.
echo ...
pause>nul
echo.
echo Dumkar: Listen, to avoid being suspicious, I think we should go back into tha bar and "have some drinks".
echo        That way, if one of them sees us, they'll think we are just drinking. We should also eavesdrop on
echo        conversations, just in case we hear something interesting.
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: Good idea. Let's do it.
echo.
echo ...
pause>nul
echo.
echo You enter the bar again through the backdoor. You decided to pretend to to have falen out with each other
echo so that you can listen to different conversations to gather as much data as possible.
echo.
echo ...
pause>nul

:bartablechoice
echo.
echo There are three different tables you can possibly eavesdrop. At the first table sit 2 cats who seem to do
echo manual labour for a living. At the second table sits a lonely cat who is talking to himself. At the third
echo table sit three young cats that talk about some frightening event they experienced. If you don't feel like
echo eavesdropping anymore, you can always leave by typing in exit.
echo.
echo (1 / 2 / 3 / exit)
set /p tablechoice=I am first going to eavesdrop on table number 
if %tablechoice%==1 goto tablenumberone
if %tablechoice%==2 goto tablenumbertwo
if %tablechoice%==3 goto tablenumberthree
if %tablechoice%==exit goto barexit

:tablenumberone
echo.
echo Ginger cat: ...so I told him to fuck off after that. He was really annoying.
echo.
echo ...
pause>nul
echo.
echo Striped cat: Yeah, well done. I would have done the same.
echo.
echo ...
pause>nul
echo.
echo Ginger cat: I feel a bit bad for him every time I am rude to that damn cat but then I slap myself and all
echo        is well again.
echo.
echo ...
pause>nul
echo.
echo Striped cat: You shouldn't feel bat even a bit, that catfucker deserves every decibel of it. He doesn't do
echo        his job properly, so he can't expect to be treated well after that. Anyway, how's your mother?
echo.
echo ...
pause>nul
echo.
echo Ginger cat: The usual, she probably drinks herself to sleep every night. It's a shame. One day she just
echo        went crazy and the only thing that keeps her safe is actually alcohol. It prevents her from being
echo        able to hurt herself or anyaone else.
echo.
echo ...
pause>nul
echo.
echo Striped cat: How did you make her drink so much alcohol anyway? She was always against it, how come she now
echo        drinks it more than pure water?
echo.
echo ...
pause>nul
echo.
echo Ginger cat: That was actually quite smart. She only drinks from her own waterbottles that I used to fill
echo        with the best water from the best well in Meowberne. Now I just fill it with the cheapest Vodka I
echo        find in LIDL. Has to be high qual... ehm.. ehm.. percentage alcohol.
echo.
echo ...
pause>nul
echo.
echo Striped cat: That shit is crazy man, I wonder what she...
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: Hmmm... this doesn't seem to be leading to anything useful. I should go somwhere else.
goto bartablechoice

:tablenumbertwo
echo.
echo Lonely cat: I was always there for her and she left me... Such a whore... always goes for the ones with the
echo        biggest ears...
echo.
echo ...
pause>nul
echo.
echo Lonely cat: Why didn't she stay with me then? I have got HUUGE ears! What did she find wrong about them?
echo.
echo ...
pause>nul
echo.
echo Lonely cat: Ah... maybe this wasn't about the size of ears after all. Maybe this was about the size of
echo       something else...
echo.
echo ...
pause>nul
echo.
echo Lonely cat: The bank account obviously! That's what all cats want! Money! How could I have missed this?
echo.
echo ...
pause>nul
echo.
echo Lonely cat: Well... now that I think of it... I am not rich, but not poor too. I live a decent life, what
echo        was wrong then? WHAT IN THE UNIVERSE DO FEMALES WANT?!?!
echo.
echo ...
pause>nul
echo.
echo Lonely cat: I guess this will remain a mystery. They always say they want a nice gentlecat who cares about
echo        them, listens to them and massages them if they need to. But the cats they end up with are always
echo        the most degenerate streetcats who vape and drink daily, treat them like excrements and... and...
echo.
echo ...
pause>nul
echo.
echo The lonely cat lies on the table and starts crying. He doesn't seem to want to stop anytime soon.
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: I don't know if it's the place or the people that are more depressing. I should probably
echo        listen to someone else, this is pointless obviously.
echo.
echo ...
pause>nul
goto bartablechoice

:tablenumberthree
echo.
echo Youngest cat: ...I was SHIVERING with fear!
echo.
echo ...
pause>nul
echo.
echo Middle cat: Yeah... me too... never seen anything like it.
echo.
echo ...
pause>nul
echo.
echo Oldest cat: Agreed. I thought I was going to shit myself, but I didn't gladly. At least not for the next
echo        5 minutes...
echo.
echo ...
pause>nul
echo.
echo Middle cat: You are joking... please tell me you are joking...
echo.
echo ...
pause>nul
echo.
echo Oldest cat: Of course. It took me more than just 5 minutes to shit myself. I ought to eat more fiber.
echo.
echo ...
pause>nul
echo.
echo Youngest cat: Damn... do you think they will be alright?
echo.
echo ...
pause>nul
echo.
echo Middle cat: Who exactly?
echo.
echo ...
pause>nul
echo.
echo Youngest cat: The cats that got kidnapped by those weird cats with hoods!
echo.
echo ...
pause>nul
echo.
echo Oldest cat: I've read part two but I'm not going to spoil it for you.
echo.
echo ...
pause>nul
echo.
echo Youngest cat: Yeah... I just can't wait for the next play! The actors are really skilled.
echo.
echo ...
pause>nul
echo.
echo Middle cat: Yep, you really think the fear is real when they fight each other.
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: Dang it! And I was thinking they have seen something that could help me. Should probably
echo        try some other table.
echo.
echo ...
pause>nul
goto bartablechoice

:barexit
echo.
echo You exit out of the bar and meet with Dumkar to exchange information.
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: So, Dumkar, did you hear anything? Because I didn't hear shit.
echo.
echo ...
pause>nul
echo.
echo Dumkar: I have heard something that may be useful, but sadly you'll need additional information to utilize
echo        this I think.
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: What is it?
echo.
echo ...
pause>nul
echo.
echo Dumkar: I heard two cats talking about a hermit in the dark woods just outside of Meowberne. He is told to
echo        know the answer to many even controversial questions, but he only answers one question per cat. I 
echo        doubt he knows everything, but it is our only chance I fear. The cats said he's got a hut near the
echo        Old Supurrior. Maybe look somewhere around there?
if %firstvisit%==market goto chapteroneending
if %firstvisit%==bar goto frombartomarket

:frombartomarket
echo.
echo %whitecatname%: Well, I don't know what to ask him. I don't even know the name of the gang.
echo.
echo ...
pause>nul
echo.
echo Dumkar: Unfortunately, I can't help you with that. I've told you all I know.
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: Yes, I really appreciate it. I guess it's time I went to search for answers elsewhere. Bye
echo        for now Dumkar.
echo.
echo ...
pause>nul
echo.
echo Dumkar: Bye and good luck %whitecatname%. Hope to see %blackcatname% and you soon. Take care.
echo.
echo ...
pause>nul
echo.
echo You wave your paw at Dumkar and head for the market.
goto market

:chapteroneending
echo.
echo %whitecatname%: It's about time I went try to save %blackcatname%. Farewell, my friend.
echo.
echo ...
pause>nul
echo.
echo You wave at each other and you walk away, fearing what lurks in the dark forest.
echo.
echo ...
pause>nul
echo.
cls
SET savedcheckpoint=2
echo ##############################################
@echo on
(
    echo %whitecatname%
    echo %blackcatname%
    echo %savedcheckpoint%
    echo %weapon%
    echo %coins%
) > savegame.sav
@echo off
echo ##############################################
echo GAME HAS BEEN SAVED
echo.
echo ...
pause>nul
goto darkforest

:darkforest
cls
:: https://patorjk.com/software/taag/#p=display&f=Banner3&t=Chapter%202%3A%0ADark%20forest
color 2
echo.
echo  ######  ##     ##    ###    ########  ######## ######## ########      #######     
echo ##    ## ##     ##   ## ##   ##     ##    ##    ##       ##     ##    ##     ##
echo ##       ##     ##  ##   ##  ##     ##    ##    ##       ##     ##           ##   #
echo ##       ######### ##     ## ########     ##    ######   ########      #######     
echo ##       ##     ## ######### ##           ##    ##       ##   ##      ##          #
echo ##    ## ##     ## ##     ## ##           ##    ##       ##    ##     ##          
echo  ######  ##     ## ##     ## ##           ##    ######## ##     ##    #########     
echo.
echo.
echo ########     ###    ########  ##    ##    ########  #######  ########  ########  ######  ######## 
echo ##     ##   ## ##   ##     ## ##   ##     ##       ##     ## ##     ## ##       ##    ##    ##    
echo ##     ##  ##   ##  ##     ## ##  ##      ##       ##     ## ##     ## ##       ##          ##    
echo ##     ## ##     ## ########  #####       ######   ##     ## ########  ######    ######     ##    
echo ##     ## ######### ##   ##   ##  ##      ##       ##     ## ##   ##   ##             ##    ##    
echo ##     ## ##     ## ##    ##  ##   ##     ##       ##     ## ##    ##  ##       ##    ##    ##    
echo ########  ##     ## ##     ## ##    ##    ##        #######  ##     ## ########  ######     ##    
echo.
echo ################################################################################################
echo.
echo ...
pause>nul
echo.
echo As you leave Meowberne and enter the Dark Forest, you can't shake off the fear that runs through your
echo veins. You are alone in a dangerous area with some %weapon% you can't even use properly. You travel on
echo foot, as it is the only way for you to travel right now. After a few hours of travel, you see a dog.
echo.
echo ...
pause>nul
echo.
echo Dog: Hello, lovely cat. What beings you to these parts of the world. Shouldn't you be somwhere in your
echo        cozy house in Meowberne? Or did you get lost? Hehe!
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: I am on a very important quest. I have to save my loved one from a secret sciety. You
echo        wouldn't understand, and I also don't want to tell you.
echo.
echo ...
pause>nul
echo.
echo Dog: Whoah! I've never seen such a cutie on a quest that sounds this important. Are you sure it isn't
echo        just some game you and your baby friends are playing?
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: Listen. Just let me pass. I don't have time nor the mood for this.
echo.
echo ...
pause>nul
echo.
echo Dog: What if I don't? Are you going to cuddle me to death? Look at this!
echo.
echo ...
pause>nul
echo.
echo The dog shows you his little dagger. It's almost comically small. Just as the brains of Bystrik's
echo classmates. Normally, it wouldn't do much damage, but this game having the combat system it has,
echo it will still kill you instantly somehow.
echo.
echo ...
pause>nul
echo.
echo You see two options now. You could either fight him and possibly get some loot, or try to threaten him so
echo he would start to fear you and move aside peacefully.
echo.
echo ...
pause>nul
echo.
echo (attack / threaten)
set /p attackorthreaten=I want to 
if /i %attackorthreaten%==attack goto fightwithdog
if /i %attackorthreaten%==threaten goto threatendog

:threatendog
echo.
echo You take out your %weapon% from its sheath.
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: You see this %weapon%? I may not looke like it, but I can handle it quite well. If you
echo        don't believe me, that's up to you but I don't guarantee you'll come out of this alive.
echo.
echo ...
pause>nul
echo.
echo Dog: Am I supposed to fear you? Are you trying to make me afraid? HA! Oh noooo! Help meeee! A small kitty
echo        is trying to harm meeee! Get lost before this gets ugly. Oh and by the way, it's goind to get ugly
echo        soon, so beat it and go away.
echo.
echo ...
pause>nul
goto fightwithdog

:fightwithdog
cls
color c
echo.
echo You grab your %weapon% very firmly and smack that bastard with the handle in the face.
echo.
echo ...
pause>nul
echo.
echo Dog: Oh, you shouldn't have done that!
echo.
echo ...
pause>nul
echo.
echo The dog is holding his dagger in his right hand. He does a pirouette and attacks from a backhand.
echo.
echo (duck / jump / dash / block)
set /p "combataction=Perform a "
if /i "%combataction%"=="jump" (goto :fightwithdogone) else (goto :deathbydog)

:fightwithdogone
echo.
echo You jump, dodging his tiny weapon. You look at him closely. No armour, just bare skin. This should be easy.
echo But where to strike?
echo.
echo (head / neck / torso / leftshoulder / rightshoulder / lefthand / righthand / leftleg / rightleg)
set /p "combataction=Aim for the "
if /i "%combataction%"=="head" (goto :fightwithdogtwo) else (goto :deathbydog)

:fightwithdogtwo
color 2
echo.
echo You hold your %weapon% above your head, using gravity to amplify it's power and chop the dogs head into
echo two. Well done, he's dead now.
echo.
echo ...
pause>nul
echo.
echo You see a bag lying on the ground, with something shiny in it.
echo.
echo ...
pause>nul
goto deepdarkforest

:deathbydog
echo.
echo You got killed by the first real enemy you faced... Sad... No comment... Let's try again, shall we?
echo.
echo ...
pause>nul
goto fightwithdog

:deepdarkforest
echo.
echo You pick up the bag, opening it slowly. There are 10 gold coins. You pause, studying the coins carefully.
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: I've never seen coins like this! I guess creatures outside of Meowberne don't use our
echo        money. I bet I could do something with it. Maybe there's a shop somwhere near?
echo.
echo ...
pause>nul
set /a coins=coins+10
echo.
echo You put the coins into your pocket and continue walking through the forest. You now have %coins% coins.
echo.
echo ...
pause>nul
echo.
echo As you walk throught the forest, you think about the way you will get %blackcatname% out. You think hard
echo but you can't think of anything. Well that's because there are multiple skilled fighters and you are alone
echo and with almost no experience in fighting. The anxiety grows larger with every step. You don't know what
echo you are doing, you don't know where you are going, you don't know how are you going to save %blackcatname%.
echo All you know is that you HAVE to do it, whatever the price may be.
echo.
echo ...
pause>nul
echo.
echo While you were deep in your thought, you have walked to a giant tree, totally different from all others.
echo While the majority of trees in The Dark Forest are healthy and have a lot of leaves on them, this one looks
echo sick, with no leaves, really old and occupying a lot of space. It just stands there like it rules all. It
echo somehow forces you to look only at it. You ignore your surroundings.
echo.
start DarkTree.bat
echo ...
pause>nul
echo.
echo As you walk closer to the tree, you can see some text that seems to be written in a different language
echo with a different alphabet to that used in Meowberne. It look ancient and very important.
echo.
echo ...
pause>nul
echo.
start NoteOnATree.txt
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: Well, this seems important. I should probably find a way how to translate it.
echo.
echo ...
pause>nul
echo.
echo You study the tree a bit more, realizing that even though it looks already dead, somehow it feels more
echo alive than the whole forest. Finally, you look away from the tree and see a small village nearby.
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: How could I have missed that?
echo.
echo ...
pause>nul
echo.
echo Confused, you make you way to the village. The locals don't seem to like visitors, as they run into their
echo houses and lock the doors. You couldn't make out any features, as they wear clothes that seem to double as
echo a camouflage for hunting. As you enter the village, you see that is a lot smaller than it seemed to be from
echo distance.
echo.
echo ...
pause>nul
echo.
echo There is a small overgrown stone fountain in the centre of the village, with only 5 houses that encompass
echo the fountain in the middle. The houses are all different, with clear purpose of each of them.
echo.
echo ...
pause>nul
echo.
echo The first house is a farmhouse, with a small plot behind it for growing crops. Sadly, is seems nothing has
echo been grown there for a long time now, as it was infested with invasive plants and clearly neglected. The
echo house itself is in good condition. It is a smaller house, suitable for a comfort for 2 adults.
echo.
echo ...
pause>nul
echo.
echo The second house is a workshop of a blacksmith. It is a big robust house made out of stone bricks. There is
echo a display for weapons on the front side of the house, however with no actual wepons in it. There is a lot of
echo dust on the display glass, meaning that it isn't a rare thing for the weapons to not be there.
echo.
echo ...
pause>nul
echo.
echo The third house looks like a mage's tower. There are some weird symbol inscribed into the stone walls, with
echo curious plants growing up the tower. It all seems weirdly purposeful, as if the plants had a mind of their
echo own. There is a weak light glowing in the upmost windows.
echo.
echo ...
pause>nul
echo.
echo The fourth house is near a mine entrance that hasn't been used for eons. Maybe the mine was blocked by
echo boulders or there has been a gas leak that made mining impossible? Close to the entrance is a house which
echo appears to be where the mine's overseer lives. You can see a figure through the curtains.
echo.
echo ...
pause>nul
echo.
echo The fifth resembles an old windmill. It feels weird, having a windmill in a forest where there is hardly
echo any airflow. Though it seems impossible, the blades of the mill show indisputable signs of being weathered
echo by wind, as the fabric is stretched out of its original frame, which wouldn't happen without some force
echo trying to push through.
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: This place feels wrong. There are just too many inconsistencies.
echo.
echo ...
pause>nul
echo.
echo You decide it would be best to ask the mage for help with the translation of the unknown letters you Found
echo earlier
echo.
echo ...
pause>nul
goto settingnonos

:settingnonos
set visitedfarmhouse=no
set visitedblacksmith=no
set visitedmill=no
set visitedmage=no
set visitedmine=no
set hasseeds=no
set hascrops=no
set hasrastalite=no
set hasmagicwind=no
set hasiron=no
set haskrivknife=no
goto villagehousechoice

:villagehousechoice
color 2
echo.
echo (farmhouse / blacksmith / mage / mine / mill)
set /p "wheretogo=I now want to go to the "
if /i "%wheretogo%"=="farmhouse" (goto :farmhouse)
if /i "%wheretogo%"=="blacksmith" (goto :blacksmith)
if /i "%wheretogo%"=="mage" (goto :mage)
if /i "%wheretogo%"=="mine" (goto :mine)
if /i "%wheretogo%"=="mill" (goto :mill)

:farmhouse
if "%visitedfarmhouse%"=="no" goto farmhousefirsttime
if "%visitedfarmhouse%"=="yes" goto farmhouseagain

:farmhousefirsttime
set visitedfarmhouse=yes
echo.
echo This place feels weird. How come everything has stopped and nobody tried to fix things? There is so much
echo to answer. It won't be as easy as you have thought.
echo.
echo ...
pause>nul
echo.
echo You knock at the door.
echo.
echo ...
pause>nul
echo.
echo Unknown creature: Famur needs silence! Famur wants peace of mind!
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: Yo chill. I just need a bit of your time. Who am I speaking with?
echo.
echo ...
pause>nul
echo.
echo Famur: Famur of course! There is no other entity in this house except for.. FAMUR!
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: Hello Famur, I'm %whitecatname%. I need to ask you why you stopped growing cro...
echo.
echo ...
pause>nul
echo.
echo Famur: Famur has a farm, yet Famur cannot grow ANYTHING! Famur is sad... Famur IS ANGRY!
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: Why can't you grow anything? Is there any way I can help?
echo.
echo ...
pause>nul
echo.
echo Famur: Famor has no seeds! Famur NEEDS SEEEEEEDS! OTHERWISE... Famur remains sad...
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: Listen, I will get the seeds for you. Where do I find them?
echo.
echo ...
pause>nul
echo.
echo Famur: Famur can tell you. Famur WILL tell you!
echo.
echo ...
pause>nul
echo.
echo Famur starts singing. You just stand there perplexed, but feel like you should listen carefully. It seems
echo very important. You want to write it down, but have nothing on you that you could use. You pay attantion.
echo.
echo ...
pause>nul
echo.
echo At the crossroads, left or right to start,
echo The right path leads to the bear's heart.
echo North or south, the branches sway,
echo Southward may lead you astray.
echo. 
echo East or west, the spirit calls,
echo West won't lead to the camp's walls.
echo Left or right, the whispers guide,
echo Left path leads where bears abide.
echo. 
echo Fork in the path, a choice to make,
echo Left will bring a daunting ache.
echo Brook's flow, a choice to make,
echo Northern path, the camp will take.
echo. 
echo Through the mist, the final test,
echo Left path fails, the right is best.
echo.
echo ...
pause>nul
echo.
echo Famur shows you a direction through in the forest. You set off to get the seeds.
echo.
echo ...
pause>nul
goto findingseeds

:messeduppath
echo.
echo You return to the village.
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: What? Again in the village? This is eerie I couldn't have come here I went the opposite way!
echo.
echo ...
pause>nul
echo.
echo You set off again to find the seeds.
echo.
echo ...
pause>nul
echo.
goto findingseeds

:findingseeds
echo.
echo As you walk, you encounter your first junction.
echo.
echo (left / right)
SET /p "directiontogo=%whitecatname%: I will go "
if /i "%directiontogo%"=="right" (goto :findingseeds1) else (goto :messeduppath)

:findingseeds1
echo.
echo As you walk, you encounter your second junction.
echo.
echo (north / south)
SET /p "directiontogo=%whitecatname%: I will go "
if /i "%directiontogo%"=="north" (goto :findingseeds2) else (goto :messeduppath)

:findingseeds2
echo.
echo As you walk, you encounter your third junction.
echo.
echo (east / west)
SET /p "directiontogo=%whitecatname%: I will go "
if /i "%directiontogo%"=="east" (goto :findingseeds3) else (goto :messeduppath)

:findingseeds3
echo.
echo As you walk, you encounter your fourth junction.
echo.
echo (left / right)
SET /p "directiontogo=%whitecatname%: I will go "
if /i "%directiontogo%"=="left" (goto :findingseeds4) else (goto :messeduppath)

:findingseeds4
echo.
echo As you walk, you encounter your fifth junction.
echo.
echo (left / right)
SET /p "directiontogo=%whitecatname%: I will go "
if /i "%directiontogo%"=="right" (goto :findingseeds5) else (goto :messeduppath)

:findingseeds5
echo.
echo As you walk, you encounter your sixth junction.
echo.
echo (north / south)
SET /p "directiontogo=%whitecatname%: I will go "
if /i "%directiontogo%"=="north" (goto :findingseeds6) else (goto :messeduppath)

:findingseeds6
echo.
echo As you walk, you encounter your final junction.
echo.
echo (left / right)
SET /p "directiontogo=%whitecatname%: I will go "
if /i "%directiontogo%"=="right" (goto :bearcamp) else (goto :messeduppath)

:bearcamp
echo.
echo You come to a camp full of bears. They look at you and immediately attack. You unsheath your %weapon% and
echo start fighting back
echo.
echo ...
pause>nul
color c
goto fightwithbears

:deathbybear
echo.
echo The bears have killed you. Honestly, one cat vs multiple bears would probably end like this :D but let's
echo try it again shall, we? You can do it!
echo.
echo ...
pause>nul
goto fightwithbears

:fightwithbears
cls
echo.
echo The first bear charges you with his sword, with his head conviently open for a strike.
echo.
echo (head / neck / torso / leftshoulder / rightshoulder / lefthand / righthand / leftleg / rightleg)
set /p "combataction=Aim for the "
if /i "%combataction%"=="head" (goto :fightwithbears1) else (goto :deathbybear)

:fightwithbears1
echo.
echo You kill the bear with a single hit as none of them are wearing armour. The bear is holding his axe in his
echo right hand. He attacks fronthand.
echo.
echo (duck / jump / dash / block)
set /p "combataction=Perform a "
if /i "%combataction%"=="duck" (goto :fightwithbears2) else (goto :deathbybear)

:fightwithbears2
echo.
echo You jump, dodging the bear's attack. As you prepare to strike him you notice another one charging with a
echo heavy attack.
echo.
echo (duck / jump / dash / block)
set /p "combataction=Perform a "
if /i "%combataction%"=="block" (goto :fightwithbears3) else (goto :deathbybear)

:fightwithbears3
echo.
echo You block the attack with your hand, the armour taking a hit. The bear's axe bounced a bit from your armour
echo and ended up stuck in a nearby tree. Your eyes fall upon his left hand trying to get it out.
echo.
echo (head / neck / torso / leftshoulder / rightshoulder / lefthand / righthand / leftleg / rightleg)
set /p "combataction=Aim for the "
if /i "%combataction%"=="lefthand" (goto :fightwithbears4) else (goto :deathbybear)

:fightwithbears4
echo.
echo You cut his arm off clean with your %weapon%. As his arm falls on the ground, followed by his dying body,
echo you can hear thumps behind you. You decide to use your size against him and make him fall.
echo.
echo (head / neck / torso / leftshoulder / rightshoulder / lefthand / righthand / leftleg / rightleg)
set /p "combataction=Aim for the "
if /i "%combataction%"=="rightleg" (goto :fightwithbears5) else (goto :deathbybear)
if /i "%combataction%"=="leftleg" (goto :fightwithbears5) else (goto :deathbybear)

:fightwithbears5
echo.
echo You cut off the bear's foot and he falls on a sharp stone head first, dying instantly. You turn your head
echo right and there is a bear prepared to stab you with his sword.
echo.
echo (duck / jump / dash / block)
set /p "combataction=Perform a "
if /i "%combataction%"=="dash" (goto :fightwithbears6) else (goto :deathbybear)

:fightwithbears6
echo.
echo You dash backwards, his arm fully extended now with the sword missing you by a few centimetres. As he
echo prepares for another stab, you decide it's time to be a true female and break his heart!
echo.
echo (head / neck / torso / leftshoulder / rightshoulder / lefthand / righthand / leftleg / rightleg)
set /p "combataction=Aim for the "
if /i "%combataction%"=="torso" (goto :fightwithbears7) else (goto :deathbybear)

:fightwithbears7
echo.
echo You feel the adrenaline kick in and go berserk for a second, bending backwards with your %weapon% behind
echo your back and throwing it right into the bear's heart. As he gets pushed back by the sheer force of your
echo throw, you see another one behind him. You run up the bear's body, pulling your weapon out without
echo stopping. You jump off the now dead bear and see an axe flying in your direction while mid-air.
echo.
echo (duck / jump / dash / block)
set /p "combataction=Perform a "
if /i "%combataction%"=="block" (goto :fightwithbears8) else (goto :deathbybear)

:fightwithbears8
echo.
echo As you fall, you extend your arms with your %weapon% in hands. Your movement force is sufficient to knock
echo the bear's axe out of his hands. He grabs a throwing knife with his left hand, you have to act quick!
echo.
echo (head / neck / torso / leftshoulder / rightshoulder / lefthand / righthand / leftleg / rightleg)
set /p "combataction=Aim for the "
if /i "%combataction%"=="lefthand" (goto :fightwithbears9) else (goto :deathbybear)
if /i "%combataction%"=="leftshoulder" (goto :fightwithbears9) else (goto :deathbybear)

:fightwithbears9
echo.
echo His arm falls off with the knife in it. You can feel his pain putting a smile on your face. Suddenly, you
echo get tossed against a tree. You hit it with your head and it hurts quite a lot. You can see a bear trying
echo to grab you, his arm aimed at your head, just like a fronthand.
echo.
echo (duck / jump / dash / block)
set /p "combataction=Perform a "
if /i "%combataction%"=="duck" (goto :fightwithbears10) else (goto :deathbybear)

:fightwithbears10
echo.
echo He misses and exposes his neck. You can see the fear in his eyes now. He wants to escape, but the fight
echo overwhelmes you.
echo.
echo (head / neck / torso / leftshoulder / rightshoulder / lefthand / righthand / leftleg / rightleg)
set /p "combataction=Aim for the "
if /i "%combataction%"=="neck" (goto :fightwithbears11) else (goto :deathbybear)

:fightwithbears11
echo.
echo You cut his head off. All other bears are now running away, but somehow you feel you just can't let them.
echo You can see an axe stuck in a nearby tree and you throw it at an escaping bear, splitting his skull in
echo half. You can hear another one running close to you but not in your direction. You spin with your %weapon%
echo and cut off his left leg. He falls to the ground and to be sure, you cut his head off. There is just one
echo bear now in the camp, unable to escape as he got caught in his own trap.
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: HEY PAL! I DON'T KNOW YOU AND I DON'T WANT TO EITHER. I JUST KNOW THAT YOU BLOODY IDIOTS
echo        SHOULDN'T ATTACK EVERYONE ON SIGHT, OR SOMETIMES THERE CAN BE A LITTLE CAT TO COME TURN YOUR CAMP
echo        UPSIDE DOWN!
echo.
echo ...
pause>nul
echo.
echo The Bear: Ok! Ok! We will be more careful in the future! I promise!
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: OH REALLY?! I'LL MAKE SURE YOU WON'T, AS I WILL MAKE SURE THERE IS NO FUTURE FOR YOU!
echo.
echo ...
pause>nul
echo.
echo As you finish the sentence, you slash the bear with your %weapon% and his whole body ends up split into
echo two halves. You calm down and realize what you've just done.
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: Dear Creator! What have I done? This has never happened to me before. I should probably
echo        meditate more. Well, let's see if I can find any seeds here so this wouldn't be a waste of blood.
echo.
echo ...
pause>nul
echo.
echo You search the camp and find a bag with glowing seeds.
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: These look magical enough for me! I'll take them back to the village.
echo.
echo ...
pause>nul
echo.
echo You return to the village.
echo.
echo ...
pause>nul
set hasseeds=yes
goto rightafterbearcamp

:farmhouseagain
if "%hascrops%"=="yes" (goto :farmdone) else (goto :farmhouseoncemore)

:farmhouseoncemore
if "%hasrastalite%"=="yes" (goto :growingcrops)
if "%hasrastalite%"=="no" (goto :rightafterbearcamp)

:rightafterbearcamp
color 2
echo.
echo You knock at the farmhouse door again.
echo.
echo ...
pause>nul
echo.
echo Famur: Yees?
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: I got some seeds. But listen, I have just realized. How on earth are you going to grow
echo        them fast enough? Doesn't it take several months or even years to grow?
echo.
echo ...
pause>nul
echo.
echo Famur: Normally, it would. But Famur knows a TRICK! Go to the mine for me and get me some Rastalite. It
echo        helps to speed up the process of growth.
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: Ok, fine, I will get it for you.
set knowsaboutrastalite=yes
goto villagehousechoice

:growingcrops
echo.
echo You return to the farm.
echo.
echo ...
pause>nul
echo.
echo Famur: Does %whitecatname% have Rastalite for Famur?
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: Yes, I do. Is there anything else or can you get me some crops now please?
echo.
echo ...
pause>nul
echo.
echo Famur: No, no, this is sufficient for Famur. You'll get the crops right away. Give Famur some time.
echo.
echo ...
pause>nul
echo.
echo After Famur finished his sentence, he waved his hand signaling you to follow him into his garden. He put
echo the seeds in the ground and some Rastalite onto the toil above them. In front of your eyes you see a very
echo rapidly growing plant, growing 10 centimetres per second. As the plant reaches its full height, another
echo one arises from the ground. It is magical. After around 5 minutes all crops cease growing and no more
echo appear from the soil.
echo.
echo ...
pause>nul
echo.
echo Famur: Famur is so ELATED! Famur hasn't grown ANYTHING in a very long time. Famus thanks %whitecatname% for
echo        the seeds and the Rastalite. Famur can finally grow crops again! Well... it seems that the farm
echo        needs some love. Leave me alone please, I will now prepare it for future harvest.
echo.
echo ...
pause>nul
set hascrops=yes
goto villagehousechoice

:farmdone
echo.
echo You knock at the door of the farm again.
echo.
echo ...
pause>nul
echo.
echo Famur: Famur is busy! Leave Famur ALONE!
echo.
echo ...
pause>nul
echo.
goto villagehousechoice

:blacksmith
if "%visitedblacksmith%"=="no" goto blacksmithfirsttime
if "%visitedblacksmith%"=="yes" goto blacksmithagain

:blacksmithfirsttime
set visitedblacksmith=yes
echo.
echo You knock at the door.
echo.
echo ...
pause>nul
echo.
echo (Probably) The Blacksmith: Who is disturbing me?!
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: Hello sir, I call myself %whitecatname% and I need a specific item made.
echo.
echo ...
pause>nul
echo.
echo (Probably) The Blacksmith: Well you're out of luck pal, I have no iron! The mines have stopped operating.
echo        You will have to go there and get me some if you want my help! And even then it's going to cost you!
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: sigh... ok... how much do you need for a Kriv Knive?
echo.
echo ...
pause>nul
echo.
echo (Probably) The Blacksmith: THE KRIV KNIFE? WHAT DOES A SNOWY CAT WANT WITH A RITUAL WEAPON?!
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: It's not for me you donut! I need help from the mage next door and he needs a Kriv Knife.
echo        That's it I swear. I don't even know what a Kriv Knife is!
echo.
echo ...
pause>nul
echo.
echo (Probably) The Blacksmith: Well... if you get me at least 10 kilograms of iron I may be able to make it
echo        for you. just make sure to not bring any less than 10 kilograms! In that case I wouldn't be able
echo        to make it of the desired quality.
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: Ok. Fair enough. I'll get to it.
echo.
echo ...
pause>nul
echo.
echo You move away from the house.
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: Oh boy, I see where this is going...
goto villagehousechoice

:blacksmithagain
if "%haskrivknife%"=="yes" (goto :blacksmithdone) else (goto :blacksmithoncemore)

:blacksmithoncemore
echo.
echo You knock at the door again.
echo.
echo ...
pause>nul
echo.
echo (Probably) The Blacksmith: What is it? Ah... it's you again. Do you have the iron I need?
echo.
echo ...
pause>nul
if "%hasiron%"=="yes" (goto :forgingkrivknife)
if "%hasiron%"=="no" (goto :leavingblacksmith)

:forgingkrivknife
echo.
echo You hand him the iron ore.
echo.
echo ...
pause>nul
echo.
echo (Probably) The Blacksmith: Very good little cat. Give me a minute and you'll have the knife in your paws
echo        safe and sound.
echo.
echo ...
pause>nul
echo.
echo He closes the door and you can hear loud bangs coming from the inside. After 3 minutes the door open again.
echo.
echo ...
pause>nul
echo.
echo (Now surely) The Blacksmith: Here you go little kitten. Be careful with it, as it can be dangerous.
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: I know how to handle a weapon. Look, I have my own %weapon%.
echo.
echo ...
pause>nul
echo.
echo (Now surely) The Blacksmith: That's cure. Well, about time I got to work.
echo.
echo ...
pause>nul
echo.
echo He closes the door without saying anything else.
echo.
echo ...
pause>nul
set haskrivknife=yes
goto villagehousechoice

:leavingblacksmith
echo.
echo %whitecatname%: No, not yet.
echo.
echo ...
pause>nul
echo.
echo (Probably) The Blacksmith: Well, I can't help ya until ye get it.
echo.
echo ...
pause>nul
echo.
echo He shuts the door before your nose.
echo.
echo ...
pause>nul
goto villagehousechoice

:mage
if "%visitedmage%"=="no" goto magefirsttime
if "%visitedmage%"=="yes" goto mageagain

:magefirsttime
set visitedmage=yes
echo.
echo You knock at the door.
echo.
echo ...
pause>nul
echo.
echo (Probably) The Mage: What? Who is it?
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: Hello. My name is %whitecatname% and I would like to ask for a little help.
echo.
echo ...
pause>nul
echo.
echo Krandon: Hello, %whitecatname%, I am Krandon. I know my way around magic and similar forces. What
echo        do you need?
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: I don't know if it is of any use to me, but I would like to translate the text on that
echo        big old tree there.
echo.
echo ...
pause>nul
echo.
echo Krandon: Ooooh, that may not be easy. Well... I do have the papers for translation but... they took me a
echo        long time to make. It wasn't easy to decrypt as I had to endure torture from the knowledge I came
echo        across while decrypting.
echo.
echo ...
pause>nul
echo.
echo Krandon: But... should you really want this information... I will provide it to you for a price.
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: Do you mean 10 coins I have conveniently found like 20 minutes earlier?
echo.
echo ...
pause>nul
echo.
echo Your face is making a "just kidding, but maybe?" expression.
echo.
echo ...
pause>nul
echo.
echo Krandon: Hah! Nooo, no no nooo... I need a Kriv Knife for one of my rituals. Get it for me and I will give
echo        you the translation papers.
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: Where the hell do I find that?
echo.
echo ...
pause>nul
echo.
echo Krandon: There's a blacksmith like 2 metres from here. He can make it.
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: Can't you go there yourself?
echo.
echo ...
pause>nul
echo.
echo Krandon: It is... not as easy as you think it is. You'll understand. Just get me the knife.
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: Ooook... Off I go!
echo.
echo ...
pause>nul
echo.
goto villagehousechoice

:mageagain
if "%haskrivknife%"=="yes" (goto :translation) else (goto :mageoncemore)

:mageoncemore
echo.
echo Krandon: Oh! It's %whitecatname%! Do you have the Kriv Knife?
echo.
echo ...
pause>nul
echo.
echo No but...
echo.
echo ...
pause>nul
if "%knowsaboutmagicwind%"=="yes" (goto :gettingmagicwind) else (goto :leavingmage)

:leavingmage
echo.
echo Krandon: Then get to it NOW! Don't disturb me until you have it.
echo.
echo ...
pause>nul
echo.
echo Krandon shuts the door angrily. You must have interrupted something important with something banal.
echo.
echo ...
pause>nul
goto villagehousechoice

:gettingmagicwind
echo.
echo %whitecatname%: I need some magic wind for the mill.
echo.
echo ...
pause>nul
echo.
echo Krandon: Oh, I see. Yes wait a moment please.
echo.
echo ...
pause>nul
echo.
echo Krandon closes the door and you can hear him doing something in his tower. It seems like he is searching
echo some wooden crates and other storage spaces. After exactly 4 minutes and 37 seconds, Krandon emerges and
echo hands you a leather bag.
echo.
echo ...
pause>nul
echo.
echo Krandon: Here. Open this when you want to unleash the magic wind. Point the bag opening in the direction
echo        you want the wind to flow.
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: Thank you Krandon! I will have your knife in no time.
echo.
echo ...
pause>nul
echo.
echo Krandon: Great mate. See you then.
echo.
echo ...
pause>nul
set hasmagicwind=yes
goto villagehousechoice

:mine
if "%visitedmine%"=="no" goto minefirsttime
if "%visitedmine%"=="yes" goto mineagain

:minefirsttime
set visitedmine=yes
echo.
echo You knock at the door of the house close to the mine entrance.
echo.
echo ...
pause>nul
echo.
echo The Miner: I'm not going into that hellhole again! Leave me alone Gerbuht!
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: Please, don't get angry. You see, I'm not Gerbuht. My name is %whitecatname%.
echo.
echo ...
pause>nul
echo.
echo The Miner: Oh, in that case, I can't help you with anything. But you can try to tell me what you need.
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: I need you to go back into that so called hellhole.
echo.
echo ...
pause>nul
echo.
echo The Miner: HAHAHAAA! Great joke. I can take it. You read the room well.
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: Is it iron that's mined in that "hellhole"?
echo.
echo ...
pause>nul
echo.
echo The Miner: Well, yes! What else?
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: I need you to go back to that so called hellhole.
echo.
echo ...
pause>nul
echo.
echo The Miner: Listen. There is only one thing that would get me into that mine again.
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: What would it be? Maybe I can get it somehow?
echo.
echo ...
pause>nul
echo.
echo The Miner: I would go down there if only I got another of those magic breads the local mill used to bake.
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: Say no more. I'm on it.
echo.
echo ...
pause>nul
echo.
echo The Miner: Good luck with that. They don't make it anymore for some reason, it may have some serious side
echo        effects.
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: Only one way to find out!
echo.
echo ...
pause>nul
echo.
echo You leave the mine area.
goto villagehousechoice

:mineagain
if "%hasiron%"=="yes" (goto :minedone) else (goto :mineagainagain)

:mineagainagain
if "%hasbread%"=="yes" (goto :mining) else (goto :mineoncemore)

:mining
echo.
echo You knock at the door once more.
echo.
echo ...
pause>nul
echo.
echo The Miner: Do you have the bread at last?
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: Yes. This time I do.
echo.
echo ...
pause>nul
echo.
echo The Miner: YES! GIVE IT TO ME!
echo.
echo ...
pause>nul
echo.
echo You have no opportunity to give him the bread, as he takes the bread violently and eats the whole loaf at
echo once. He then turns around and sprints into the mine. You stand there perplexed about what just happened.
echo You can hear his pickaxe hitting on rocks and soon enough he returns with something shiny in his hands.
echo.
echo ...
pause>nul
echo.
echo The Miner: Here you go! I got you the iron you wanted. Now excuse me I need to go mining before this bread
echo        loses its power inside of me! Adios amigo!
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: What was weird as heck. Well, no time to lose.
echo.
echo ...
pause>nul
set hasiron=yes

:mineoncemore
echo.
echo You knock at the door again.
echo.
echo ...
pause>nul
echo.
echo The Miner: Oi! You got the bread?
echo.
echo ...
pause>nul
echo.
if "%knowsaboutrastalite%"=="yes" (goto :gettingrastalite) else (goto :leavingmine)

:gettingrastalite
echo.
echo %whitecatname%: I require some Rastalite in order to grow the crops. I was told you should have some.
echo.
echo ...
pause>nul
echo.
echo The Miner: Oh yes, I do. Here, take it, I don't need it anymore. All Rastalite is used to speed up the
echo        growth of crops. I suspect you must have gotten your hands on some seeds. Very well.
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: I'll be on my way. I'll be back in a few moments with the bread hopefully.
set hasrastalite=yes
goto villagehousechoice

:leavingmine
echo.
echo %whitecatname%: No, not yet.
echo.
echo ...
pause>nul
echo.
echo The Miner: Then go get it!
echo.
echo ...
pause>nul
echo.
echo The Miner closes the door and leaves you there standing like a fool. You decide to go elsewhere.
goto villagehousechoice

:mill
if "%visitedmill%"=="no" goto millfirsttime
if "%visitedmill%"=="yes" goto millagain

:millfirsttime
set visitedmill=yes
echo.
echo You look at the mill, clearly not catching any wind and thus motionless. This one may be more difficult
echo may one initially think.
echo.
echo ...
pause>nul
echo.
echo You knock at the door.
echo.
echo ...
pause>nul
echo.
echo Mr Miller: I, Mr Miller, tell you to go away. We can't help with anything. We need help ourselves and we
echo        are no charity!
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: Hey, Mr Miller. Some refer to me as %whitecatname% and I may be able to help, provided that
echo        you will help me.
echo.
echo ...
pause>nul
echo.
echo Mr Miller: What do you ask for your services?
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: That one magical bread you used to make.
echo.
echo ...
pause>nul
echo.
echo Mr Miller: Well... that's the problem actually. We don't have any crops to mill in order to make it!
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: And where can I find the crops needed for this special bread?
echo.
echo ...
pause>nul
echo.
echo Mr Miller: There is a farm in our community that has the capacity of growing the neccessary crops, but
echo        they have stopped growing them for some reason. One day, we just didn't get any supplies and
echo        that was it. It's been some time since that happened.
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: Ok, I'll have a little chat with them.
echo.
echo ...
pause>nul
goto villagehousechoice

:millagain
if "%hasbread%"=="yes" (goto :milldone) else (goto :millonceagain)

:millonceagain
if "%hasmagicwind%"=="yes" (goto :actualmilling)
if "%hasmagicwind%"=="no" (goto :askingforcrops)

:askingforcrops
echo.
echo You knock at the door of the mill.
echo.
echo ...
pause>nul
echo.
echo Mr Miller: Ay. Got me the crops I need?
echo.
echo ...
pause>nul
if "%hascrops%"=="yes" (goto :millingcrops) else (goto :leavingmill)

:millingcrops
echo.
echo %whitecatname%: Yes, I do actually.
echo.
echo ...
pause>nul
echo.
echo Mr Miller: Very well, give them to me and we can start milling them and make some bread.
echo.
echo ...
pause>nul
echo.
echo You give Mr Miller the crops and he starts putting them into the mill, but nothing happens.
echo.
echo ...
pause>nul
echo.
echo Mr Miller: Darn! I need the magic wind! Could you get it for me?
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: Where do I get it?
echo.
echo ...
pause>nul
echo.
echo Mr Miller: The magician can provide you with magic wind. Just ask him for it and he will know it is for me.
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: Oh boy. Okay, wait here.
echo.
echo ...
pause>nul
echo.
echo Mr Miller: I'm not going to move kitty.
echo.
echo ...
pause>nul
set knowsaboutmagicwind=yes
goto villagehousechoice

:actualmilling
echo.
echo You return to the mill with the wind in paws.
echo.
echo ...
pause>nul
echo.
echo Mr Miller: That's awesome! Quick, release it! Make it spin baby!
echo.
echo ...
pause>nul
echo.
echo These creatures really are W.E.I.R.D.
echo.
echo ...
pause>nul
echo.
echo You shrug off their antics and release the wind into the mill's blades. They start to spin furiously fast
echo and you can't stop watching. This is unlike anything you have ever seen before. You keep staring at it for
echo a solid 15 minutes in disbelief when you are interrupted by Mr Miller.
echo.
echo ...
pause>nul
echo.
echo Mr Miller: The bread's DONEEE!
echo.
echo ...
pause>nul
echo.
echo Your eyes fall from the blades upon Mr Miller holding a perfectly looking loaf of bread.
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: That looks delicious!
echo.
echo ...
pause>nul
echo.
echo Mr Miller: It sure is! Give it to the miner. He'll do anything for it.
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: Thank you.
echo.
echo ...
pause>nul
echo.
echo Mr Miller: Yeah enjoy. I'll get to prepairing my bakery for a re-opening. So no distractions please!
set hasbread=yes
goto villagehousechoice

:leavingmill
echo.
echo %whitecatname%: I don't have them yet.
echo.
echo ...
pause>nul
echo.
echo Mr Miller: Then what are you doing here? Get to work!
echo.
echo ...
pause>nul
echo.
goto villagehousechoice

:milldone
echo.
echo You knock at the mills doors.
echo.
echo ...
pause>nul
echo.
echo Mr Miller: Go away please! I'm trying to work here!
echo.
echo ...
pause>nul
goto villagehousechoice

:translation
echo.
echo Krandon: I hope it's something important now. You have been disturbing me enough for today as it is.
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: I have the Kriv Knife you wanted.
echo.
echo ...
pause>nul
echo.
echo Krandon: Really? I didn't think you would be able to withstand this torture. Even Bystrik almost failed
echo        while he was making this part. Legends say it took him more than 3 hours to write the code for
echo        this village and 2 more to fix all the bugs!
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: You doubted me? I don't blame you. And why do you all keep saying stuff about some code and
echo        other shenanigans? I don't get it.
echo.
echo ...
pause>nul
echo.
echo Krandon: One day you will little cat. The day will come soon enough.
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: Okay, anyway. Give me the translation papers please!
echo.
echo ...
pause>nul
echo.
echo Krandon: You don't even want to know where it leads? You are just goind to open a tree without any clue
echo        about what is on the other side?
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: Well...
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: ...yes?
echo.
echo ...
pause>nul
echo.
echo Krandon: HAH! No worries kitty. I'll tell you before I give you the papers. I know what you seek. I know
echo        WHO you seek.
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: Are you talking about my little %blackcatname%?
echo.
echo ...
pause>nul
echo.
echo Krandon: I know that too. But now, you seek the hermit that lives in these woods, to give you an answer you
echo        desperately need to save said %blackcatname%.
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: Yes! That is right! I almost forgot while doing these errands for the village.
echo.
echo ...
pause>nul
echo.
echo Krandon: Don't worry. That tree will teleport you right to Old Supurrior. You will find his hut there.
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: Is it true that he knows almost everything?
echo.
echo ...
pause>nul
echo.
echo Krandon: It surely is. He is the best mind of all in this forest. He knows about every move we make here.
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: That's kinda creepy, isn't it?
echo.
echo ...
pause>nul
echo.
echo Krandon: Only if you think about it while bathing.
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: Brrrr... I... hope to not need to bath in this forest.
echo.
echo ...
pause>nul
echo.
echo Krandon: Hahaha! Just kidding. He is not magical. He can't see everything. He knows all his knowledge from
echo        other creatures that come to consult with him their problems. That's why he knows about a lot of
echo        controversial stuff. He just hears it a lot and remembers it well. But, enough of this. Here, take
echo        this note. It should help you translate what's on that three.
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: Didn't you ever wonder and translate it yourself? Why do I have to translate it?
echo.
echo ...
pause>nul
echo.
echo Krandon: It's because the tree shows something different to every creature that reads it. Translate the
echo        script and you shall understand.
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: Ok well, thank you a lot Krandon. You have helped me a lot.
echo.
echo ...
pause>nul
echo.
echo Krandon: You have helped me even more kitty. You don't even know how much good you have done today. It
echo        shall be remembered. Farewell, new friend.
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: Farewell, Krandon. Live well.
echo.
echo ...
pause>nul
echo.
echo You approach the tree with the paper Krandon gave you.
start NoteOnATree.txt
start TreeTranslation.txt
echo.
echo ...
pause>nul
goto actualtranslation

:actualtranslation
echo.
set /p "treetranslation=%whiteatname%: "
if /i %treetranslation%==shoorasl (goto :oldsupurrior) else (goto :translationnotgood)

:translationnotgood
echo.
echo Nothing happens
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: Hmmm... maybe I translated it wrong.
echo.
echo ...
pause>nul
goto actualtranslation

:oldsupurrior
echo.
echo The tree starts to glow and after a few seconds everything becomes white around you. You can't see anything
echo except you in your gear. Not even the ground. It's just you in some blank white space for 2 seconds and
echo then you appear near a hut close to the Old Supurrior lake.
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: I'm here. Finally. That took some time.
echo.
echo ...
pause>nul
echo.
echo You approach teh hut when suddenly, an old gray cat walks out.
echo.
echo ...
pause>nul
echo.
echo The cat: Welcome %whitecatname%! I've been waiting for you.
echo.
echo ...
pause>nul
echo.
echo You are a little bewildered at first but then you realize that this cat is no ordinary creature. You greet
echo them politely.
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: Hello mister. I've heard that you know things others have no idea about sometimes?
echo.
echo ...
pause>nul
echo.
echo The cat: Yes, that may be true. But there is a catch. You may ask only 1 question.
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: Yes, I have heard about it. Well so...
echo.
echo ...
pause>nul
echo.
echo The cat interrupts you.
echo.
echo ...
pause>nul
echo.
echo The cat: Why don't we discuss this in my hut? Oh any by the way, you can call me Hebumio
echo.
echo ...
pause>nul
echo.
echo You nod and enter the hermit's hut. He offers you some tea and you accept, being quite thirsty after all
echo that you had to endure up until this point. You discuss some light topics to know each other better,
echo although you feel like he knows you better than you know yourself and is doing this just for show. He then
echo tells you that he knows about %blackcatname%.
echo.
echo ...
pause>nul
echo.
echo Hebumio: I know what you seek. But this won't be easy. The Umonidu are a very dangerous gang. They steal
echo        the life forces out of cats that posess a lot of it. But they have captured %blackcatname% not only
echo        for his life force, but also for his blood. You see, he has a special blood that can resurrect the
echo        dead. The gang somehow discovered this and decided it would be best if they had it. Even though this
echo        seems like bad news, it is actually great, as they won't kill him for his life force yet, because
echo        they need a lot of his blood for their needs. When they have enough so their leader can keep making
echo        more by his magical abilities, they will however kill him so that no other creature can get their
echo        limbs onto it. They want it only for themselves.
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: That is horrible! I must stop them as soon as possible!
echo.
echo ...
pause>nul
echo.
echo Hebumio: You know what they look like and you know their name. I don't need to tell you that. But I can and
echo        will tell you that you must now head for the Great Dunes. You must kill Xramius, the great worm that
echo        has been terrorising those lands for decades. The local people will be grateful and pledge their allegiance to
echo        you because of that. They are skilled fighters and you will need them on your journey and especially
echo        in the end when you will fight the Umonidu themselves to rescue %blackcatname%. Your path will have
echo        more stops than just the dunes and the Unomidu hideout, but I sadly can't tell you more about it.
echo        I can tell you however that you can make it, you just need to believe in your abilities and
echo        determination.
echo.
echo ...
pause>nul
echo.
echo He then asks you abut your journey so far and you tell him everything that happened. You both laugh and have
echo a great time together. After 20-something minutes he starts to cut the conversation.
echo.
echo ...
pause>nul
echo.
echo Hebumio: It's about time you went on your quest %whitecatname%. Farewell my friend. Be sure to visit me with
echo        %blackcatname% sometimes when all will be sorted out.
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: We sure will if we survive both. I'm looking forward to it. Stay safe Hebumio. Farewell.
echo.
echo ...
pause>nul
echo.
echo Hebumio: Farewell %whitecatname%.
echo.
echo ...
pause>nul
echo.
echo After hearing that, Hebumio teleports you to...
echo.
echo ...
pause>nul
cls
SET savedcheckpoint=3
SET blackcatname=BlackCatName
SET weapon=none
SET coins=0
echo ##############################################
@echo on
(
    echo %whitecatname%
    echo %blackcatname%
    echo %savedcheckpoint%
    echo %weapon%
    echo %coins%
) > savegame.sav
@echo off
echo ##############################################
echo GAME HAS BEEN SAVED
echo.
echo ...
pause>nul
goto thedunes

:thedunes
cls
:: https://patorjk.com/software/taag/#p=display&f=Banner3&t=Chapter%203%3A%0AThe%20dunes
color e
echo.
echo  ######  ##     ##    ###    ########  ######## ######## ########      #######   ##  
echo ##    ## ##     ##   ## ##   ##     ##    ##    ##       ##     ##    ##     ## #### 
echo ##       ##     ##  ##   ##  ##     ##    ##    ##       ##     ##           ##  ##  
echo ##       ######### ##     ## ########     ##    ######   ########      #######       
echo ##       ##     ## ######### ##           ##    ##       ##   ##             ##  ##  
echo ##    ## ##     ## ##     ## ##           ##    ##       ##    ##     ##     ## #### 
echo  ######  ##     ## ##     ## ##           ##    ######## ##     ##     #######   ##  
echo.
echo.
echo ######## ##     ## ########    ########  ##     ## ##    ## ########  ######         
echo    ##    ##     ## ##          ##     ## ##     ## ###   ## ##       ##    ##        
echo    ##    ##     ## ##          ##     ## ##     ## ####  ## ##       ##              
echo    ##    ######### ######      ##     ## ##     ## ## ## ## ######    ######         
echo    ##    ##     ## ##          ##     ## ##     ## ##  #### ##             ##        
echo    ##    ##     ## ##          ##     ## ##     ## ##   ### ##       ##    ##        
echo    ##    ##     ## ########    ########   #######  ##    ## ########  ######         
echo.
echo ####################################################################################
echo.
echo ...
pause>nul
echo.
echo ...The Dunes! Well... you probably know that from reading the title... Anyway, you also feel a weird
echo sensation you can't much describe. After some time speculating what it may be, you see a small stone on the
echo ground and can't help but try to move it just by your thoughts.
echo.
echo ...
pause>nul
echo.
echo You concentrate as hard as you can and after a few seconds...
echo.
echo ...
pause>nul
echo.
echo ...nothing happens. Well, at least you tried.
echo.
echo ...
pause>nul
echo.
echo But then you realise that Bystrik wrote this and also that he loves his girlfriend very VERY much. So, to
echo make her happy, he allows the white cat to try again. This time...
echo.
echo ...
pause>nul
echo.
echo You succeed, blowing the poor pebble into heaven and back and now possess telekinetic abilities! And he
echo loves you so much so that you also spawin in a Lambo and you can fly and you can...
echo.
echo ...
pause>nul
echo.
echo Well, let's leave it at the telekinesis, shall we? :D I'll give you the Lambo later ;)
echo.
echo ...
pause>nul
echo.
echo After realising you now possess telekinesis, you decide to look around. There is nothing but sand, except
echo for the singular tiny rock you threw into oblivion with you telekinesis, which is actually not there
echo anymore. You can see nothing but sand above sand above sand. No buildings, no water, just sand. The sun is
echo scorching and you sweat a lot. You need to find anything. Literally anything would be better than this.
echo You have to decide which way to go. You think about going the way you were facing when you teleported, but
echo that small stone could be a navigation point that was prepared for you.
echo.
echo (stone / teleport)
set /p "direction=I want to go the direction of the "
if /i "%direction%"=="stone" (goto :oasis) else (goto :oasis)

:oasis
echo.
echo You walk for what feels like 3 hours when you finally see an oasis in close distance. You speed up as you
echo long for a fresh water.
echo.
echo ...
pause>nul
echo.
echo You come to the oasis and have a nice cold drink, even though the air is extremely hot. After you drink as
echo much water as you need, you start to sense the magic of this place. This is even more magical than the
echo village you came from. You look up and see a camel that is doing funny faces at you.
echo.
echo (wave / funnyface / nothing)
set /p "decision=I will do "
if /i "%decision%"=="wave" (goto :waveatcamel)
if /i "%decision%"=="funnyface" (goto :doafunnyfaceatcamel)
if /i "%decision%"=="nothing" (goto :donothingatcamel)

:waveatcamel
echo.
echo You wave at it, just for fun. Because why not.
echo.
echo ...
pause>nul
goto chatwithcamel

:doafunnyfaceatcamel
echo.
echo You return a funny face to the camel.
echo.
echo ...
pause>nul
goto chatwithcamel

:donothingatcamel
echo.
echo You do nothing and wait for what comes next.
echo.
echo ...
pause>nul
goto chatwithcamel

:chatwithcamel
echo.
echo The camel laughs almost like a normal cat would and signals you to wait there.
echo.
echo ...
pause>nul
echo.
echo After some time the camel finally comes to you.
echo.
echo ...
pause>nul
echo.
echo The Camel: Heeeey funky lady! I'm a camel, despite what that one idiot thinks.
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: Wha... You can TALK?
echo.
echo ...
pause>nul
echo.
echo The Camel: You've met bears, dogs and whatever else that could -hablar- and at the SAME TIME are
echo        -sorprendido- that a camel can -hablar-?
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: Considering I was surprised you even talked, you aren't proving me otherwise by speaking
echo        Spanish.
echo.
echo ...
pause>nul
echo.
echo The Lamb (What?): Hey, let's -introducir- ourselves shall we? According to a certain -hombre-, I'm a LAMB!
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: A *lamb* you say?
echo.
echo ...
pause>nul
echo.
echo The Lamb (ah, makes sense): Well I'm not a lamb -obviamente-. As you can see with your own -ojos-. But because
echo        of this -biologico- misunderstanging, I have *lamb* in my -nombre-. Followed by -realizacion-. It stuck,
echo        even though nobody knows why.
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: What do you mean by "realization"?
echo.
echo ...
pause>nul
echo.
echo The Lamb: You see, when they were naming me, they thought I was a lamb. They didn't have a lamb here, so I
echo        was just supposed to be called "lamb". But then he realized and said "Oh..."
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: So you're telling me your name is...
echo.
echo ...
pause>nul
echo.
echo Lamb-Oh: Lamb-Oh, -pero- you can call me Lambo, for short.
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: Well, hi Lambo, I'm %whitecatname%.
echo.
echo ...
pause>nul
echo.
echo Lambo: Hey %whitecatname%, nice to meet you.
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: So, Lambo, what are you doing here?
echo.
echo ...
pause>nul
echo.
echo Lambo: Oh. I’m here because I was thirsty, of course! And what are you doing here my new cat friend?
echo.
echo ...
pause>nul
echo.
echo %whitecatquest%: I’m here to kill Xramius somehow. That’s supposed to be a gia…
echo.
echo ...
pause>nul
echo.
echo Lambo laughs out loud
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: What? I didn’t make it up even though it may seem like it.
echo.
echo ...
pause>nul
echo.
echo Lambo: No, I know it’s true. It’s just something near impossible. You would -necesitar- to be able to move stuff just using your mind. His attacks can’t be parried with just 2 limbs.
echo.
echo ...
pause>nul
echo.
echo You demonstrate your new telekinetic abilities on a nearby tree by ripping it out of the ground and throwing it into the water.
echo.
echo ...
pause>nul
echo.
echo Lambo: …
echo.
echo ...
pause>nul
echo.
echo Lambo: I want to be your best -amigo-.
echo.
echo ...
pause>nul
echo.
echo You both laugh
echo.
echo ...
pause>nul
echo.
echo Lambo: Listen. I know this land. I’ve been here for too long now. Let’s make a deal. I will show you around and you can kill everything in our way if necessary. Or if you want to, your choice. Anyway, we would be a great team. I can run pretty fast, so if you rode me we could be great warriors. The only proper challenge would be the great worm, but with your abilities I don’t even think you need the help of the people here.
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: Well, I’d still rather had their support. Winning easily and winning just barely is a huge difference. Take me to their city or village or whatever they live in.
echo.
echo ...
pause>nul
echo.
echo Lambo: It’s a long and dangerous journey, but of course. Without a doubt. It will take us approximately 5 days to get there.
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: Ok. Let’s go then. I want to be there as soon as possible.
echo.
echo ...
pause>nul
echo.
echo You hop onto Lambo and fire up his V12 AKA tell him to start moving.
echo.
echo ...
pause>nul
echo.
echo You walk for the rest of the day and in the evening you find a reasonable spot to sleep at. As you both sit down to talk, you agree to get some water. You look around and don’t see anything.
echo.
echo ...
pause>nul
goto dunesdayonechoice

:dunesdayonechoice
echo.
echo (weapon / telekinesis)
SWORD —> dunestryweapon
TELEKINESIS —> dunestrytelekinesis

:dunestryweapon
echo.
echo You unsheath your %weapon%, look at it and look around
echo (dig / play / throw)
DIG —> dunesweapondig
PLAY —> dunesweaponplay
THROW —> dunesweaponthrow

:dunesweapondig
echo.
echo You try digging a hole in the ground to reach some water but nothing happens.
echo.
echo ...
pause>nul
echo.
echo Lambo: That won’t be possible. There is no water beneath these piles of sand.
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: Yeah, I figured as much. Well, let’s try something else.
echo.
echo ...
pause>nul
goto dunesdayonechoice

:dunesweaponplay
echo.
echo You take your %weapon% and play with it for a while. You didn’t find any water. What were you thinking?
echo.
echo ...
pause>nul
echo.
echo Lambo: Purposeless, but cool.
echo.
echo ...
pause>nul
goto dunesdayonechoice

:dunesweaponthrow
echo.
echo You throw your %weapon% into the sand in front of you.
echo.
echo ...
pause>nul
echo.
echo Lambo: Why did you do that?
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: I just don’t like the sand I guess.
echo.
echo ...
pause>nul
goto dunesdayonechoice

:dunestrytelekinesis
echo.
echo You remember you have superpowers. But how to use them to get water?
echo.
echo (sand / Lambo)
SAND —> dunestelekinesissand
LAMBO —> dunestelekinesislambo

:dunestelekinesissand
echo.
echo You pick up some sand and make a nice tornado out of it, eventually becoming a sandstorm.
echo.
echo ...
pause>nul
echo.
echo Lambo: I don’t see the -rason-. Other than showing off your new -habilidad- though. You can keep doing it. It’s really impressive to watch.
echo.
echo ...
pause>nul
echo.
echo You perform a great show to Lambo, but don’t get any water
goto dunesdayonechoice

:dunestelekinesislambo
echo.
echo You pick up Lambo and rise him 20 metres into the sky.
echo.
echo ...
pause>nul
echo.
echo Lambo: Hey! Put me down!
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: Ok ok ok. I’ll get you back down.
echo.
echo ...
pause>nul
echo.
echo Lambo: WAIT! I can see something about 60 metres away. I don’t know what but we should go and have a look!
echo.
echo ...
pause>nul
echo.
echo %whitecatname%: Definitely. I’ll get you down and we can set off.
echo.
echo ...
pause>nul
echo.
echo After some time you find a well with a singular cactus standing 5 metres from it.