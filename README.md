# luus
_LARBS Universal Utility Scripts_

### Features
1. **Speed** - Resource friendly, easily integrated with the command-line, i3wm and ranger.
2. **History** - Both **LUD** and **LUP** are equipped with history files in `~/.lud_history` and `~/.lup_history`, allowing previous files to be viewed/downloaded.
3. **Modularity** - Both **LUD** and **LUP** have `$1` & `$2` for command-line functionality.


## LUD
_(The) LARBS Universal Downloader_

#### Usage
1. Grabs clipboard / `$1`
2. Choose destination / `$2`
3. Choose type of download

## LUP
_(The) LARBS Universal Player_

#### Usage
1. Choose clipboard/destination / `$1`
2. Choose player application / `$2`

| Requirements | Usage |
| :------------- | :------------- |
| [aria2c](https://github.com/aria2/aria2) | Regular Downloader |
| [youtube-dl](https://github.com/ytdl-org/youtube-dl) | Video Downloader |
| [dmenu](https://github.com/LukeSmithxyz/dmenu) | Menu System |
| [xclip](https://github.com/astrand/xclip) | Clipboard |
| [notify-send](https://github.com/vlevit/notify-send.sh) | Notification |

### Integration
#### Ranger
`map dl shell lud "" "%d"`

#### i3wm
`bindsym $foo_command exec --no-startup-id lud`

`bindsym $bar_command exec --no-startup-id lup`

#### Command-line
`lud "https://www.youtube.com/watch?v=DB6UWGeNePk" "~/Videos/"`

`lup "https://www.youtube.com/watch?v=DB6UWGeNePk" "mpv (video)"`
