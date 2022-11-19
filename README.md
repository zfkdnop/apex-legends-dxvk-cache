# NOTICE
The author has obsoleted this project
```
I now recommend that people just switch to Proton Experimental and the 
Nvidia Vulkan Beta driver version 515.49.10. This will use the new 
graphics pipeline library support, which eliminates stutter and the need
 for sharing cache files. Note that driver version 515.65 does NOT
 work because it is not the vulkan beta driver branch. People with AMD 
or Intel graphics will need to wait until Mesa adds support for graphics
 pipeline libraries to have the same experience.
```

I personally use [Proton-GE](https://github.com/GloriousEggroll/proton-ge-custom) and it works great.


# apex-legends-dxvk-cache
A compilation of DXVK states pre-cached, for use with Apex Legends on Linux via Steam/Proton. Helps to improve and promote a smooth gaming experience.

The following text is a slightly modified copy from https://www.reddit.com/r/linux_gaming/comments/t5xrho/dxvk_state_cache_for_fixing_stutter_in_apex/

# DXVK state cache for fixing stutter in Apex Legends

People have probably noticed that Apex Legends has a stutter problem. This is caused by shaders needing to be compiled by DXVK at draw time in the game due to differences in how Vulkan and Direct3D 11 work. Other games do not have nearly as many shaders, so it is less of a problem for them.

Overwatch has a similar problem, but the lutris project solved it by distributing a dxvk cache file. Unfortunately, Valve is not distributing dxvk cache files, so we need to do this manually. I had planned to wait another day before posting this, but after seeing someone post "Everyone should install and play a little bit of Apex Legends, even if you are not into that kind of game. Let’s show other devs how many of us are gaming on Linux!", I decided to post a thread with the cache file so people can have a decent experience:

**ORIGINAL LINK** https://cdn.discordapp.com/attachments/483946408676818974/990268358379319366/r5apex.dxvk-cache.zst

*The file found at the link above is the file located in this repository - as of Jun 25, 2022*


The cache is now zstd compressed due to discord's 8MB file size limit being reached. You can use Ark to extract it. Let me know if you have problems decompressing it. I might find alternative hosting if the compression poses a problem.

The standard caveats about downloading files from strangers on the internet apply. If you have shader pre-caching enabled, the file goes in */path/to/steamapps/shadercache/1172470/DXVK_state_cache/r5apex.dxvk-cache*. 
The default location is *~/.local/share/Steam/steamapps/shadercache/1172470/DXVK_state_cache/r5apex.dxvk-cache*. 
If shader pre-caching is disabled, then the file will go in the game directory.

**Note:** My directory is located at /home/user/.steam/debian-installation/steamapps/shadercache/1172470/DXVK_state_cache/r5apex.dxvk-cache (with shader pre-caching enabled).... /home/user/.steam/debian-installation/steamapps/common/Apex\ Legends/r5apex.dxvk-cache (with shader pre-caching disabled)


The current cache file has 42320 entries and more are still being occasionally added. However, people using it report no stutter, even though there is likely to be a small number of missing entries.

I plan to update this post with links to newer cache files. Feel free to send me your cache files. I will merge them into mine to make the cache file I share more complete. Even if you have only played a little bit, there could be shaders that are not in my cache file, so feel free to send those caches to me too. When we finally have a cache with all shaders, the stutter problem should disappear.

Also, for those wondering where the merge tool is, lutris distributes a build of it:

https://lutris.nyc3.cdn.digitaloceanspaces.com/games/overwatch/merge-tool.tar.xz

It is originally from here:

https://github.com/DarkTigrus/dxvk-cache-tool

Note that using feral gamemode in addition to this has made additional improvements in stutter for some people:

https://github.com/FeralInteractive/gamemode

Edit: Someone sent me a cache file that had 265 new entries a few minutes after I posted this. That brings us from 5749 entries to 6014 entries. The link has been updated. :)

Edit: Three people sent me cache files. They collectively added 1426 new entries. This brings us from 6014 entries to 7440 entries.

Edit: I was sent another cache file. It added 2 new entries. That brings us from 7440 entries to 7442 entries. I am now playing games with zero stutter and without any new entries being generated, so my guess is that the cache file is now relatively mature.

Edit: /u/Melon__Bread sent me a new cache file. It added 31 new entries. That brings us from 7442 entries to 7473 entries.

Edit: /u/najodleglejszy sent me a new cache file. It added 82 new entries. That brings us from 7473 entries to 7555 entries.

Edit: I found 2 new entries while testing the cache. That brings us from 7555 entries to 7557 entries. Also, I am still having a stutter-free experience while using the cache file, despite the discovery of a couple new entries.

Edit: I received cache files from /u/PsychologicalLog1090 and 2 others. Collectively, they added 287 entries. That brings up from 7557 entries to 7844 entries.

Edit: I found 3 more new entries while testing the cache. That brings us from 7844 entries to 7847 entries.

Edit: I received another cache file from /u/a9dnsn. This gives us 574 new entries. That brings us from 7847 entries to 8421 entries.

Edit: I found 8 more new entries while testing the cache and someone else sent me 1 more. That brings us from 8421 entries to 8430 entries.

Edit: Four people, including /u/LilCalosis, sent me cache files. They collectively added 450 new entries. This brings us from 8430 entries to 8880 entries. Note that I am only posting names of people who sent them to me via public comments. Those who messaged me privately are kept anonymous unless they tell me otherwise.

