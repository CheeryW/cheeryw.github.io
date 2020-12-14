---
layout: post
title:  Improving Discord Watch Party Experience
date:   2020-12-11 15:01:35 +0300
image:  06.png
tags:   Design Project
---
This past year has been a special year. With the few-month-long quarantine still going on, some of the more conventional means of sociolizing has been greatly challenged. As for me, a college student, I can't check out school events by just walking around the campus anymore. I can't hangout and discuss with my classmates at the library anymore. Many things have changed because of the online learning environment. To have a fulfiling last few months of my undergraduate studies, I tried my best to engage with my other classmates online. During this process, I became a regular Discord user. In this class design project, my teammates (Yong Woon Chung and Dennis Juanito) and I all have high motivation to re-design Discord because it is truly something that helps connecting people during this pandemic, and we believe that we have the potential to make the socializing experience on Discord better.

## Find the Problem
To find out what exactly we can improve on Discord, we first did some user research. We came up with some questions to ask users and then we translated the them to a survey using Google Forms. We mass distributed the survey through other Discord Channels, Reddit, close friends, and other social medias. 

#### User Demographics
Our survey got 41 responses in total. These participants of the survey __mostly have used Discord on regular basis and all of them have used Discord for social activities__. 75.6% of our survey respondents are 18 to 25 years old, and 22% of them are 26 to 35 years old. It is safe to say that in this study, we are mostly targeting users who are __18 to 35 years old__.

#### Research Findings
Below are our findings:

* 87.8% of the respondents have done a video call/screen share on Discord before
* 41.5% of the respondents have used Discord to watch Netflix/YouTube/Twitch, etc. before
* 61% of the respondents wish the UI on Discord is more customizable
* Screen sharing is the second most unsatisfying feature of Discord, right after notification settings
* Other commonly used apps that are similar to Discord are Zoom, Facebook Messenger, and Slack

After reviewing those findings, we decided that we want to focus on improving the experience of a Discord watch party for movies or TV shows, since screen sharing is a commonly used feature in Discord that people have complaints about, and a watch party is a particular usage of this slightly unsatisfying feature that we can work on.

## User Personas
Now that we finished user research, we wanted to visualize a few user personas to have a deeper understanding of our target audience, so we drafted the following personas:
![]({{ site.baseurl }}/images/alice.png)
![]({{ site.baseurl }}/images/bob.png)
![]({{ site.baseurl }}/images/bill.png)
![]({{ site.baseurl }}/images/carol.png)

## Competitors
Below we listed some other apps that can also be used to hold a watch party. We analyzed their pros and cons, so that we can possibly integrate some good features into our design and avoid things they don't do so great on.

### Netflix Party
URL: https://www.netflixparty.com
#### Pros
* The user doesn't have to share their screen in order to watch them together with their friends. The user only needs to share a link to a Netflix video with their friends so that they can start to watch it together.
* Has interactive live comments that visible to all users.
* Users have a variety of options that they can stream together with their friends, such as Netflix, Disney, Hulu, and HBO.
* No copyright issues.

#### Cons
* All users are currently required to have a Netflix account before allowing the user the service.
* Can’t stream youtube videos.
* Complicated installation process (learning curve for less tech-advanced people)
* Chat only, no video camera interaction
* Chat isn’t very interactive/customizable (Discord has custom server emotes and features/functions that can make it feel more personalized to each user group)

### Zoom
#### Pros
* Video quality and screen sharing features are excellent.
* Have more capacity for people to be on social meetings.

#### Cons
* The UI-designed feels towards for non-social meetings.
* Copyright issues
* Control over UI disappears when sharing screen
* No volume slider for each person
* No volume slider for screen being shared

### Air Time
URL: https://apps.apple.com/us/app/airtime-watch-together/id1018368216
#### Pros
* Has a variety of Emojis that users can use to describe their emotions at a particular moment during live streaming with their friends.

#### Cons
* Doesn’t provide a way for users to login to their Netflix so that they can watch Netflix videos. 
* Mobile UI only
* Small video camera feeds

### Rave
URL: https://apps.apple.com/us/app/rave-watch-together/id929775122
#### Pros
* Users have a variety of options that they can stream together with their friends, such as Netflix, Amazon Prime, Youtube, Vimeo.
* No copyright issues.

#### Cons
* According to Netflix's terms of use, all users are currently required to have a Netflix account before allowing the user the service
* Mobile only UI
* No landscape mode (portrait video only with chat below)


## UX Flow
Before we started to implement our design, we drew a UX flow demonstrating the specific steps in user interaction.
![]({{ site.baseurl }}/images/ux_flow.png)
*UX Flow*

When you and your friends join a group video call, Discord will show DM/server minimize buttons for you to make more screen space, along with a chat window on the side. There are also permanent UI buttons that allow you to show webcam, share screen, mute, disconnect. You don’t have to hover your mouse over to see those buttons anymore. After someone starts screen sharing their casual media browsing (youtube, twitch, etc), and people turn on their video cameras to show reactions, multiple popup windows will appear, one for streaming and one for friends’ webcams. When you hover your mouse over the shared video, it will show audio volume slider and video bitrate setting.

