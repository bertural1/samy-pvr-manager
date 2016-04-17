# Samsung's INF file structure #

The following table describes the inf-format of pvr recordings.
The length is 1356 bytes for default/old files and 7464 bytes for extended/new files.

# Structure #

| **Field** | **Offset** | **Comment** |
|:----------|:-----------|:------------|
| CHANNELNAME | 0x0000     |             |
| [RAWTITLE](INF_RAWTITLE.md) | 0x0100     | I've never seen this on tv |
| CHANNELNUMBER | 0x0200     |             |
| X0300     | 0x0300     |             |
| RECTIME   | 0x0304     | start time  |
| DURATION  | 0x0308     | duration    |
| X0314     | 0x0314     |             |
| RECTITLE  | 0x0318     | title       |
| X0530     | 0x0530     | 0x08 or 0x2A |
| LANGCODE  | 0x0534     |             |
| X0544     | 0x0544     | 02 or 04    |
| X054C     | 0x054C     | 02 or 04    |
| X056E     | 0x056E     | 3602 or 00 00 |
| GUIDANCEINFOLENGTH | 0x065C     | Guidance Information string length (0=no guidance info) |
| INFOLENGTH | 0x065E     |             |
| GUIDANCEINFO | 0x0660-0x06F5 | Guidance Information text |
| INFO      | 0x06F6     |             |
| TIMERSTART | 0x18F8     | start time if timer was used |
| TIMEREND  | 0x18FC     | end time if timer was used |
| HD        | 0x1904     | HD flag (1=HD, 0=SD) |
| SUBTITLES | 0x1906     | Subtitles (1=present, 0=absent) |
| TELETEXT  | 0x1908     | Teletext flag (1=present, 0=absent) |
| AUDIODESC | 0x190A     | Audio Description flag (1=present, 0=absent) |
| SUBTITLES4HI | 0x190C     | Subtitles for hearing impaired (1=present, 0=absent) |
| CONTENTLANG | 0x1910     | Language of content (reverse!) |
| CATEGORY  | 0x1B0E     | see [CATIDX](INF_CATIDX.md) |
| ASPECTRATIO | 0x1D0C     | Aspect Ratio (0=1:1, 1=4:3, 2=16:9) |
| IMAGEDEF  | 0x1D10     | Image Definition (0=1080i, 1=1080p, 2=288i, 3=480i, 4=480p, 5=576i, 6=576p, 7=720p) |
| LOCK      | 0x1D14     | (1=locked, 0=unlocked) |
| MINAGE    | 0x1D18     | Minimum Recommended Age (0x01=4 years, 0x02=5 years, 0x03=6 years, and so on up to 0x0F=18 years, or FF=suitable for all or not rated) |
| FAVORITE  | 0x1D1C     | Favourites flags (bits 0-4 for Favourite 1 to 5) (It's not a simple flag!) |
| SPLIT     | 0x1D20     | Split flag (1=no split) |
| [LANGIDX](INF_LANGIDX.md) | 0x1D24     | Index of the Language string in the list of translated strings |
| [CATIDX](INF_CATIDX.md) | 0x1D26     | Index of the category string in the list of translated strings |