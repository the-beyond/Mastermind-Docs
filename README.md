![alt text](https://i.ibb.co/hs2Ym63/mastermind.png "Mastermind Logo")
# Mastermind Documentation
This is the public documentation for The Beyond's Blood on the Clocktower Discord bot. The bot has been developed in Python using the Nextcord module which is a fork of the original discord.py module. All commands are slash commands.
### Key Notes
* Anything listed in <> is a required argument for the commands and the command will not work without it, DO NOT INCLUDE THE <> IN THE COMMAND.
* Anything listed in [] is an optional argument for the commands and allows the command to use what you add, DO NOT INCLUDE THE [] IN THE COMMAND.
## General Commands
* Base Counts
  * `/base_counts photo`: Get the photo listing all base counts.
  * `/base_counts generic_lookup <count: The number of players to get base counts for>`: Get the base counts for a specified number of players.
  * `/base_counts current_game`: Get the base counts for the number of players in the current game.
* `/cult_leader [cult_description: What is your cult like? Why should people join it?]`: Request that players join our cult.
* `/doomsayer call_upon`: Call upon the Doomsayer!
* `/duchess`: Go and visit the Duchess!
* `/documentation`: Get the link to the Mastermind documentation! (You are here!)
* Gangster
  * `/gangster ga_select <kill_player: the neighbor you want to kill> <agree_player: the neighbor that must agree to the killing>`: Select a neighbor to kill (once a day).
  * `/gangster ga_respond <result: Do you agree to kill the indicated player?`: Respond to a gangster kill request.
* `/give_beggar_vote`: Donate your dead vote to the beggar.
* `/gossip <tidbit: your juicy gossip for the day>`: Send your gossip for the day.
* `/guess_damsel <player: the player that you're guessing is the damsel>`: Attempt to guess the damsel. One use per game.
* `/gunslinger <player: the player to target>`: Attempt to use the gunslinger ability.
* `/judge <vote_num: Which vote of the day are you ruling on?> <result: How should the selected vote proceed?>`: Decide the outcome of an execution.
* `/juggler <player1: Select a player!> <role1: What role will you juggle them as?>`: Do some juggling! (Up to 5 players)
* Klutz
  * `/klutz kl_claim`: Publically claim to be the Klutz.
  * `/klutz kl_select <player: the player you want to target>`: Select the player you want to use the klutz ability on.
* `/meetup <target: Who will you meetup with?> <meet_channel: Which channel are you meeting in?>`: Send a meetup message!
* `/meetup_storyteller`: Send a meetup message for the Storyteller!
* Moonchild
  * `/moonchild mc_claim`: Publically claim to be the moonchild!
  * `/moonchild mc_select <player: Select the player you want to target with the moonchild ability.>`: Select the player you want to use the moonchild ability on!
* `/nominate <player: Select the player to nominate.> <reason: Optional (but encouraged) reason for nominating them.>`: Nominate a player for execution!
* Psychopath
  * `/psychopath axe_attack <target: Who will suffer from your attack?>`: Attack a player as the Psychopath!
  * `/psychopath roshambo <choice: Rock, Paper, or Scissors?>`: Play Roshambo to see if you die!
* Resources
  * `/resources script_directory`: Get the link to the script directory!
  * `/resources spreadsheet`: Get the link to Eru's spreadsheet template!
  * `/resources wiki [page: Select wiki page to lookup. If left blank, will default to the BotC wiki homepage.]`: Get BotC Wiki links!
* `/slayer <player: Select the player to slay!>`: Attempt to use the Slayer ability!

## Storyteller Commands
These commands will only function for users with the `Storyteller` role.
* `/add_vote <player: Who is having their vote added?>`: Add a vote to a dead player!
* Announce
  * `/announce al_hadikhia <choice1: first selection> <choice 2: second selection> <choice3: third selection>`: Announce the choices of the Al-Hadikhia!
  * `/announce conclude [message: Optional, enter any special message you need to add.]`: End the morning announcements!
  * `/announce fearmonger`: Announce the Fearmonger has chosen a player!
  * `/announce leviathan <day: Which day number is it?> [message: additional optional message]`: Announce that there is a Leviathan!
  * `/announce newday <day: What day is it?> <player_count: How many players are in the game?>`: Start a new day!
  * `/announce night_death <player: Who died?> [cause: Cause of death?]`: Announce a player died at night!
  * `/announce nothing`: Announce nothing!
  * `/announce resurrect <player: Who is being resurrected?>`: Resurrect a dead player!
  * `/announce vizier <player: Who is the Vizier?>`: Announce the Vizier is in play!
* `/build_script <num_players: Number of players that will be playing.> <script: Which type of game would you like?>`: Generate a random player list for the selected BotC script!
* `/doomsayer enact_wrath <caller: Who called upon the Doomsayer?> <victim: Who will suffer the wrath?>`: Enact the wrath of the Doomsayer!
* Execution
  * `/execution ex_death <player: Select the dying player!> <message: Enter the message as part of the embed!> [votes: Optional, how many votes did they have?]`: A player is executed and dies!
  * `/execution ex_nodeath <player: Select the dying player!> <message: Enter the message as part of the embed!> [votes: Optional, how many votes did they have?]`: A player is executed and does not die!
* `/exile <player: Who is being exiled?> <votes: How many votes did they get?>`: Exile a traveller!
* `/fiddler <day: What day will the Fiddler end the game?>`: Causes the Fiddler to enter the game!
* `/log_vote <vote_number: Which vote was this?> <nominee: Who was the nominee?> <nominator: Who nominated them?> <votes: Enter the vote count!> <result: Select the result!> [note: Optional, enter an additional note!]`: Log a recently finished vote!
* `/misc_death <player: Who is dying?> [reason: Optional, why did they die?]`: mark a player as Dead for any other reason!
* Nuke
  * `/nuke single`: Nuke the channel you are currently in.
  * `/nuke mass_nuke`: Nuke all village channels.
* `/remove_vote <player: Who is having their vote removed?>`: Remove a vote from a dead player!
