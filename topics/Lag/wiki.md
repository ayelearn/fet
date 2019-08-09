The following text has been accessed from https://en.wikipedia.org/wiki/Lag at Thu Aug 8 22:54:59 IST 2019
Creative_Commons_Attribution-ShareAlike_License




















****** Lag ******
From Wikipedia, the free encyclopedia
Jump_to_navigation Jump_to_search
For other uses, see Lag_(disambiguation).
 This article has multiple issues. Please help improve_it or discuss these issues on the talk_page. (Learn_how
 and_when_to_remove_these_template_messages)
  This article needs additional citations for verification. Please help improve_this_article by adding_citations_to_reliable
  sources. Unsourced material may be challenged and removed.
  Find sources: "Lag" â news Â· newspapers Â· books Â· scholar Â· JSTOR (April 2011)(Learn_how_and_when_to_remove_this
  template_message)
  This article possibly contains original_research. Please improve_it by verifying the claims made and adding
  inline_citations. Statements consisting only of original research should be removed. (December 2008)(Learn
  how_and_when_to_remove_this_template_message)
  This article contains instructions,_advice,_or_how-to_content. The purpose of Wikipedia is to present facts,
  not to train. Please help improve_this_article either by rewriting the how-to content or by moving it to
  Wikiversity, Wikibooks or Wikivoyage. (April 2016)
 (Learn_how_and_when_to_remove_this_template_message)
In online_gaming, lag is a noticeable delay between the action of players and
the reaction of the server supporting the video_game.
The tolerance for lag depends on the type of game. For instance, a strategy
game or a turn-based_game with a low pace may have a high threshold or even be
mostly unaffected by high delays, whereas a twitch_gameplay game such as a
first-person_shooter with a considerably higher pace may require significantly
lower delay to be able to provide satisfying gameplay. However, the specific
characteristics of the game matter. For example, fast_chess is a turn-based
game that is fast action and may not tolerate high lag. Also, some twitch games
can be designed such that only events that don't impact the outcome of the game
introduce lag, allowing for fast local response most of the time.
⁰
***** Contents *****
    * 1_Etymology
    * 2_Ping
    * 3_Causes
    * 4_Effects
    * 5_Solutions_and_lag_compensation
          o 5.1_Client-side
          o 5.2_Server-side
                # 5.2.1_Rewind_time
                # 5.2.2_Trust_clients
                # 5.2.3_Make_clients_extrapolate
          o 5.3_Design
    * 6_Cloud_gaming
    * 7_See_also
    * 8_References
