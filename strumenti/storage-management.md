---
description: How we manage the overwhelming amount of Scambi Festival’s media
---

# 💾 Storage management

{% hint style="danger" %}
### Be careful❗️

The following process is cumbersome and quite stressful by itself, but it can easily turn into a nightmare if the following precautions are not followed:

* Ensuring that date, time and time zone are **correct** and **consistent** across all cameras
* Store pictures in one folder for each creator
{% endhint %}

### digiKam

To manage and store each event’s pictures, we use [digiKam](https://digikam.org), a powerful and cool open source software specifically crefted for this purpose.

1. Ensure pictures’ metadata correctness (see warning above)
2. Rename pictures according to their date, stored into the EXIF metadata, using the following format: `[date:yyyy.MM.dd-HH.mm.ss]{unique}`
3. Ensure all files are in JPG format
4. Assign author and copyright in pictures’ metadata
   1. apply general basic copyright settings
   2. apply author-specific copyright settings
   3. Create a tag for each author and assign it to their pictures, in order to make filtering and sorting easier
5. Sort images in albums according to their topic/sub-event
6. Select and edit photos
7. Batch rename according to the following format: `[date:yyyy.MM.dd-HH.mm.ss]{unique} [dir], Scambi Festival`. Such format means pictures’ name contain the name of their belonging album, hence the name of the activity they are related to.
8. Check geotagging inside pictures’ metadata
9. Create/set/assign location tags
10. People recognition
    1. People’s face detection
    2. People’s face recognition
11. In order to upload the pictures in batch to the Internet Archive, all media and their metadata should be parsed in a CSV file. To do this, let’s use digiKam’s “Batch Queue Manager” and use the “custom shell script” tool, with this input: `echo "\"$INPUT\",$COLORLABEL,$TAGSPATH" >> ~/Desktop/ia-scambi.csv`

### Internet Archive

In order to make Internet Archive backups actually useful, a lot of metadata should be added to each item being uploaded, so that—thanks to the powerful and clever IA search queries’ features—finding pictures and videos about what you are looking for is quick and simple.

Fill the information according to [this reference CSV file](https://x.scambi.org/scambi-archive.org-reference.csv).

* ARCHIVE.ORG
* TOSAVE
* NOT\_COMPLETE
