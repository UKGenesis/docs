# UK Genesis Podcast - Procedures

These are the steps needed to setup and run a podcast show.

## Setup for Next Show

Schedule: http://gmj.to/ukgschedule

* Create a Hangout On Air under the +UKGenesis account: https://plus.google.com/b/115249804192711751807/hangouts/onair 
	* Title follows the format: “UK Genesis Podcast #17 | With Mike Little
	* Set for Later, at the appropriate date and time (usually 2pm).
	* Use ukgenesis.co.uk Podcast entry content as Google+ Event content, but swap out any markup, use plain text links etc.
	* Once the event is saved, Add a Trailer, and Upload the guest image.
	* Add the Hangout link (plus.google.com/event…) to the Podcast entry.
	* Share the Hangout entry to Public and Genesis Community page, and +1 the event by personal accounts.
* Create new draft Podcast entry on ukgenesis.co.uk website.
	* Start with by selecting New Draft from an existing entry (clone previous entry).
	* Title follows the format: `Mike Little, Episode #17`.
	* Slug should be of the format: `mike-little-episode-17`.
	* Content should include links to guest’s website and Twitter account.
	* Featured Image should be 960 ⨉ 540px, should have a title of the guest name, and a suitable alt value e.g. Headshot of Mike Little.
	* Yoast SEO focus keyword should be their name.
	* Yoast SEO meta title can be left as default.
	* Yoast SEO meta description should start with their name, and summarise what the show topics will be. Use the present tense e.g. “Mike Little chats with us about…”
	* Fill out the Hangout link (created via steps above).
	* Leave YouTube URL blank until pre-show.
	* Adjust the Podcast Sidebar details if necessary.
* Publish Podcast entry, with a timestamp of 2pm, exactly one week before the show starts.
* Promote the ukgenesis.co.uk/podcasts/… URL on Twitter, with guest photo.
* Re-send [Guest Briefing](https://github.com/UKGenesis/docs/blob/master/guest-briefing.md) to guest if needed.

## Pre-Show

* Aim to do pre-show checks at 30 minutes before the start time.
* Set up local environment - backdrop, drink, Twitter / client website / [Questions](https://github.com/UKGenesis/docs/blob/master/guest-briefing.md) etc.
* Go to https://plus.google.com/b/115249804192711751807/+UkgenesisCoUk/posts (ensure the top-right account is UK Genesis), find the relevant event, and click on the event title (just underneath the video preview). Hit Start to start the Hangout on Air (but don’t broadcast).
* Send link of the pop-up Hangout window to guest and co-host via Slack or other IM.
* Get YouTube link (links icon, bottom right), and enter into Podcast entry on ukgenesis.co.uk no earlier than 30 minutes before the start time. This will swap out the guest photo for a video of the live event. Will show as standing by until we start broadcasting.
* Remind guest to setup lower third - their briefing document tells them how to do this.
* Setup tweets for 15 minutes before the show (include guest photo) and 5 minutes into the show.
* Publicise the show in #general channel of genesiswp group on Slack.
* Ensure Hangout view has everyone de-selected, so that it auto-switches to whoever is speaking.

## Post-Show

Some of this can be done before or during the recording.

* Update video details via the Video Manager on YouTube (UKGenesis account).
	* Title and description should already be populated from the Google Event.
		* Tags should be “WordPress (Blogger)” and “Podcast (Website Category)”.
		* Under Advanced Settings, change the following:
		* Caption certification to “This content has never aired on US television”
		* Category to “People and Blogs”
		* Video Location to the city/town where the guest lives
		* Video Language to “English (United Kingdom)”
		* Recording date to the right date (often, Today).
	* Add a Card (Associated Website):
	* Website URL: 
	* Title: “UK Genesis - Genesis Framework community in the UK” (remove the “a “ from the pre-populated value to get within character limit)
	* Call to Action: “Visit ukgenesis.co.uk”
	* Teaser text: “Visit ukgenesis.co.uk”
	* Ensure the card is set to show at the very start of the show (drag along the timeline).
* Once the show appears under the Video Manager -> Videos https://www.youtube.com/my_videos?o=U (it won’t to start with, whilst it’s being processed), then
	* Change the thumbnail, under Info and Settings, to one that shows the a good image of the guest.
	* Add the video to the existing “UK Genesis Podcasts” playlist.
* Change the Topic and Intro in Scheduleto Done.

## Podcast Feed
* From the Video Manager page, download the MP4 of the video.
* Drag into Audacity.
	* Convert to mono (Tracks->Stereo to Mono).
	* If there is any background hum, find a section and apply Noise Removal.
	* Chop out any annoying bits in the introduction - breathing, “er”’s etc. Highlight a section, and either hit delete, or Generate -> Silence.
	* Apply Compressor, to reduce the peaks above a certain point (-12dB is fine).
	* Export as MP3, at 64k constant bit rate, joint stereo. Same as the same slug as their web page e.g. mike-little-episode-17.mp3
* Use Kid3 to edit the ID3v2 tags (adapt for each show):
	* Title: Mike Little, Episode #17
	* Artist: UK Genesis
	* Album: UK Genesis Podcasts
	* Date: 2015 (year only)
	* Track Number: 17
	* Genre: Podcast
	* Publisher: UK Genesis
	* Website: http://ukgenesis.co.uk/podcasts/mike-little-episode-17/
	* Add a 600x600 guest photo
		* Double-click to select type as Artist / Performer and Description as the guest’s name.
* Use PowerPress plugin to upload .mp3 to UKGenesis hosting.