***** Etymology[edit] *****
The origin of this term is unknown, but it might be from North_Germanic;
compare Norwegian lagga "to move slowly".
***** Ping[edit] *****
Ping refers to the network latency between a player's client and the game
server as measured with the ping_utility or equivalent. Ping is reported
quantitatively as an average time in milliseconds (ms). The lower one's ping
is, the lower the latency is and the less lag the player will experience. High
ping and low ping are commonly used terms in online gaming, where high ping
refers to a ping that causes a severe amount of lag; while any level of ping
may cause lag, severe lag is usually caused by a ping of over 100 ms.[1] This
usage is a gaming cultural colloquialism and is not commonly found or used in
professional computer networking circles. In games where timing is key, such as
first-person_shooter and real-time_strategy games, a low ping is always
desirable, as a low ping means smoother gameplay by allowing faster updates of
game data between the players' clients and game server.
High latency can cause lag. Game servers may disconnect a client if the latency
is too high and may pose a detriment to other players' gameplay. Similarly,
client software will often mandate disconnection if the latency is too high.
High ping may also cause servers to crash due to instability.
In some first-person shooter games, a high ping may cause the player to
unintentionally gain unfair advantages, such as disappearing from one location
and instantaneously reappearing in another, simulating the effect of
teleportation, thus making it hard for other players to judge their character's
position and subsequently making the player much more difficult to target. To
counter this, many game servers automatically kick players with a ping higher
than average. Conversely, a high ping can make it very difficult for the player
to play the game due to negative effects occurring, making it difficult for the
player to track other players and even move their character.
Rather than using the traditional ICMP echo request and reply network_packets
to determine ping times, video_game_programmers often build their own latency
detection into existing game packets (usually based on the UDP protocol)
instead.
Some factors that might affect ping include: communication_protocol used,
Internet throughput (connection speed), the quality of a user's Internet
service provider and the configuration of firewalls. Ping is also affected by
geographical location. For instance, if someone is in India, playing on a
server located in the United States, the distance between the two is greater
than it would be for players located within the US, and therefore it takes
longer for data to be transmitted. However, the amount of packet-switching and
network hardware in between the two computers is often more significant. For
instance, wireless_network_interface_cards must modulate digital signals into
radio_signals, which is often more costly than the time it takes an electrical
signal to traverse a typical span of cable. As such, lower ping can result in
faster internet download and upload rates.
***** Causes[edit] *****
A simplified game architecture
While a single-player_game maintains the main game state on the local machine,
an online_game requires it to be maintained on a central server in order to
avoid inconsistencies between individual clients. As such, the client has no
direct control over the central game state and may only send change requests to
the server, and can only update the local game state by receiving updates from
the server. This need to communicate causes a delay between the clients and the
server, and is the fundamental cause behind lag. While there may be numerous
underlying reasons for why a player experiences lag, they can be summarized as
insufficient hardware in either the client or the server, or a poor connection
between the client and server.[2]
Hardware related issues cause lag due to the fundamental structure of the game
architecture. Generally, games consist of a looped sequence of states, or
"frames". During each frame, the game accepts user input and performs necessary
calculations (AI, graphics etc.). When all processing is finished, the game
will update the game state and produce an output, such as a new image on the
screen and/or a packet to be sent to the server. The frequency at which frames
are generated is often referred to as the frame_rate. As the central game state
is located on the server, the updated information must be sent from the client
to the server in order to take effect. In addition, the client must receive the
necessary information from the server in order to fully update the state.
Generating packets to send to the server and processing the received packets
can only be done as often as the client is able to update its local state.
Although packets could theoretically be generated and sent faster than this, it
would only result in sending redundant data if the game state cannot be updated
between each packet. A low frame rate would, therefore, make the game less
responsive to updates and may force it to skip outdated data.
Conversely, the same holds true for the server. The frame rate (or tick rate)
of the server determines how often it can process data from clients and send
updates. This type of problem is difficult to predict and compensate for. Apart
from enforcing minimum hardware requirements and attempting to optimize the
game for better performance, there are no feasible ways to deal with it.
Perhaps the most common type of lag is caused by network_performance problems.
Losses, corruption or jitter (an outdated packet is in effect a loss) may all
cause problems, but these problems are relatively rare in a network with
sufficient bandwidth and no or little congestion. Instead, the latency involved
in transmitting data between clients and server plays a significant role.
Latency varies depending on a number of factors, such as the physical distance
between the end-systems, as a longer distance means additional transmission
length and routing required and therefore higher latency. Routing over the
Internet may be extremely indirect, resulting in far more transmission length
(and consequent latency) than a direct route, although the cloud gaming service
OnLive has developed a solution to this issue by establishing peering
relationships with multiple Tier_1_network Internet Service Providers and
choosing an optimal route between server and user.[3] In addition, insufficient
bandwidth and congestion, even if not severe enough to cause losses, may cause
additional delays regardless of distance. As with the hardware issues, packets
that arrive slowly or not at all will make both the client and server unable to
update the game state in a timely manner.
Online game systems utilizing a wireless_network may be subject to significant
lag, depending on the architecture of the wireless network and local
electromagnetic_interference impacting that network. Electromagnetic
interference (e.g. from a microwave_oven) can cause transmitted packets to be
lost, requiring a retransmission which incurs latency. Although radio
propagation through the air is faster than light through an optical fiber,
wireless systems are often shared among many users and may suffer from latency
incurred due to network_congestion, or due to network_protocols that introduce
latency.
***** Effects[edit] *****
The noticeable effects of lag vary not only depending on the exact cause, but
also on any and all techniques for lag compensation that the game may implement
(described below). As all clients experience some delay, implementing these
methods to minimize the effect on players is important for smooth gameplay. Lag
causes numerous problems for issues such as accurate rendering of the game
state and hit detection.[4] In many games, lag is often frowned upon because it
disrupts normal gameplay. The severity of lag depends on the type of game and
its inherent tolerance for lag. Some games with a slower pace can tolerate
significant delays without any need to compensate at all, whereas others with a
faster pace are considerably more sensitive and require extensive use of
compensation to be playable (such as the first-person shooter genre). Due to
the various problems lag can cause, players that have an insufficiently fast
Internet connection are sometimes not permitted, or discouraged from playing
with other players or servers that have a distant server host or have high
latency to one another. Extreme cases of lag may result in extensive
desynchronization of the game state.
Lag due to an insufficient update rate between client and server can cause some
problems, but these are generally limited to the client itself. Other players
may notice jerky movement and similar problems with the player associated with
the affected client, but the real problem lies with the client itself. If the
client cannot update the game state at a quick enough pace, the player may be
shown outdated renditions of the game, which in turn cause various problems
with hit- and collision detection.[5] If the low update rate is caused by a low
frame rate (as opposed to a setting on the client, as some games allow), these
problems are usually overshadowed by numerous problems related to the client-
side processing itself. Both the display and controls will be sluggish and
unresponsive. While this may increase the perceived lag, it is important to
note that it is of a different kind than network-related delays. In comparison,
the same problem on the server may cause significant problems for all clients
involved. If the server is unable or unwilling to accept packets from clients
fast enough and process these in a timely manner, client actions may never be
registered. When the server then sends out updates to the clients, they may
experience freezing (unresponsive game) and/or rollbacks, depending on what
types of lag compensation, if any, the game uses.
Lag due to network delay is in contrast often less of a problem. Though more
common, the actual effects are generally smaller, and it is possible to
compensate for these types of delays. Without any form of lag compensation, the
clients will notice that the game responds only a short time after an action is
performed. This is especially problematic in first-person shooters, where
enemies are likely to move as a player attempts to shoot them and the margin
for errors is often small.
***** Solutions and lag compensation[edit] *****
There are various methods for reducing or disguising delays, though many of
these have their drawbacks and may not be applicable in all cases. If
synchronization is not possible by the game itself, the clients may be able to
choose to play on servers in geographical proximity to themselves in order to
reduce latencies, or the servers may simply opt to drop clients with high
latencies in order to avoid having to deal with the resulting problems.
However, these are hardly optimal solutions. Instead, games will often be
designed with lag compensation in mind.[6]
Many problems can be solved simply by allowing the clients to keep track of
their own state and send absolute states to the server or directly to other
clients.[7] For example, the client can state exactly at what position a
player's character is or who the character shot. This solution works and will
all but eliminate most problems related to lag. Unfortunately, it also relies
on the assumption that the client is honest. There is nothing that prevents a
player from modifying the data they send, directly at the client or indirectly
via a proxy, in order to ensure they will always hit their targets. In online
games, the risk of cheating may make this solution unfeasible, and clients will
be limited to sending relative states (i.e. which vector it moved on or shot
in).
**** Client-side[edit] ****
As clients are normally not allowed to define the main game state, but rather
receive it from the server, the main task of the client-side compensation is to
render the virtual world as accurately as possible. As updates come with a
delay and may even be dropped, it is sometimes necessary for the client to
predict the flow of the game. Since the state is updated in discrete steps, the
client must be able to estimate a movement based on available samples. Two
basic methods can be used to accomplish this; extrapolation and interpolation.
[7]
Extrapolation is an attempt to estimate a future game state. As soon as a
packet from the server is received, the position of an object is updated to the
new position. Awaiting the next update, the next position is extrapolated based
on the current position and the movement at the time of the update.
Essentially, the client will assume that a moving object will continue in the
same direction. When a new packet is received, the position may be corrected
slightly.
Interpolation works by essentially buffering a game state and rendering the
game state to the player with a slight, constant delay. When a packet from the
server arrives, instead of updating the position of an object immediately, the
client will start to interpolate the position, starting from the last known
position. Over an interpolation interval, the object will be rendered moving
smoothly between the two positions. Ideally, this interval should exactly match
the delay between packets, but due to loss and variable delay, this is rarely
the case.
Both methods have advantages and drawbacks.
    * Interpolation ensures that objects will move between valid positions only
      and will produce good results with constant delay and no loss. Should
      dropped or out-of-order packets overflow the interpolation buffer the
      client will have to either freeze the object in position until a new
      packet arrives, or fall back on extrapolation instead. The downside of
      interpolation is that it causes the world to be rendered with additional
      latency, increasing the need for some form of lag compensation to be
      implemented.
    * The problem with extrapolating positions is fairly obvious: it is
      impossible to accurately predict the future. It will render movement
      correctly only if the movement is constant, but this will not always be
      the case. Players may change both speed and direction at random. This may
      result in a small amount of "warping" as new updates arrive and the
      estimated positions are corrected, and also cause problems for hit
      detection as players may be rendered in positions they are not actually
      in.
