---
description: Uploading to and using the Internet Archive for Scambi Festival media
---

# 🏛 Internet Archive

{% hint style="info" %}
Please, do <mark style="background-color:yellow;">read the</mark> [<mark style="background-color:yellow;">Storage management</mark>](./) <mark style="background-color:yellow;">page first</mark>!
{% endhint %}

While Cubbit is perfect to have a redundant and reliable backup of heavy files, it lacks the possibility of easily previewing and sorting them, as well as properly applying filters while searching.

Luckily enough, the [Internet Archive](https://archive.org) perfectly solves this problem: it allows us to upload an unlimited amount of media of any size, as long as it is public domain.

In order to make Internet Archive backups actually useful, a lot of metadata should be added to each item being uploaded, so that finding pictures and videos about what you are looking for is quick and simple.

Fill the information according to [this reference CSV file](https://x.scambi.org/scambi-archive.org-reference.csv).

### Fields

* **``**[**`identifier`**](https://archive.org/developers/metadata-schema/#identifier): unique identifier that will determine the URL of the item (e.g. identifier: `scambi2022-345`, URL: [`https://archive.org/details/scambi2022-345`](https://archive.org/details/scambi2022-345))
* **``**[**`mediatype`**](https://archive.org/developers/metadata-schema/#mediatype): what is this? Usually `image` or `video`
* **``**[**`collection`**](https://archive.org/developers/metadata-schema/#collection): the collection this item belongs to. So far, Scambi Festival has: [`scambi-2021`](https://archive.org/details/scambi-2021), [`scambi-presenta-2022`](https://archive.org/details/scambi-presenta-2022), and [`scambi-2022`](https://archive.org/details/scambi-2022)``
* **`file`**: the local path the CLI interface should retrieve the file from
* **``**[**`title`**](https://archive.org/developers/metadata-schema/#title): item title
* **``**[**`date`**](https://archive.org/developers/metadata-schema/#date): item original date
* **``**[**`creator`**](https://archive.org/developers/metadata-schema/#creator): if the author is known, use their name; otherwise, write `Scambi Festival`
* **``**[**`coverage`**](https://archive.org/developers/metadata-schema/#coverage): the item location in ISO standard format (for us it is `IT-IM`)
* **``**[**`licenseurl`**](https://archive.org/developers/metadata-schema/#licenseurl): the URL of the license for the image. If it is a graphics or something created from scratch, we use [`https://creativecommons.org/licenses/by-nd/1.0/`](https://creativecommons.org/licenses/by-nd/1.0/), but usually we go for [`https://creativecommons.org/licenses/by-sa/4.0/`](https://creativecommons.org/licenses/by-sa/4.0/)``

#### Custom

To improve filtering specifically related to Scambi Festival stuff, here are some extra custom metadata fields. Most of the same information should be added to the subjects, but it is useful to have dedicated fields anyways.

* **`what`**: kind of activity; for example, it could be `Backstage`, `Allestimento collettivo`, `Lab`, `Pinolo`, Dissolvenze, `SquiLibristi`…
* **`pinolo`**: if it is a [Pinolo](../../format/pinoli.md), what Pinolo is it?
* **`lab`**: if it is a [Lab](../../format/lab.md), what Lab is it?
* **`location_tag`**: name of the location; for example, it could be `Piazza Santa Brigida`, `Piazzetta dei Ferri`, `Il Buco`, `La Ciotola`, `Via Tapoletti`… a complete list of the locations is [in this table](https://pino.scambi.org/database/61/table/322), on [Pino](../pino.md)
* **`relations`**: name of the entity hosting this activity, consistent with the Relation database on Pino
* **`rating`**:
* **`cubbit_path`**:

### Searching

Since all media uploaded to the Internet Archive beefed up with a comprehensive amount of metadata, it becomes easy and straightforward—even fun—to [search](https://archive.org/search.php) and filter the results.\
Use [**advanced search**](https://archive.org/advancedsearch.php) to add easily filters and conditions.

Here are some useful resources to master this extremely useful tool.

* [Search — a basic guide](https://help.archive.org/help/search-a-basic-guide/)

#### Examples

* [Scambi Festival 2022 pictures rated “Best of”](https://archive.org/search.php?query=collection%3A%28scambi-2022%29%20AND%20rating%3A%28Best%20of%29) — search query: `collection:(scambi-2022) AND rating:(Best of)`
* All of Scambi Festival’s images taken in Piazza Santa Brigida (during any edition) — search query: `subject:(Scambi Festival) AND location_tag:(Piazza Santa Brigida)`
* Best of Scambi Festival 2022 Pictures taken in Piazza Cassini
