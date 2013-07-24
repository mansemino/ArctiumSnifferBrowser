Basic and fancy sniffer dump browser, parser & gatherer.

Open your PacketDump.XXXXXX file to inspect, search, export and analize data.
Right click on table data to interact with the packets.
You can export selected data to SQL, CSV or Arctium formats, to manage it as you wish.
It has some other features and maybe it'll improve soon.

Content:

- SnifferBrowser.exe -> Main program
- SnifferBrowser.DAT -> Text file with opcode names, values and types. Don't change it, unless you know you're doing.
- SnifferBrowser.INI -> Position and flag values from program.


It's coded using Embarcadero Studio C++, so probably you'll need some dlls (not included here).
If so, get them from here: http://fbe.am/jue
or here: http://www.4shared.com/zip/Ac3pw7Ab/SnifferBrowser_dlls.html

Updates:
- Added parser for Who & CliWhoRequest opcodes
- Added offsets for connection opcodes (thanks to SgtFatality & Destalker for point out it to me)
- Fixed a crash when exporting address names for IDA
- Updated Opcode Offsets to 5.3.0.17128
- Added parser for CliQuestRequest & QuestResponse, and Gatherer for QuestResponse.
- Added SQL create table for the 3 quest tables.
- Added gatherer for 'gameobject_stats' table (just open your dumps, click 'Tools' -> 'DB Gatherer' and select 'Game Objects stats' from the combobox; Give a name for the file and you're done!
- *new feature* Gatherer module (under tools): You can create Arctium SQL file with data for several tables.
- Changed some icons for popup menus
- Parser for QueryGameObject packets
- Updated Opcode Offsets to 5.3.0.17055 (universal patcher still works! :P)
- Parser for NPCText packets
- Pressing "DEL" key on main table will erase all packets of the same kind as the selected one
- Parser for UpdateObject packets (still to do full MoveObjectUpdate block parser)
- Parser for basic root messages (MoveRoot/MoveUnroot)
- Parser for emote packets (TextEmote, PlayEmote, PlayOneShotAnimKit)
- Parser for some PlaySound packets
- Parser for StandStateUpdate packets
- Parser for some chat messages (ChatMessageAfk/Dnd, Chat, ChatMessageWhisper)
- Basic AuthSession & AddonInfo packet parser
- ESC key can be used now to close the auxiliary windows
- Universal Client patcher for 5.3.x clients (both x32 & x64).
	. Click "Tools -> Client Patcher" and select your client;
	. The browser will autodetect build & architecture and it will create Wow_Patched.exe/Wow-64_Patched.exe to be used with Arctium.

- Get offsets for every opcode (constructor, handler, destructor)
- Export handlers' offsets to rename IDA DB with scripts
