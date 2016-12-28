---
layout: post
title: "Gitter Cheatsheet"
description: "The Gitter.im commands I use and don't want to forget"
category: "Cheatsheet"
tags: ['Cheatsheet', 'Gitter']
---
{% include JB/setup %}
My morning routine consist of making my coffee, streaming my music, then opening my fav'd Gitter rooms before I start cutting code. 

Sometimes I get into some quick converstations so it is nice to know some common shortcuts.

## Commands

All commands are executed in the chat bar and begin with a forward slash `/`. Gitter will give you a nice autocomplete with the most common commands. As you type Gitter will auto-suggest the command closest to what you have entered.

The following are some cool commands I have used in the past.

I recommend you create a room for yourself to try out these commands until you are comfortable with them. The last thing you want is everyone seeing you are trying to ban someone because you had a typo.

----

#### Sanity Commands

There is always someone that doesn't contribute much other than spaming your Chrome notification popup. Here is a command to block a user:

	/ban @username

Once you've calmed down, you can un-block them with:

	/unban @username

Notify-all will turn on muted notifications. This can get kind of spammy if you use Chrome notifications in a busy room.

	/notify-all

Use notify-mute if you get too many notification pop-ups. This is great when you just need to work and what to ignore what's happening in Gitter for awhile.

	/notify-mute

If you just want to be notified when someone is chatting @ you.

	/notify-announcements

----

#### Room Commands

Adding a new room is easy enough through the interface or you can simply use the `/channel` command to bring ut the create room dialog.

	/channel

To favorite a room you can click on the **star** in the top right by you avatar or use this. This will unfavorite if you have already fav'ed the room.

	/fav

to leave a room and drop out of the converstions you can simply execute. I found that this command also **unfavorites** the room on you.

	/leave

If you are the admin of a room you can add a description to the room with:

	/topic We talk about Vuejs anything else is punishable by banning

If you are the admin of a room you can remove a user with:

	/remove @username

----

#### Message Commands

 If you want to spam everyone and tell them something use:

	/me I am sitting here coding in case you are interested
 
 If you have been away and have a bunch of unread messages you don't care about you can:

	/mark-all-read
 
To start a private conversation you can hover over the user's avatar or use the command:

	/query @username

There are some collapse commands to tidy your chat history. I haven't used them but here they are:

	/collapse
	/collapse-all




----