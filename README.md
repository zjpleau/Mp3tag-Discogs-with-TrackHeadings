# Mp3tag-Discogs-with-TrackHeadings

A custom Mp3tag tag-source that:

- Fetches release metadata via the Discogs API  
- Splits out per-track section headings (the “disc titles” or other grouping headings)  
- Writes them into a `%TRACKHEADING%` tag field alongside the normal fields  

---

## Installation

1. **Download** or **clone** this repository:

   ```bash
   git clone https://github.com/zjpleau/Mp3tag-Discogs-with-TrackHeadings.git
   ```

2. **Copy** the script into your Mp3tag sources folder:

   - Windows:
     ```
     %APPDATA%\Mp3tag\data\sources
     ```
   - macOS (Wine):
     ```
     ~/.wine/drive_c/users/<you>/Application Data/Mp3tag/data/sources/
     ```

3. Restart Mp3tag.

---

## Usage

1. In Mp3tag select the files you want to tag.  
2. Go to **Tag Sources → Discogs Release ID (Track Headings)**.  
3. Enter the Discogs **Release ID** (e.g. `33197211`) and click **OK**.  
4. In the preview screen you’ll see:

   - **Metadata Album**: ALBUM, ALBUMARTIST, YEAR, GENRE, STYLE, LABEL, CATALOGID, DISCOGS_RELEASE_ID  
   - **Tracks** grid: TRACK, DISCNUMBER, TITLE, ARTIST, LENGTH, **TRACKHEADING**  

5. Check or uncheck fields as needed, then click **OK** to write tags.

---

## License

MIT © [zjpleau](https://github.com/zjpleau)

