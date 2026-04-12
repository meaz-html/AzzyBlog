---
title: "IRC: My thoughts/findings"
description: "Exploring IRC!"
date: 2025-11-30
tags: ["Other", "Retro-Tech", "Technology"]
---

Hello Everyone, In my last post, i talked about flirb, well today, we are heading at IRC, which yes, is still alive even to this day, I have been experimenting with it over the last weeks, and i have to say, it's a great discord alternative from 1988 (since there's a lot of crap inside discord).

Basically, to be able to use IRC, you of course need a IRC client, I used [Halloy](https://halloy.chat) for desktop, and Revolution IRC on my 2 phones:

![](https://res.cloudinary.com/dnkm8pijh/image/upload/v1775997007/screenshot-2025-11-30-102445-2_w6a1xv.jpg)

![](https://res.cloudinary.com/dnkm8pijh/image/upload/v1775996949/revolution-irc_lkmhdh.jpg)

You also need a "nickname" to be able to chat on IRC, for example, my nicknames are stellarcapricorn on freenode and libera (i will explain IRC Servers later)

There is also channels, which are basically public group chats you can discuss stuff in, for example, linux on freenode and debian on libera.

IRC Servers are basically where anybody can (if on that server) can talk to you by your nickname, its your channels, nicknames, SASL Auth (more on that) that are stored, and you can connect there to chat, it's in short, a community.

On the Technical side, SASL is an Authentication Mechanism that is used in most servers, that allow you to login in one server you registered your nick again, this is useful since if you already registered a nick with that server, and then login with that nick on the same server, but a different device/client, it will either ask you to change your nickname, or it changes it for you after 1 minute or less, SASL allows you to authenticate yourself with the same nick on the same server, without it changing it after 1 minute or so. Its making sure that you are "that" person trying to use that nick in short.

SASL is sometimes confused with IRC Bouncers, basically, bouncers help you to stay signed in on your client so you can still receive messages even if the app is closed (stays in background), this is because, even if you are registered with "NickServ" (the nickname service that manages the registration of nicknames on a server,this is also SASL), the client will log you out after inactivity, but with bouncers, they stay logged in, there are IRC Mobile clients (Goguma and IRCloud) that have bouncers like [IRC Today](https://irctoday.com) or [IRCCloud](https://www.irccloud.com) baked in the client, all they have to do is sign up for the bouncer service and connect their nick to it, and voila, but with other clients (like Halloy), they don't have bouncers directly baked in.

Halloy actually depends on a config.toml file that fetches nicks, preconfigured channels, SASL info and the IRC Server/s, they have bouncer support, but you need to host one yourself (Soju), you cannot just use something like IRC Today as your bouncer in Halloy, it wont work.

From my own findings, you cannot connect two different devices, with a different client, with the same server and nicks on each device (even with SASL), at the same time, I personally find it annoying that to be able to connect to IRC on my Desktop, I have to go and disconnect from my other device that's connected to the server.

Another thing i found, IRC Servers are not federated, they use the same protocol of course, but it's not like i can join a channel from freenode on libera unlike ActivityPub where its federated and I can like/comment on a Mastodon post from Bluesky (its weird, but i am not sure that's happening right now).

In the End, IRC is a great alternative to Discord, but it has its downsides, like unreliable servers or DDos attacks, but remember, you can host your own, it's just hard work to do it. But i will see you in my next post!
