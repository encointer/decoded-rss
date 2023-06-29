# feed
A GH page for rss feed of meetup times and community messages.

## Community Message Format

```json
   {
        "id": "1",
        "title": "Anmelden für Versammlung",
        "content": "Heute ist die letzte Möglichkeit dich für die kommende Versammlung anzumelden um dein Gemeinschaftseinkommen abzuholen. Diese findet schon übermorgen Mittag statt.",
        "showAt": "2022-12-07T11:30:00.00+00:00"
    }
```

### Hints
Some JSON libraries do not allow dangling commas after the last entry in the list, or map. So this should be prevented.

## Appcast

Appcast is used by the *Upgrader* to download app details. The appcast follows the structure defined by the [Sparkle](https://sparkle-project.org/)  framework. An appcast is essentially an RSS feed with a single channel containing a collection of items, each representing a different app version. The appcast provides the necessary information for the upgrader to determine when an upgrade should be recommended.


## Announcements

The Announcements folder within the `dev` directory contains subfolders: *global*,  *Leo community* and *GBD community*. These folders store announcements in English and German languages.

Each announcement includes the following information in JSON format:

*Community Identifier*: Identifies the specific community.\
*Title*: Describes the main subject of the announcement.\
*Publisher SVG*: Provides a link to the publisher's SVG image.\
*Content*: Contains the detailed message of the announcement.\
*Publish Date*: Indicates the date and time when the announcement was published.

### Announcement Format

```json
   {
      "communityIdentifier": "u0qj944rhWE",
        "title": "Leu Day on June 17th",
        "publisherSVG": "https://encointer.github.io/feed/dev/announcements/community_leader_icons/communnity_leader_gesa.png",
        "content": "We will be at L200 on Langstrasse from 12:15 for Leu Lunch. At 12:50 you can move into Leu together again, at the meetings: Guarantee your friends & colleagues access to the community income by giving them a leap of faith. You can find all the information on the website.",
        "publishDate": "2023-06-15T11:30:00.00+00:00",
        "isFavorite": true,
        "countFavorite": 2  
    }
```


The **announcements** serve as important updates and notifications related to the community, such as new acceptance points, upcoming events, and other relevant information.
