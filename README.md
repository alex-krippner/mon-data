# mon-data

Holds data such as dictionaries for the [Mon](https://github.com/alex-krippner/mon) reading app.

Each release contains the downloadable dictionary packs (`*.db.gz`) and a `catalog.json` that lists them.
The Mon app fetches the `catalog.json` of the latest release.

## Licence and attribution

The data in this repository is licensed under the
[Creative Commons Attribution-ShareAlike 4.0 International licence (CC BY-SA 4.0)](https://creativecommons.org/licenses/by-sa/4.0/).
The full text is in [`LICENSE`](LICENSE).

### JMdict

The Japanese–English and Japanese–German dictionary packs are derived from the
[JMdict](https://www.edrdg.org/jmdict/j_jmdict.html) dictionary file.

- JMdict is the property of the [Electronic Dictionary Research and Development Group](https://www.edrdg.org/)
  (EDRDG) and is used in conformance with the group's
  [licence](https://www.edrdg.org/edrdg/licence.html) (CC BY-SA 4.0).
- The JMdict data was obtained through
  [jmdict-simplified](https://github.com/scriptin/jmdict-simplified), which provides it as JSON.

**Changes made:** the jmdict-simplified JSON was converted into Mon's SQLite pack format and compressed
with gzip. The entries are not otherwise edited.

Each pack's `dictDate` in `catalog.json` and in its file name (`jmdict-<lang>-<dictDate>.db.gz`) is the date
of the JMdict data it was built from. The data is rebuilt and re-released regularly to keep it current.

### Other files

Any other file in this repository that is not dictionary data is covered by the same licence unless it
says otherwise.
