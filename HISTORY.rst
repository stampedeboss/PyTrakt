Release History
^^^^^^^^^^^^^^^
2.8.1 (2018-08-09)
++++++++++++++++++

* Fix bug loading stored credentials for PIN auth (#84)
* Fix an issue with the formatting of now() timestamps on the 10th of the month

2.8.0 (2018-02-25)
++++++++++++++++++

* Add support for device authentication (#81)

2.7.3 (2016-11-5)
+++++++++++++++++

* Fix a bug with comment instance creation (#73)

2.7.2 (2016-07-11)
++++++++++++++++++

* Properly export module contents across `trakt` module (#70)

2.7.1 (2016-07-09)
++++++++++++++++++

* Added `datetime` representation of episode first_aired date

2.7.0 (2016-06-05)
++++++++++++++++++

* Add Movie and TV credit accessors to the Person class

2.6.0 (2016-06-04)
++++++++++++++++++

* Add optional year to movie search parameters @justlaputa (#67)
* Add optional year to show, and episode searches
* Add convenience Person.search class method

2.5.3 (2016-06-02)
++++++++++++++++++

* Fix missing episode ids returned from calendar @anongit (#66)

2.5.2 (2016-05-29)
++++++++++++++++++

* Fix logic in _bootstrapped function @permster (#65)

2.5.1 (2016-05-15)
++++++++++++++++++

* Fix TVShow id attributes @TheJake123 (#64)

2.5.0 (2016-05-09)
++++++++++++++++++

* Add support for enumerate list items (#63)

2.4.6 (2016-05-01)
++++++++++++++++++

* Fix adding to watchlists (#59)

2.4.5 (2016-03-20)
++++++++++++++++++

* Add `six` support for cleaner 2-3 compatibility
* General code cleanup and style improvements

2.4.4 (2016-03-19)
++++++++++++++++++

* Update `slugify` function to better match trakt slugs (#51)

2.4.3 (2016-03-12)
++++++++++++++++++

* Python Style Fixes (per flake8)
* Added mocked unit level tests to ensure API responses are handled properly
* Miscellaneous bug fixes and improvements

2.4.2 (2016-03-05)
++++++++++++++++++

* Fix authentication issue pointed out by @BrendanBall (#48)

2.4.1 (2016-02-20)
++++++++++++++++++

* Fixed user list retrieval @permster (#42)
* Fixed return from generator py 2.x bug (#45)

2.4.0 (2016-02-13)
++++++++++++++++++

* Cleaned up some ugliness in the auth workflows
* User GET's now actually fetch User data from trakt
* User.watching no longer raises an exception if a user isn't watching anything (#40)
* HTTP 204 responses now return None for more obvious error handling

2.3.0 (2016-02-12)
++++++++++++++++++

* Expose documented vars, fix watching query (#39)
* Add easier customization for PIN Authentication url (#38)

2.2.5 (2015-09-29)
++++++++++++++++++

* Added `User.watchlist_movies` and `User.watchlist_shows` properties to the `trake.users.User` class. Thanks @a904guy! (#32)

2.2.4 (2015-09-25)
++++++++++++++++++

* Fix a bug with authentication prompts on Python 2.x. Thanks @Dreamersoul (#30)

2.2.3 (2015-09-21)
++++++++++++++++++

# Fix a bug with loading calendars of `TVEpisode` objects. Thanks @Dreamersoul (#28)
# Fix a bug with `TVEpisode.__str__` (and some others) not properly escaping non-ascii characters on Python 2.x (#27)

2.2.2 (2015-09-20)
++++++++++++++++++

* Fix a bug loading `trakt.calendar.SeasonCalendar` (#25)
* Added new personalized Calendar classes to `trakt.calendar` module

2.2.1 (2015-09-16)
++++++++++++++++++

* Add default values to non-critical `dict.get` calls (#23)
* Updated some documentation.

2.2.0 (2015-08-23)
++++++++++++++++++

* A TVSeason's `episodes` attribute is now dynamically generated from all episodes in that season
* `sync.rate` and `sync.add_to_history` now properly make valid requests (#21)
* Note: `sync.add_to_history`'s `watched_at` argument is now expected to be a datetime object, in order to match `sync.rate`

2.1.0 (2015-07-19)
++++++++++++++++++

* Add Trakt PIN Authentication (#15)

2.0.3 (2015-07-12)
++++++++++++++++++

* Fix BASE_URL to point at correct v2 API (#19)

2.0.2 (2015-04-18)
++++++++++++++++++

* Fix CLIENT_SECRET assignment Bug (#16)

2.0.1 (2015-03-15)
++++++++++++++++++

* Fixed TVEpisode Scrobbling Bug (#13)
* Fixed DEBUG logging messages to properly reflect HTTP Methods
* Added a 400 HTTP Response Code Exception type

2.0.0 (2015-03-04)
++++++++++++++++++

* 2.0 Version bump due to incompatible API changes relating to the location of the trakt api_key attribute
* Add additional debug logging for API responses
* Add tmdb_id to the `TVShow.ids` attribute
* Fixed `trakt.init` to instruct users on how to create a new OAuth application
* * Fixed `TVSeason.to_json` to return accurately scoped season information
* Updated documentation on APIv2's Authentication patterns

1.0.3 (2015-02-28)
++++++++++++++++++

* Fixed a bug with `First Aired Date` datetime parsing

1.0.2 (2015-02-17)
++++++++++++++++++

* Fixes Generator issue detailed in #7
* Fixes Python 2x Unicode bug

1.0.1 (2015-02-15)
++++++++++++++++++

* PyTrakt now utilizes Trakt's new API 2.0
* API Keys can now obtained via the `trakt.init` function
* Note: POSTS have been hit or miss, but get's all appear to be working

0.3.6 (2015-01-15)
++++++++++++++++++

* Bug fix for the failure to process JSON API responses

0.3.4 (2014-08-12)
++++++++++++++++++

* Merged @stampedeboss changes from PR #1
* Some small stylistic changes for consistency

0.3.3 (2014-07-04)
++++++++++++++++++

* trakt.tv.TVShow improvements/changes
* Misc bug fixes in trakt.tv
* Import enhancements in trakt.movies
* Added community module
* Fixed/updated documentation


0.3.0 (2014-06-19)
++++++++++++++++++

* Initial Release
