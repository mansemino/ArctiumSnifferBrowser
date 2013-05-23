Basic and rough sniffer dump browser.

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

Updated:
- Get offsets for every opcode (constructor, handler, destructor)
- Export handlers' offsets to rename IDA DB with scripts
- Calculator por CMSGS GUID indexes