Often, in order to allow smooth gameplay, the client is allowed to do soft
changes to the game state. While the server may ultimately keep track of
ammunition, health, position, etc., the client may be allowed to predict the
new server-side game state based on the player's actions, such as allowing a
player to start moving before the server has responded to the command. These
changes will generally be accepted under normal conditions and make delay
mostly transparent. Problems will arise only in the case of high delays or
losses, when the client's predictions are very noticeably undone by the server.
Sometimes, in the case of minor differences, the server may even allow
"incorrect" changes to the state based on updates from the client.
**** Server-side[edit] ****
Unlike clients, the server knows the exact current game state, and as such
prediction is unnecessary. The main purpose of server-side lag compensation is
instead to provide accurate effects of client actions. This is important
because by the time a player's command has arrived time will have moved on, and
the world will no longer be in the state that the player saw when issuing their
command. A very explicit example of this is hit detection for weapons fired in
first-person shooters, where margins are small and can potentially cause
significant problems if not properly handled.
*** Rewind time[edit] ***
Another way to address the issue is to store past game states for a certain
length of time, then rewind player locations when processing a command.[7] The
server uses the latency of the player (including any inherent delay due to
interpolation; see above) to rewind time by an appropriate amount in order to
determine what the shooting client saw at the time the shot was fired. This
will usually result in the server seeing the client firing at the target's old
position and thus hitting. In the worst case, a player will be so far behind
that the server runs out of historical data and they have to start leading
their targets.
This is a WYSIWYG solution that allows players to aim directly at what they are
seeing. But the price is an aggravation of the effects of latency when a player
is under fire: not only does their own latency play a part, but their
attacker's too. In many situations, this is not noticeable, but players who
have just taken cover will notice that they carry on receiving damage/death
messages from the server for longer than their own latency can justify. This
can lead more often to the (false) impression that they were shot through cover
and the (not entirely inaccurate) impression of "laggy hitboxes".[7]
One design issue that arises from rewinding is whether to stop rewinding a dead
player's lagged commands as soon as they die on the server, or to continue
running them until they "catch up" to the time of death. Cutting compensation
off immediately prevents victims from posthumously attacking their killers,
which meets expectations, but preserves the natural advantage of moving players
who round a corner, acquire a target and kill them in less time than a round
trip to the stationary victim's client.
Rewinding can be criticised for allowing the high latency of one player to
negatively affect the experience of low-latency players. Servers with lag
compensation will sometimes reduce the length of player history stored, or
enforce ping limits, to reduce this problem.
*** Trust clients[edit] ***
It is possible for clients to tell the server what they are doing and for the
server to trust the data it receives. This method is avoided if at all possible
due to its susceptibility to cheating: it is a simple matter to route network
data through a second computer which inserts fabricated hit messages or
modifies existing ones, a technique which cannot be detected by anti-cheat
tools.[7]
However, the sheer scale of some games makes computationally expensive
solutions like rewinding impossible. In Battlefield_3, for example, a "hybrid
hit detection" system is used where clients tell the server that they hit and
the server performs only a vague test of plausibility before accepting the
claim.[8]
Trusting a client's results otherwise has the same advantages and disadvantages
as rewinding.
*** Make clients extrapolate[edit] ***
A less common lag solution is to do nothing on the server and to have each
client extrapolate (see above) to cover its latency.[9] This produces incorrect
results unless remote players maintain a constant velocity, granting an
advantage to those who dodge back and forth or simply start/stop moving.
Extended extrapolation also results in remote players becoming visible (though
not vulnerable) when they should not be: for example if a remote player sprints
up to a corner then stops abruptly at the edge, other clients will render them
sprinting onward, into the open, for the duration of their own latency. On the
other side of this problem, clients have to give remote players who just
started moving an extra burst of speed in order to push them into a
theoretically-accurate predicted location.
**** Design[edit] ****
It is possible to reduce the perception of lag through game_design. Techniques
include playing client-side animations as if the action took place immediately,
reducing/removing built-in timers on the host machine, and using camera
transitions to hide warping.[10]
***** Cloud gaming[edit] *****
Cloud_gaming is a type of online gaming where the entire game is hosted on a
game server in a data center, and the user is only running a thin_client
locally that forwards game_controller actions upstream to the game server. The
game server then renders the next frame of the game video which is compressed
using low-lag video_compression and is sent downstream and decompressed by the
thin client. For the cloud gaming experience to be acceptable, the round-trip
lag of all elements of the cloud gaming system (the thin client, the Internet
and/or LAN connection the game server, the game execution on the game server,
the video and audio compression and decompression, and the display of the video
on a display_device) must be low enough that the user perception is that the
game is running locally.[3][11] Because of such tight lag requirements,
distance considerations of the speed_of_light through optical_fiber come into
play, currently limiting the distance between a user and a cloud gaming game
server to approximately 1000 miles, according to OnLive, the only company thus
far operating a cloud gaming service.[12] There is also much controversy about
the lag associated with cloud gaming. In multiplayer games using a client/
server network architecture, the player's computer renders the game's graphics
locally and only information about the player's in-game actions are sent to the
server. For example, when the player presses a button, the character on-screen
instantly performs the corresponding action. However, the consequences of the
action such as an enemy being killed are only seen after a short delay due to
the time taken for the action to reach the server. This is only acceptable as
long as the response to the player's input is fast enough.
When using cloud gaming, inputs by the player can lead to short delays until a
response can be seen by them. Inputs must first be transmitted to the remote
server, then the server must start rendering the graphics of the action being
performed and stream the video back to the player over the network, taking
additional time. Thus, the player experiences a noticeable delay between
pressing a button and seeing something happen on-screen. Depending on the skill
and experience of the player, this can cause disorientation and confusion
similar to Delayed_Auditory_Feedback and hampers navigation and aiming in the
game world. When rapidly inputting a long combination move, the on-screen
character will not be synchronized with the button presses. This usually causes
severe confusion in the player resulting in the failure of the combination
move.
The extra input lag can also make it very difficult to play certain single
player games. For example, if an enemy takes a swing at the player and the
player is expected to block, then by the time the player's screen shows that
the enemy has commenced attacking, the enemy would have already struck and
killed the player on the server.
***** See also[edit] *****
    * Lagometer
    * Latency_(engineering)
