Basic and fancy sniffer dump browser, parser & gatherer.

Open your PacketDump.XXXXXX file to inspect, search, export and analize data.
Right click on table data to interact with the packets.
You can export selected data to SQL, CSV or Arctium formats, to manage it as you wish.

It has some other features and maybe it'll improve soon:

. You can patch your 5.4.1.x client (any architecture, any build) to use it with Arctium Server
. You can get offsets for CliGet/CliPut handlers
. You can export these offsets to TXT to import from IDA
. All the features for the packets as ever (filtering, searching, exporting, etc.)
. Please, note that offsets are for x86 client and not rebased.

Content:

- SnifferBrowser.exe -> Main program
- SnifferBrowser.DAT -> Text file with opcode names, values and types. Don't change it, unless you know you're doing.
- SnifferBrowser.INI -> Position and flag values from program.

It's coded using Embarcadero Studio C++, so probably you'll need some dlls (not included here).
If so, get them from here: http://fbe.am/jue
or here: http://www.4shared.com/zip/Ac3pw7Ab/SnifferBrowser_dlls.html


Updates:

- Updated to add parsers for several packets (no gatherer yet)
  . ChatMessageAfk, ChatMessageDnd, ChatMessageSay, ChatMessageYell, ChatMessageWhisper, LogXPGain, LogoutResponse, LogoutInstant, MoveUpdate
  . Full handler offsets for 5.4.1.17538
- Updated to support 5.4.1.17538 retail client
  . Parser/Gatherer module disabled atm (I'm updating the structs :P)
  . Same for details on packets: Only RAW data is shown
- Added some opcodes from Arctium Server to SnifferParser.DAT