Edit: Someone sent me a cache file that had 1 new entry a few minutes after I posted the last update. That brings us from 8880 entries to 8881 entries. The link has been updated. :)

Edit: I found 11 new entries while testing the cache. That brings us from 8881 entries to 8892 entries.

Edit: /u/Flubberding and 2 others sent me cache files that collectively contained 498 new entries. I also found 3 new entries while testing. That brings us from 8892 entries to 9393 entries.

Edit: /u/AnyEntertainment8080, /u/arvind-d, /u/DAVE_nn, /u/yourfavrodney, /u/jumper775, /u/Tiflotin and 2 others sent me cache files that collectively contained 496 new entries. That brings us from 9393 to 9889 entries.

Edit: /u/NineBallAYAYA and /u/najodleglejszy sent me cache files. I also found a few more entries. Collectively, that added 33 entries. That brings us from 9889 to 9922 entries.

Edit: Two people sent me cache files. They collectively added 18 new entries. This brings us from 9922 entries to 9940 entries.

Edit: /u/CaptainKrisss, /u/11986NineBallAYAYA and one more person sent me cache files. They collectively added 679 new entries. This brings us from 9940 entries to 10619 entries

Edit: /u/Nik0ne (twice), /u/Tenshar, /u/a9dnsn and 1 other person sent me cache files. They have collectively added 66 new entries. This brings us from 10619 entries to 10685 entries. I took a break yesterday from doing updates and merged all that I could find. If I missed any submissions, it was not intentional. Please send them to me again. The same goes for other miscellaneous messages.

Edit: As of 03/09/2022: /u/-ThunderFox, /u/EpicCreeper713 and two others sent me cache files. I also found a few entries while testing. Collectively, this added 398 entries. This brings us from 10685 entries to 11083 entries.

Edit: /u/Kitchen-Drop236 sent me a cache file. It contained 533 new entries. That brings us from 11083 to 11616 entries.

Edit: 03/11/2022 update: /u/SneakySnk, /u/K1f0 and one other person sent me a cache file. They collectively added 121 new entries. That brings us from 11616 to 11737 entries.

Edit: 03/12/2022 update: /u/gudhost, /u/EpicCreeper713 and /u/wanna_play_r5 sent me cache files. They collectively added 10 new entries. This brings us from 11737 to 11747 entries.

Edit: 03/14/2022 update: /u/SneakySnk, /u/baryluk and one other person sent me cache files. They collectively added 13 new entries. That brings us from 11747 entries to 11760 entries.

Edit: 03/16/2022 update: Two people sent me cache files. They collectively added 25 new entries. That brings us from 11760 entries to 11785 entries.

Edit: 03/28/2022 update: Five people sent me cache files. I also found 7 new entries while testing. This collectively added 201 new entries. That brings us from 11785 entries to 11986 entries.

Edit: 03/29/2022 update: There is a new Apex Legends map, which has added a fair number of entries. Two people sent me cache files, with one of the files containing entries from the new map. That brings us from 11986 entries to 13658 entries.

Edit: 03/29/2022 update: Three people sent me cache files, which collectively added 1290 new entries. That brings us from 13658 entries to 14948 entries.

Edit: 03/29/2022 update: I did a test game and found 69 new entries. This brings us from 14948 entries to 15017 entries.

Edit: 03/29/2022 update: Six people sent me cache files, which collectively added 1053 new entries. This brings us from 15017 entries to 16070 entries.

Edit: 03/30/2022 update: Six people sent me cache files, which collectively added 1587 entries. This brings us from 16070 entries to 17657 entries.

Edit: 03/30/2022 update: /u/sP6awFXL94V6vH7C sent me a new cache file, which added 488 entries. This brings us from 17657 entries to 18145 entries.

Edit: 03/31/2022 update: 5 people sent me new cache files, which added 388 entries. This brings us from 18145 entries to 18533 entries.

Edit: 04/02/2022 update: 2 people sent me new cache files. We now have 18701 entries.

Edit: 04/16/2022 Update: 4 people sent me new cache files. We now have 19071 entries.

Edit: 04/23/2022 Update: 2 people sent me new cache files. We now have 19278 entries.

Edit: 05/10/2022 Update: New season. 3 people sent me cache files. We now have 23639 entries.

Edit: 05/11/2022 Update: I was sent two cache files. We now have 25805 entries.

Edit: 05/12/2022 Update: I was sent a cache file and also merged the cache file bcook254 has been keeping in github. We now have 28101 entries.

Edit: 05/13/2022 Update: I was sent a cache file and also merged the cache file bcook254 has been keeping in github. We now have 28206 entries.

Edit: 05/21/2022 Update: Three people sent me cache files and I also merged the cache file bcook254 has been keeping in github. We now have 30436 entries.

Edit: 06/21/2022 Update: Two people sent me cache files and I also merged the cache file bcook254 has been keeping in github. We now have 35150 entries.

Edit: 06/22/2022 Update: Two people sent me cache files and I also merged the cache file bcook254 has been keeping in github. We now have 37440 entries. Note that the cache is now zstd compressed due to discord's 8MB file size limit being reached. Use Ark to decompress it.

Edit: 06/23/2022 Update: Three people sent me cache files. We now have 40183 entries.

Edit: 06/25/2022 Update: Four people sent me cache files. We now have 42320 entries.