***** References[edit] *****
   1. ^"How_to_Get_Rid_of_Lag_|_GeForce". www.geforce.com. Retrieved 2018-09-
      13.
   2. .mw-parser-output cite.citation{font-style:inherit}.mw-parser-output
      .citation q{quotes:"\"""\"""'""'"}.mw-parser-output .citation .cs1-lock-
      free a{background:url("//upload.wikimedia.org/wikipedia/commons/thumb/6/
      65/Lock-green.svg/9px-Lock-green.svg.png")no-repeat;background-position:
      right .1em center}.mw-parser-output .citation .cs1-lock-limited a,.mw-
      parser-output .citation .cs1-lock-registration a{background:url("//
      upload.wikimedia.org/wikipedia/commons/thumb/d/d6/Lock-gray-alt-2.svg/
      9px-Lock-gray-alt-2.svg.png")no-repeat;background-position:right .1em
      center}.mw-parser-output .citation .cs1-lock-subscription a{background:
      url("//upload.wikimedia.org/wikipedia/commons/thumb/a/aa/Lock-red-alt-
      2.svg/9px-Lock-red-alt-2.svg.png")no-repeat;background-position:right
      .1em center}.mw-parser-output .cs1-subscription,.mw-parser-output .cs1-
      registration{color:#555}.mw-parser-output .cs1-subscription span,.mw-
      parser-output .cs1-registration span{border-bottom:1px dotted;cursor:
      help}.mw-parser-output .cs1-ws-icon a{background:url("//
      upload.wikimedia.org/wikipedia/commons/thumb/4/4c/Wikisource-logo.svg/
      12px-Wikisource-logo.svg.png")no-repeat;background-position:right .1em
      center}.mw-parser-output code.cs1-code{color:inherit;background:
      inherit;border:inherit;padding:inherit}.mw-parser-output .cs1-hidden-
      error{display:none;font-size:100%}.mw-parser-output .cs1-visible-error
      {font-size:100%}.mw-parser-output .cs1-maint{display:none;color:
      #33aa33;margin-left:0.3em}.mw-parser-output .cs1-subscription,.mw-parser-
      output .cs1-registration,.mw-parser-output .cs1-format{font-size:95%}.mw-
      parser-output .cs1-kern-left,.mw-parser-output .cs1-kern-wl-left{padding-
      left:0.2em}.mw-parser-output .cs1-kern-right,.mw-parser-output .cs1-kern-
      wl-right{padding-right:0.2em}
   3. ^Cronin, Eric; Filstrup, Burton; Anthony, Kurc. "A_Distributed
      Multiplayer_Game_Server_System" (PDF). University of Michigan. Retrieved
      16 July 2014.
   4. ^ a b"The_Process_of_Invention:_OnLive_Video_Game_Service". The FU
      Foundation School of Engineering & Applied Science (Columbia University).
      Retrieved 2010-01-23.
   5. ^Smith, Joshua. "Distributed_Game_Architecture_To_Overcome_System
      Latency" (PDF). United States Patent. Retrieved 16 July 2014.
   6. ^Claypool, Mark; Claypool, Kajal. "Latency_Can_Kill:_Precision_and
      Deadline_in_Online_Games". Retrieved 16 July 2014.
   7. ^Roelofs, Gregory. "Compensating_For_Network_Latency_In_A_Multi-Player
      Game" (PDF). United States Patent. Retrieved 16 July 2014.
   8. ^ a b c d eBernier, Yahn (2001). "Latency_Compensating_Methods_in_Client/
      Server_In-game_Protocol_Design_and_Optimization". Valve_Corporation.
      Retrieved 17 September 2011.
   9. ^Kertz, Alan (December 11, 2011). "Re:_We_need_someone_to_create_a_guide
      for_the_new_Network_Interpolation_Setting_slider". Retrieved 4 November
      2013. BF3's hit model uses a combined client server model, a Hybrid Hit
      Detection. The client says to the server "Hey, I shot him!" and the
      server does a check against the position of the two targets and
      determines if the player could reasonably have hit that target and then
      applies the damage.
  10. ^Gibson, John (5 December 2010). "Re:_Will_HoS_present_the_netcode
      disadvantages_of_UE3?". Tripwire_Interactive. Retrieved 18 September
      2011.
  11. ^Aldridge, David (2011). "I_Shot_You_First:_Networking_the_Gameplay_of
      HALO:_REACH". Game Developers Conference 2011. GDC Vault.
  12. ^"D8_Video:OnLive_demoed_on_iPad,_PC,_Mac,_Console,_iPhone". Wall Street
      Journal. 2010-08-09. Retrieved 2010-08-19.
  13. ^"Beta_Testing_at_the_Speed_of_Light". OnLive. 2010-01-21. Retrieved
      2010-01-23.

Retrieved from "https://en.wikipedia.org/w/index.php?title=Lag&oldid=908566831"
Categories:
    * Online_games
    * Computer_networks
    * Multiplayer_video_games
    * Video_game_terminology
Hidden categories:
    * Articles_needing_additional_references_from_April_2011
    * All_articles_needing_additional_references
    * Articles_that_may_contain_original_research_from_December_2008
    * All_articles_that_may_contain_original_research
    * Articles_needing_cleanup_from_April_2016
    * All_pages_needing_cleanup
    * Articles_containing_how-to_sections
    * Articles_with_multiple_maintenance_issues
***** Navigation menu *****
**** Personal tools ****
    * Not logged in
    * Talk
    * Contributions
    * Create_account
    * Log_in
**** Namespaces ****
    * Article
    * Talk
⁰
**** Variants ****
**** Views ****
    * Read
    * Edit
    * View_history
⁰
**** More ****
**** Search ****
[Unknown INPUT type][Search][Go]
**** Navigation ****
    * Main_page
    * Contents
    * Featured_content
    * Current_events
    * Random_article
    * Donate_to_Wikipedia
    * Wikipedia_store
**** Interaction ****
    * Help
    * About_Wikipedia
    * Community_portal
    * Recent_changes
    * Contact_page
**** Tools ****
    * What_links_here
    * Related_changes
    * Upload_file
    * Special_pages
    * Permanent_link
    * Page_information
    * Wikidata_item
    * Cite_this_page
**** Print/export ****
    * Create_a_book
    * Download_as_PDF
    * Printable_version
**** Languages ****
    * Ø§ÙØ¹Ø±Ø¨ÙØ©
    * Deutsch
    * EspaÃ±ol
    * FranÃ§ais
    * íêµ­ì´
    * Italiano
    * ×¢××¨××ª
    * Nederlands
    * æ¥æ¬èª
    * Polski
    * PortuguÃªs
    * RomÃ¢nÄ
    * Ð ÑÑÑÐºÐ¸Ð¹
    * Simple_English
    * Suomi
    * à¹à¸à¸¢
    * Ð£ÐºÑÐ°ÑÐ½ÑÑÐºÐ°
    * ä¸­æ
Edit_links
    * This page was last edited on 30 July 2019, at 14:56 (UTC).
    * Text is available under the Creative_Commons_Attribution-ShareAlike
      License; additional terms may apply. By using this site, you agree to the
      Terms_of_Use and Privacy_Policy. WikipediaÂ® is a registered trademark of
      the Wikimedia_Foundation,_Inc., a non-profit organization.
    * Privacy_policy
    * About_Wikipedia
    * Disclaimers
    * Contact_Wikipedia
    * Developers
    * Cookie_statement
    * Mobile_view
    * [Wikimedia_Foundation]
    * [Powered_by_MediaWiki]
