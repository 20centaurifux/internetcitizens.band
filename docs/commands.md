# Available commands

## addr
     /addr {street address}
     /addr

Sets the street address of the registered user. You can use a pipe as delimiter.

Without an argument the street address is unset.

## away
     /away {message}
     /away

Sets the away status or displays your away message when no argument is given.

## beep
     /beep {nick}

Notifies a user.

## boot
     /boot {nick}

Throws a user out of a group.

## cancel
     /cancel {-q} {-n nick|-s address}

Cancels an invitation. Use the -q option if you don't want to receive a confirmation.

## cp
     /cp {current password} {new password}

Sets a new password for your registered nickname.

## delete
     /delete {password}

Deletes your registered nickname.

## drop
     /drop {nickanem}

Drops a user.

## echoback
     /echoback {mode}

Receive messages you send.

```
Mode        Description
---------------------------------------------------------
off         receive no messages you send
on          receive public messages you send
verbose     receive public and personal messages you send
```

## email
     /email {email address}
     /email

Sets the email address of the registered user.

Without an argument the email address is unset.

Confirm your email address to enable message forwarding or resetting your password.

## exclude
     /m {nick} {message}

Sends an open message excluding the specified nick.

## forward
     /forward

Turns on personal message forwarding.

Messages from the personal inbox are sent to the confirmed email address.

## g
     /g {group}

Joins another group.
     
If the group doesn't already exist it will be created. When the group name isn't protected (e.g. 1) you'll be the moderator.

You can also join the same group as a known user:

     /g @alice

Prepend dot(s) to the group name if you want to change its initial visibility:

```
Prefix Description
-------------------
.      secret group
..     hidden group
```

## help
     /help
     /help {topic|command}

Displays a help page.

## hush
     /hush {-q} {-o} {-p} {-n nick|-s site}

Hush nicknames or sites.

Note that hush is a toggle. If you have hushed someone, issue the same command you used to hush them to unhush them.

```
Argument         Description
-----------------------------------------------------------
                 show hush list
-n               server doesn't send you messages from this nickname
-s               server doesn't send you messages from people logged in from this site
-q               don't receive confirmation
-o               hush open messages only
-p               hush personal messages only
```

## invite
     /invite {-q} {-r} {-n nick|-s address}

Invites a nickname (-n) or address (-s) to a restricted group. Use the -r option if the invited user has to be registered to join.

Set the -q option if you don't want to receive a confirmation.

## log
     /log {level}
     /log

Sets the log level (0-4). With no argument the current level is displayed.

## m
     /m {nick} {message}

Sends a private message to a user.

Private messages sent to "server" are interpreted as command.

## name
     /name {new nick}

Changes your nickname.

## news
     /news {item}
     /news

Prints a news item. With no argument all news items are displayed.

## noaway
     /noaway

Removes the away status.

## nobeep
     /nobeep {mode}

Changes the beep mode of the current session.

```
Mode        Description
---------------------------------------------------------
off         receive beep messages
on          ignore beep messages
verbose     ignore beep messages, but show a notification
```

## notify
     /notify {-q} {-n nick|-s site}

Receive a notification when a nickname or site signs on/off.

```
Argument         Description
-----------------------------------------------------------
                 show notification list
-n               notify when nickname signs on/off
-s               notify when site signs on/off
-q               don't receive confirmation
```

## nofoward
     /noforward

Turns off personal message forwarding.

## noprotect
     /noprotect

Allow other users to see the email address of the registered nick.

## phone
     /phone {phone number}
     /phone

Sets the phone number of the registered user.

Without an argument the phone number is unset.

## p
     /p {password}

Registers your nickname.

A new record is created if you register a nickname for the very first time. Otherwise the password is checked.

## protect
     /protect

Don't allow other users to see the email address of the registered nick.

## read
     /read

Reads the messages from your personal inbox. Messages get deleted as soon as they are being received.

## reputation
     /reputation {nick}

Displays the reputation value (0.0..1.0) of a logged in user.

## rname
     /rname {real name}
     /rname

Sets the real name of the registered user.

Without an argument the real name is unset.

## secure
     /secure

When this mode is activated a password is mandatory to register the nickname. Otherwise the nickname will be registered automatically if the address of the last successful registration matches your current address.

## stats
     /stats {-s|-t|-m|-y|-a}

Lists various server statistics. There are several time frame filters available:

```
Flag  Filter
------------------------
s     since server start
t     today
m     this month
y     this year
a     overall
```

## status
     /status {flags|options}
     /status

Sets group flags and options.

The following flags and options are available:

```
Flag  Name
----------------
Visibility
----------
v     visible
s     secret
i     invisible

Control
-------
p     public
m     moderated
r     restricted
c     controlled

Volume
------
q     quiet
n     normal
l     loud

Option           Name
---------------------------
# {size}         size limit
b {seconds}      idle-boot
im {seconds}     idle-mod
```

With no argument the group's current flags and options are displayed.

## talk
     /talk {-q} {-d} {-r} {-n nick|-s address}

Adds a nickname (-n) or address (-s) to the list of allowed talkers in a controlled group. Use the -r option if the user has to be registered to talk. The -d option removes an entry from the list.

Set the -q option if you don't want to receive a confirmation.

## text
     /text {text}
     /text

Sets the arbitrary text of the registered user profile.

Without an argument the text is unset.

## topic
     /topic {topic}
     /topic

Sets the group's topic.

With no argument the topic is shown.

## unsecure
     /unsecure

When this mode is activated the server tries to register your nickname automatically. This happens if the address of the last successful registration matches your current address.

## v
     /v

Prints server version.

## wall
     /wall {message}

Sends an important broadcast message.

## whereis
     /whereis {-a} {nick}

Displays the address of a user. Use the -a flag to show more details.

## whois
     /whois {nick}

Displays the profile of the specified nickname.

## write
     /write {nick} {message}

Writes a message to a user. Messages are stored in a personal inbox.

## w
     /w {-s|-g|.|group}

Displays a list of available groups and their members.

```
Argument         Description
-------------------------------------------------
 .               lists everyone on server
-s               short list of everyone on server
-g               lists the groups on the server
.                lists just the group you're in
{group name}     lists the specified group
```

## www
     /www {website}
     /www

Sets the website of the registered user.

Without an argument the website is unset.
