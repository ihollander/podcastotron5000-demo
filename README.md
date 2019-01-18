# React Podcast Manager

This is a demo of the features for a **React Podcast Manager**, a tool for managing your podcasts subscriptions and listening to your favorite shows. The frontend was built with React/Redux and the backend is a Ruby on Rails API.

Requires [podcastotron5000](https://github.com/ihollander/podcastotron5000) frontend and [podcastotron5000-api](https://github.com/ihollander/podcastotron5000-api) backend.

## Features
1. [Search and subscribe to podcasts](#search-and-subscribe)
2. [Get recent podcast episodes](#find-episodes)
3. [Manage your personal playlist](#manage-your-playlist)
4. [Responsive audio player](#responsive-audio-player)

### Search and Subscribe
Users can find any podcast available on the iTunes store using the search function. Search results and matching terms are cached on the server for fast load times and to limit external API requests. 

![podcast-search](gifs/podcast-search.gif)

Once a user finds a podcast they're interested in, they can subscribe to it to keep track of their favorite podcasts and make sure they get the latest episodes.
![podcast-subscribe](gifs/podcast-subscribe.png)


### Find Episodes
Users can view all episodes for any given podcast on the episode detail page. Episode details are taken from the RSS feed associated with the podcast after fetching the feed URL from the iTunes Search API. Users can also filter episodes by title.

![podcast-detail-view](gifs/podcast-detail-view.gif)

For podcasts the user is subscribed to, they can also view a list of all podcast episodes sorted by most recent. The recent podcasts page utilizes an infinite scrolling feature to prevent overfetching from the API.

![podcast-recent-episodes](gifs/podcast-recent-episodes.gif)

### Manage Your Playlist
Users can add any episode they're interested in listening to to their personal playlist.

![podcast-playlist](gifs/podcast-playlist.gif)

### Responsive Audio Player
The playlist is integreted with a custom responsive audio player with built-in playback controls.

![podcast-audio-controls](gifs/podcast-audio-controls.gif)
