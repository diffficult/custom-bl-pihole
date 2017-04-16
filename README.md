# custom-bl-pihole
Downloading, parsing and adding custom lists to the adlists.list on Pi-hole

I didn't make this, just tweaked it to make it work for me and for any future installation. It's a work in progress.

## Installation

1. Clone repo
2. Create a directory under `/var/www/html/` to place your future host list. For example `lists`
3. Create `adlists.list` on your pi-hole, use `sudo cp /etc/pihole/adlists.default /etc/pihole/adlists.list`
4. Edit the newly created `adlists.list` with your favorite editor and add `http://pi.hole/lists/adblock.hosts` at the end. If you want you can make changes and add other lists by uncommenting the contents. Any changes will be permanent and will not be overwritten on future pi-hole updates.
5. Now to actually add From your repo just run `update_adlists`

## TO-DO
* automate procedure
* clean up scripts

## Thanks to
[**user BozzCL**](https://www.reddit.com/user/BozzCL/) and [**user deleted**](https://www.reddit.com/r/pihole/comments/59t5ft/is_there_a_newbfriendly_complete_guide_for_adding/d9cole7/)
