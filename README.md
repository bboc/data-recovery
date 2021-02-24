# data-recovery
Scripts and snippets for working with files extracted from broken storage media 

When restoring data from corrupted media (e.g. with tools like Disk Drill) one typically ends up with thousands of files where only the extension is known. In this repository I collect a number of Python scripts to help make sense of such files by looking at metadata and renaming and sorting files based on that metadata.

## Some Considerations

### Revove Duplicate Files

It is not uncommon for a recovery tool to recover several identical versions of a file, in my tests I found between 5-20% of duplicates, therefore it is a good idea to remove all duplicates before doing anything else.



### Audio Files

If audio files are tagged, advanced recovery tools will already create a filename out of these tags, Sorting a well-tagged collection of audio files can be done manually with [mp3Tag](https://www.mp3tag.de/en/index.html), or automatically with [Bliss](https://www.blisshq.com/). For anything files that lack metadata, [MusicBrainz Picard](https://picard.musicbrainz.org/) is your best bet. 