## UI Sketches
After we knew our basic UX flow, we drew some screen designs by hand. By this point, none of us had any experience with any UI design tool (such as Figma). Those sketches helped us focus on learning to use the UI design tool instead of designing the screens on the spot when we later implemented the low fidelity prototypes.
#### UI Sketch 1 (from DM Group Chat)
![]({{ site.baseurl }}/images/sketch1_1.jpg)
![]({{ site.baseurl }}/images/sketch1_2.jpg)
![]({{ site.baseurl }}/images/sketch1_3.jpg)

#### UI Sketch 2 (from Server Voice Channel)
![]({{ site.baseurl }}/images/sketch2_1.jpg)
![]({{ site.baseurl }}/images/sketch2_2.jpg)
![]({{ site.baseurl }}/images/sketch2_3.jpg)

## Low Fidelity Prototype
Below are the low fidelity prototypes we made, which is highly correlated with our UI Sketches. 

#### Prototype 1
*Note that even though you will see overlapping screens in the following GIFs, it doesn't actually exist in our UI design. This is purely a flaw of GIF.*
![]({{ site.baseurl }}/images/lofi_flow_1.gif)

#### Prototype 2
![]({{ site.baseurl }}/images/lofi_flow_2_1.png)
![]({{ site.baseurl }}/images/lofi_flow_2_2.png)

## User Testing on Low Fidelity Prototypes
After we finished the prototypes, we showed them to six potential users and gathered some feedback from them about the prototypes.
#### What Users Liked
The users liked the functionality of having the chat on the side a lot because Discord only provides a PIP window of the video feed, which can damage the media sharing experience. The users also liked hiding the server list and DM list, since the server list is always there on Discord.

#### What Users Struggled With
A few users were confused regarding the emoji feature of the video chat, because they believed that they would be bothered or spammed by their friends while watching/sharing videos or games. A potential fix would be for the sharer to toggle this feature or to make the emojis in a corner of the design.

#### Plan for Next Steps
Moving forward we feel confident because the only disapproval we felt that we received was the emojis features, but we can change that with a few new features (toggling the feature, having the feature smaller on the screen). We will proceed with a mix of the two designs and just make them equal because they are generally similar.

## High Fidelity Prototype
Based on the feedback we got from low fidelity prototype user testing, we built a high fidelity prototype that looks much more like Discord than the previous prototypes.
#### Starting Point
![]({{ site.baseurl }}/images/server_start.png)
*Starting from server voice channel*
![]({{ site.baseurl }}/images/DM_start.png)
*Starting from DM group chat*
#### When Side Chat is Shown
![]({{ site.baseurl }}/images/server_all_expanded.png)
*Server View*
![]({{ site.baseurl }}/images/DM_all_expanded.png)
*DM View*
#### Servers/DMs and Side Chat Minimized
![]({{ site.baseurl }}/images/minimized.png)
#### When Netflix Screen Share Starts
![]({{ site.baseurl }}/images/with_reax_option.png)
#### Viewing Chat While Watching Netflix
![]({{ site.baseurl }}/images/chat_expanded.png)
#### Choose Emoji Reaction
![]({{ site.baseurl }}/images/choose_emoji.png)
#### Emoji Reax Turned On
![]({{ site.baseurl }}/images/reax_on.png)

## User Testing on High Fidelity Prototype
To get consistent user feedback, we will be revisiting our interview subjects from the earlier milestones to get direct feedback on things they already commented on.

The interview subjects are heavy discord users. Some enjoy gaming, others do not game, and they possess a medium to high level of tech familiarity. Below are the feedback we received from them:

* The UI looks simple compared to the existing UI and looks easier to use and understand
* I like the updated reactions implementation that would have a toggle on the page and keep the reactions on the side in case people spam emojis
* Would prefer to have custom server emotes on the emojis implementation
* Should separate the screen sharing and the webcam sharing features on the UI so we can see share screen as the main and see the video cameras on the side or above like zoom (zoom does this very well)
* Have the ability to change fonts, font size

## Refining High Fidelity Prototype
#### Adding What was in Low Fidelity Prototype
In our first version of high fidelity prototype, there are still some elements that exist in earlier prototypes that we didn't have time to implement, so we added those after getting the feedback.
![]({{ site.baseurl }}/images/invite_friends.png)
*User invites friends to watch party*
![]({{ site.baseurl }}/images/friend_notification.png)
*The notification friends receive after being invited*

#### Modification based on Feedback
From the feedback we received, we decided that Zoom-like camera windows and the pause request button are things that we can add on top of our current prototype, and the implementations are shown below.
##### Moveable Camera Windows
![]({{ site.baseurl }}/images/camera_windows.png)
*Several users' cameras showing on the side*
![]({{ site.baseurl }}/images/minimized_camera.png)
*Only one user's camera is showing*
##### Pause Request Button
![]({{ site.baseurl }}/images/pause_request.png)

## Reflection
As a software developer, it is a novel and enriching experience to personally go through the events that happen before any code is written. I appreciate the opportunity this project has given me to get familiar with the design process. If we have more time, we will probably focus on refining the visual details of our high fidelity prototype so it is as close to the real Discord in terms of UI as possible.