## Documentation

- ITS: [primer](_info_/its.primer), [building](kshack/build.doc)
- DDT: [manual](info/ddt.33), [commands](_info_/ddtord.1462),
  [colon commands](_info_/ddt.:cmnds)
- MIDAS: [manual](info/midas.25)
- DUMP: [manual](_info_/dump.info), [format](sysdoc/dump.format)

### DDT cheat sheet for Unix users

The `$` character represents typing ESC.

| Unix command  | DDT command          | Colon command            |
| ------------- | -------------------- | ------------------------ |
| login user   	| user$u               | :login user              |
| logout       	| $$u                  | :logout                  |
| ls           	| ^F                   | :listf                   |
| ls dir       	| dir^F                | :listf dir               |
| ls /         	| ^R m.f.d. (file)     | :print m.f.d. (file)     |
| more file    	| ^R file              | :print file              |
| mkdir dir    	| ^R dir;..new. (udir) | :print dir;..new. (udir) |
| cd dir       	| dir$$s               | :cwd dir                 |
| cp f1 f2     	| $^R f1,f2            | :copy f1,f2              |
| rm file      	| ^O file              | :delete file             |
| ln f1 f2     	| $^O f1,f2            | :link f1,f2              |
| mv f1 f2     	| $$^O f1,f2           | :rename f1,f2            |
| mv file dir  	|                      | :move file,dir           |
| ps           	| $$v                  | :listj                   |
| killall -9 id	| id$j  $^X            | :job id  :kill           |