# Topics

## Registration
Your nick is how people know you. If you want to use a nick permanently you should register it with the /p command.

A new record is created if you register a nickname for the very first time. From now on your password is required for registration. Change your password with /cp.

A registered nick has an inbox for private messages. This allows you to send messages to signed off users.

You can view user profiles with /whois. Feel free to fill in your own profile to share personal information with other users.

## User
Every user has a nickname and is member of a group.

Use /w to receive a list of available groups and connected users. You can change your group membership with /g.

To see status and address of a connected user use the /whereis command.

```
Flag     Description
----------------------------
r        registered user
a        administrator
nr       real name not known
ssl      secure connection
aw       away flag is set
```

Chat directly with /m. To send a notification use the /beep command.

If you're going to leave your desk you might want to set an away message with /away.

## Confirmation
     
Registered nicks can confirm their email address with the /confirm command. This makes it possible to forward messages from the personal inbox as email or request a new password with /newpasswd.

## Group
Groups have a moderator who can set topic and status. The latter affects visibility, volume, control, allowed size and idle time(s).

### Control
There are four control levels:

```
p    public
     - everyone can change the topic
     - there aren't any restrictions when there's no moderator

m    moderated
     - only the moderator can modify the group and boot members

r    restricted
     - only the moderator can modify the group and boot members
     - only invited nicks/addresses can join the group
     - only the moderator is allowed to invite or cancel nicks/addresses

c    controlled
     - only the moderator can modify the group and boot members
     - only nicks/addresses from the list of talkers are allowed to speak
     - only the moderator can manage the list of talkers
```

### Visibility
There are three visibility levels. They affect how a group is listed.

```
Flag  Name          Description
------------------------------------------
v     visible       group is visible
s     secret        group's name is hidden
i     invisible     group doesn't appear
```

### Volume
There are three volume levels:

```
Flag  Name       Description
-------------------------------------------------
l     loud       all messages are delivered
n     normal     a few status messages are ignored
q     quiet      no messages at all
```

### Idle
Group members and moderators can be booted automatically when they're idling too long.

The idle-boot option defines the maximum allowed idle time for all group members except the moderator.

Use the idle-mod option to set an idle timeout for moderators.

When the moderator is booted the group member with the shortest idle time and without an away message becomes the next moderator. If no user can be found the group becomes public.

### Inbox
Registered nicks have a personal inbox.

You are able to send and receive messages with the /write and /read commands after registration.

Messages are stored in an inbox even when the receiver isn't logged in.
