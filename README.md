# spotify-playlist-archive [![Build Status](https://travis-ci.com/mackorone/spotify-playlist-archive.svg?branch=master)](https://travis-ci.com/mackorone/spotify-playlist-archive)

> Daily snapshots of public Spotify playlists

Spotify's playlists are great. I like that they're updated once in a while -
change is good! I don't like, however, that it's impossible to see older
versions. How am I supposed to remember the name of that song I really liked?
Apparently, I'm not alone: see
[here](https://community.spotify.com/t5/Content-Questions/View-previous-versions-of-playlists/td-p/4400750),
[here](https://community.spotify.com/t5/Accounts/A-playlist-was-modified-Can-I-get-the-old-songs-back/td-p/1001889),
[here](https://community.spotify.com/t5/Content-Questions/Seeing-an-old-version-of-a-playlist/td-p/1318739),
[here](https://community.spotify.com/t5/Other-Partners-Web-Player-etc/Playlists-Is-there-any-way-to-recover-previous-versions-of-a/td-p/4726831),
[here](https://community.spotify.com/t5/Desktop-Mac/Find-Songs-of-old-versions-of-Spotify-Playlists/td-p/998504),
[here](https://community.spotify.com/t5/Closed-Ideas/Playlist-Versioning-History/idi-p/1133819),
[here](https://community.spotify.com/t5/Closed-Ideas/Playlist-History-Versioning/idi-p/1346418),
[here](https://community.spotify.com/t5/Closed-Ideas/Playlists-Playlist-History/idi-p/1816799),
and [here](https://community.spotify.com/t5/Live-Ideas/Playlists-Edit-History/idi-p/4573743).
Since Spotify won't take snapshots of our favorite playlists, let's do it ourselves!

## Quick start

1. To view the current version of a playlist, click on its name below
1. To see all songs that ever belonged to a playlist, click "cumulative"
1. To determine which songs were added or removed from a playlist, click "githistory"
1. To add a playlist to the archive, simply `touch playlists/plain/<playlist_id>` and make a pull request

## How it works

This reposity contains a script for scraping Spotify playlists and publishing
them back to the repo. The script is run daily via
[Travis CI](https://travis-ci.com/mackorone/spotify-playlist-archive)
(free for public GitHub repos). It's also run after every commit, which means
that playlists get regenerated whenever the scraping or formatting logic
changes, or when new playlists are added - cool!

The script determines which playlists to scrape by looking at the file names in
`playlists/plain`. Anything that's not a valid playlist ID gets removed. Files
that *are* a valid playlist IDs get regenerated: a pretty version of each
playlist gets dumped in `playlists/pretty`, new tracks are added to the
files in `playlists/cumulative`, and a plaintext version of each playlist is
written back to `playlists/plain`. The plain version is sorted alphabetically,
rather than by track number, so that it only changes when tracks are added or
removed, making [Git History](https://githistory.xyz/) a nice way to visualize
how the playlist evolves over time.

The list below is autogenerated.

## Playlists

- [A.M. Commute](https://github.com/mackorone/spotify-playlist-archive/blob/master/playlists/pretty/A.M.%20Commute.md)
- [Acoustic Hits: Oldies but Goodies](https://github.com/mackorone/spotify-playlist-archive/blob/master/playlists/pretty/Acoustic%20Hits:%20Oldies%20but%20Goodies.md)
- [Acoustic Love](https://github.com/mackorone/spotify-playlist-archive/blob/master/playlists/pretty/Acoustic%20Love.md)
- [All New Indie](https://github.com/mackorone/spotify-playlist-archive/blob/master/playlists/pretty/All%20New%20Indie.md)
- [All Out 00s](https://github.com/mackorone/spotify-playlist-archive/blob/master/playlists/pretty/All%20Out%2000s.md)
- [All Out 10s](https://github.com/mackorone/spotify-playlist-archive/blob/master/playlists/pretty/All%20Out%2010s.md)
- [All Out 60s](https://github.com/mackorone/spotify-playlist-archive/blob/master/playlists/pretty/All%20Out%2060s.md)
- [All Out 70s](https://github.com/mackorone/spotify-playlist-archive/blob/master/playlists/pretty/All%20Out%2070s.md)
- [All Out 80s](https://github.com/mackorone/spotify-playlist-archive/blob/master/playlists/pretty/All%20Out%2080s.md)
- [All Out 90s](https://github.com/mackorone/spotify-playlist-archive/blob/master/playlists/pretty/All%20Out%2090s.md)
- [All The Feels](https://github.com/mackorone/spotify-playlist-archive/blob/master/playlists/pretty/All%20The%20Feels.md)
- [Always Perfect](https://github.com/mackorone/spotify-playlist-archive/blob/master/playlists/pretty/Always%20Perfect.md)
- [Ambient Relaxation](https://github.com/mackorone/spotify-playlist-archive/blob/master/playlists/pretty/Ambient%20Relaxation.md)
- [Barack Obama's 2019 Summer Playlist](https://github.com/mackorone/spotify-playlist-archive/blob/master/playlists/pretty/Barack%20Obama's%202019%20Summer%20Playlist.md)
- [Beast Mode](https://github.com/mackorone/spotify-playlist-archive/blob/master/playlists/pretty/Beast%20Mode.md)
- [Beats to think to](https://github.com/mackorone/spotify-playlist-archive/blob/master/playlists/pretty/Beats%20to%20think%20to.md)
- [Bedroom Pop](https://github.com/mackorone/spotify-playlist-archive/blob/master/playlists/pretty/Bedroom%20Pop.md)
- [Binaural Beats: Focus](https://github.com/mackorone/spotify-playlist-archive/blob/master/playlists/pretty/Binaural%20Beats:%20Focus.md)
- [Brain Food](https://github.com/mackorone/spotify-playlist-archive/blob/master/playlists/pretty/Brain%20Food.md)
- [Butter](https://github.com/mackorone/spotify-playlist-archive/blob/master/playlists/pretty/Butter.md)
- [Carry Me Away Radio](https://github.com/mackorone/spotify-playlist-archive/blob/master/playlists/pretty/Carry%20Me%20Away%20Radio.md)
- [Chill Hits](https://github.com/mackorone/spotify-playlist-archive/blob/master/playlists/pretty/Chill%20Hits.md)
- [Chill Tracks](https://github.com/mackorone/spotify-playlist-archive/blob/master/playlists/pretty/Chill%20Tracks.md)
- [chill\DnB](https://github.com/mackorone/spotify-playlist-archive/blob/master/playlists/pretty/chill\DnB.md)
- [Chilled R&B](https://github.com/mackorone/spotify-playlist-archive/blob/master/playlists/pretty/Chilled%20R&B.md)
- [Chillin' on a Dirt Road](https://github.com/mackorone/spotify-playlist-archive/blob/master/playlists/pretty/Chillin'%20on%20a%20Dirt%20Road.md)
- [Confidence Boost](https://github.com/mackorone/spotify-playlist-archive/blob/master/playlists/pretty/Confidence%20Boost.md)
- [Dance Party](https://github.com/mackorone/spotify-playlist-archive/blob/master/playlists/pretty/Dance%20Party.md)
- [Deep Focus](https://github.com/mackorone/spotify-playlist-archive/blob/master/playlists/pretty/Deep%20Focus.md)
- [Digster HITS - Best of 2013](https://github.com/mackorone/spotify-playlist-archive/blob/master/playlists/pretty/Digster%20HITS%20-%20Best%20of%202013.md)
- [Disco Forever](https://github.com/mackorone/spotify-playlist-archive/blob/master/playlists/pretty/Disco%20Forever.md)
- [Dreampop](https://github.com/mackorone/spotify-playlist-archive/blob/master/playlists/pretty/Dreampop.md)
- [EDM](https://github.com/mackorone/spotify-playlist-archive/blob/master/playlists/pretty/EDM.md)
- [Energy Boost](https://github.com/mackorone/spotify-playlist-archive/blob/master/playlists/pretty/Energy%20Boost.md)
- [Epic Gaming](https://github.com/mackorone/spotify-playlist-archive/blob/master/playlists/pretty/Epic%20Gaming.md)
- [Feel Good Friday](https://github.com/mackorone/spotify-playlist-archive/blob/master/playlists/pretty/Feel%20Good%20Friday.md)
- [Good Vibes](https://github.com/mackorone/spotify-playlist-archive/blob/master/playlists/pretty/Good%20Vibes.md)
- [Happy Hits!](https://github.com/mackorone/spotify-playlist-archive/blob/master/playlists/pretty/Happy%20Hits!.md)
- [Happy Pop](https://github.com/mackorone/spotify-playlist-archive/blob/master/playlists/pretty/Happy%20Pop.md)
- [Have a Great Day!](https://github.com/mackorone/spotify-playlist-archive/blob/master/playlists/pretty/Have%20a%20Great%20Day!.md)
- [Heart Beats](https://github.com/mackorone/spotify-playlist-archive/blob/master/playlists/pretty/Heart%20Beats.md)
- [Hot Country](https://github.com/mackorone/spotify-playlist-archive/blob/master/playlists/pretty/Hot%20Country.md)
- [Jazz Vibes](https://github.com/mackorone/spotify-playlist-archive/blob/master/playlists/pretty/Jazz%20Vibes.md)
- [Jazzy Romance](https://github.com/mackorone/spotify-playlist-archive/blob/master/playlists/pretty/Jazzy%20Romance.md)
- [Just Good Music](https://github.com/mackorone/spotify-playlist-archive/blob/master/playlists/pretty/Just%20Good%20Music.md)
- [Late Night Jazz](https://github.com/mackorone/spotify-playlist-archive/blob/master/playlists/pretty/Late%20Night%20Jazz.md)
- [License To Chill](https://github.com/mackorone/spotify-playlist-archive/blob/master/playlists/pretty/License%20To%20Chill.md)
- [Lo-Fi Beats](https://github.com/mackorone/spotify-playlist-archive/blob/master/playlists/pretty/Lo-Fi%20Beats.md)
- [Lorem](https://github.com/mackorone/spotify-playlist-archive/blob/master/playlists/pretty/Lorem.md)
- [Lounge - Soft House](https://github.com/mackorone/spotify-playlist-archive/blob/master/playlists/pretty/Lounge%20-%20Soft%20House.md)
- [Love Pop](https://github.com/mackorone/spotify-playlist-archive/blob/master/playlists/pretty/Love%20Pop.md)
- [Low Key Pop](https://github.com/mackorone/spotify-playlist-archive/blob/master/playlists/pretty/Low%20Key%20Pop.md)
- [Lowkey Tech](https://github.com/mackorone/spotify-playlist-archive/blob/master/playlists/pretty/Lowkey%20Tech.md)
- [Mellow Beats](https://github.com/mackorone/spotify-playlist-archive/blob/master/playlists/pretty/Mellow%20Beats.md)
- [Mellow Classics](https://github.com/mackorone/spotify-playlist-archive/blob/master/playlists/pretty/Mellow%20Classics.md)
- [Modern Soft Pop](https://github.com/mackorone/spotify-playlist-archive/blob/master/playlists/pretty/Modern%20Soft%20Pop.md)
- [Mood Booster](https://github.com/mackorone/spotify-playlist-archive/blob/master/playlists/pretty/Mood%20Booster.md)
- [Morning Acoustic](https://github.com/mackorone/spotify-playlist-archive/blob/master/playlists/pretty/Morning%20Acoustic.md)
- [Morning Coffee - Wake Up](https://github.com/mackorone/spotify-playlist-archive/blob/master/playlists/pretty/Morning%20Coffee%20-%20Wake%20Up.md)
- [Morning Motivation](https://github.com/mackorone/spotify-playlist-archive/blob/master/playlists/pretty/Morning%20Motivation.md)
- [New Boots](https://github.com/mackorone/spotify-playlist-archive/blob/master/playlists/pretty/New%20Boots.md)
- [New Music Friday Indonesia](https://github.com/mackorone/spotify-playlist-archive/blob/master/playlists/pretty/New%20Music%20Friday%20Indonesia.md)
- [New Music Friday](https://github.com/mackorone/spotify-playlist-archive/blob/master/playlists/pretty/New%20Music%20Friday.md)
- [Orgánica](https://github.com/mackorone/spotify-playlist-archive/blob/master/playlists/pretty/Orgánica.md)
- [Peaceful Piano](https://github.com/mackorone/spotify-playlist-archive/blob/master/playlists/pretty/Peaceful%20Piano.md)
- [Peaceful Pop](https://github.com/mackorone/spotify-playlist-archive/blob/master/playlists/pretty/Peaceful%20Pop.md)
- [Piano in the Background](https://github.com/mackorone/spotify-playlist-archive/blob/master/playlists/pretty/Piano%20in%20the%20Background.md)
- [POLLEN](https://github.com/mackorone/spotify-playlist-archive/blob/master/playlists/pretty/POLLEN.md)
- [Rap UK](https://github.com/mackorone/spotify-playlist-archive/blob/master/playlists/pretty/Rap%20UK.md)
- [RapCaviar](https://github.com/mackorone/spotify-playlist-archive/blob/master/playlists/pretty/RapCaviar.md)
- [Relax & Unwind](https://github.com/mackorone/spotify-playlist-archive/blob/master/playlists/pretty/Relax%20&%20Unwind.md)
- [Rocket League Game Soundtrack (Complete)](https://github.com/mackorone/spotify-playlist-archive/blob/master/playlists/pretty/Rocket%20League%20Game%20Soundtrack%20(Complete).md)
- [Rocket League Soundtrack (Complete OST)](https://github.com/mackorone/spotify-playlist-archive/blob/master/playlists/pretty/Rocket%20League%20Soundtrack%20(Complete%20OST).md)
- [Sad Bops](https://github.com/mackorone/spotify-playlist-archive/blob/master/playlists/pretty/Sad%20Bops.md)
- [Sad Indie](https://github.com/mackorone/spotify-playlist-archive/blob/master/playlists/pretty/Sad%20Indie.md)
- [Skatepark Punks](https://github.com/mackorone/spotify-playlist-archive/blob/master/playlists/pretty/Skatepark%20Punks.md)
- [Soft Pop Hits](https://github.com/mackorone/spotify-playlist-archive/blob/master/playlists/pretty/Soft%20Pop%20Hits.md)
- [Songs to Sing in the Car](https://github.com/mackorone/spotify-playlist-archive/blob/master/playlists/pretty/Songs%20to%20Sing%20in%20the%20Car.md)
- [Songs to Sing in the Shower](https://github.com/mackorone/spotify-playlist-archive/blob/master/playlists/pretty/Songs%20to%20Sing%20in%20the%20Shower.md)
- [Soul 'n' the City](https://github.com/mackorone/spotify-playlist-archive/blob/master/playlists/pretty/Soul%20'n'%20the%20City.md)
- [Summer Days](https://github.com/mackorone/spotify-playlist-archive/blob/master/playlists/pretty/Summer%20Days.md)
- [Summer Hits](https://github.com/mackorone/spotify-playlist-archive/blob/master/playlists/pretty/Summer%20Hits.md)
- [Summer Party](https://github.com/mackorone/spotify-playlist-archive/blob/master/playlists/pretty/Summer%20Party.md)
- [Sunny Day](https://github.com/mackorone/spotify-playlist-archive/blob/master/playlists/pretty/Sunny%20Day.md)
- [Techno Bunker](https://github.com/mackorone/spotify-playlist-archive/blob/master/playlists/pretty/Techno%20Bunker.md)
- [The Sound of Medieval](https://github.com/mackorone/spotify-playlist-archive/blob/master/playlists/pretty/The%20Sound%20of%20Medieval.md)
- [Today's Top Hits](https://github.com/mackorone/spotify-playlist-archive/blob/master/playlists/pretty/Today's%20Top%20Hits.md)
- [Totally Stress Free](https://github.com/mackorone/spotify-playlist-archive/blob/master/playlists/pretty/Totally%20Stress%20Free.md)
- [Twenty One Pilots Radio](https://github.com/mackorone/spotify-playlist-archive/blob/master/playlists/pretty/Twenty%20One%20Pilots%20Radio.md)
- [Ultimate Indie](https://github.com/mackorone/spotify-playlist-archive/blob/master/playlists/pretty/Ultimate%20Indie.md)
- [United States Top 50](https://github.com/mackorone/spotify-playlist-archive/blob/master/playlists/pretty/United%20States%20Top%2050.md)
- [Unwind 00s](https://github.com/mackorone/spotify-playlist-archive/blob/master/playlists/pretty/Unwind%2000s.md)
- [Warm Fuzzy Feeling](https://github.com/mackorone/spotify-playlist-archive/blob/master/playlists/pretty/Warm%20Fuzzy%20Feeling.md)
- [Wild + Free](https://github.com/mackorone/spotify-playlist-archive/blob/master/playlists/pretty/Wild%20+%20Free.md)
- [Women of Pop](https://github.com/mackorone/spotify-playlist-archive/blob/master/playlists/pretty/Women%20of%20Pop.md)
- [You & Me](https://github.com/mackorone/spotify-playlist-archive/blob/master/playlists/pretty/You%20&%20Me.md)
- [Young & Free](https://github.com/mackorone/spotify-playlist-archive/blob/master/playlists/pretty/Young%20&%20Free.md)
- [Young, Wild & Free](https://github.com/mackorone/spotify-playlist-archive/blob/master/playlists/pretty/Young,%20Wild%20&%20Free.md)
- [Your Favorite Coffeehouse](https://github.com/mackorone/spotify-playlist-archive/blob/master/playlists/pretty/Your%20Favorite%20Coffeehouse.md)
