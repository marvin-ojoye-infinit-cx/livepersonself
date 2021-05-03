---
pagename: Voice and Video
Keywords:
sitesection: Documents
categoryname: "Messaging Channels"
documentname: Mobile App Messaging SDK for Android
subfoldername: Advanced Features
permalink: mobile-app-messaging-sdk-for-android-advanced-features-voice-and-video.html
indicator: messaging
---

### Introduction

Voice and Video integration allows brand agents to communicate with consumers via voice or video calls.
<div style="width: 100%; position: relative;">
    <img src="../../../../img/android_voice_call.png" alt="Voice call example screen" style="float: left; width: 25%;height: auto; margin-right: 1em">
    <img src="../../../../img/android_video_call.png" alt="Video call example screen" style="width: 25%;height: auto;">
</div>

{:.important}
Voice & Video capabilities are available only on Android SDK 4.8.1 and above. Only enabled for authentication mode: Code flow and JWT flow.

KB article: [Voice & Video Overview](https://knowledge.liveperson.com/agent-manager-workspace-agent-tools-for-messaging-agent-workspace-for-messaging-cobrowse-for-messaging.html)

To enable the feature on your Conversational Cloud account please review the KB article

### How to enable:

```xml
<bool name="lp_enable_voice_video_call">true</bool>
```


### Branding and Configurations

#### lp_enable_voice_video_call
Enables or disables the ability for an Agent to start a voice or video call.

- **Type:** bool
- **Default value:** false

#### lp_voice_call_image_icon
Defines default Image icon for Voice Invite.

- **Type:** drawable

#### lp_video_call_image_icon
Defines default Image icon for Video Invite.

- **Type:** drawable

#### lp_voice_video_accept_call_button_image
Defines default background image for Accept button on Voice & Video Invite

- **Type:** drawable

#### lp_voice_video_decline_call_button_image
Defines default background image for Decline button on Voice & Video Invite

- **Type:** drawable

#### lp_voice_video_end_call_button_image
Defines default background image for End button on Voice & Video Invite

- **Type:** drawable
- **Preconditions:** This image is only shown on the Voice & Video Invite when Consumer has an active Call
- **Notes:** To enable this image lp_voice_video_end_call_button_type should be set to hangup`

#### lp_voice_video_join_call_button_image
Defines default background image for Join button on Voice & Video Invite

- **Type:** drawable
- **Preconditions:** This image is only shown on the Voice & Video Invite when Consumer has an active Call

---

#### lp_voice_video_invite_icon_tint
Defines default icon tint color on Voice & Video Invite

- **Type:** color
- **Default value:** gray

#### lp_voice_video_accept_button_tint
Defines default tint color for Accept/Join Button on Voice & Video Invite

- **Type:** color
- **Default value:** white
- **Note:** This property controls both the Accept and Join call Button

#### lp_voice_video_decline_button_tint
Defines default tint color for Decline/End Button on Voice & Video Invite

- **Type:** color
- **Default value:** red
- **Note:** This property controls both the Decline and End call Button

#### lp_voice_video_accept_button_background_color
Defines default background color for Accept/Join Button on Voice & Video Invite

- **Type:** color
- **Default value:** green
- **Note:** This property controls both the Accept and Join call Button

#### lp_voice_video_decline_button_background_color
Defines default background color for Decline/End Button on Voice & Video Invite

- **Type:** color
- **Default value:** clear
- **Note:** This property controls both the Decline and End call Button

#### lp_voice_video_invite_icon_render_original_image
Defines if use original image lp_video_call_image_icon or lp_voice_call_image_icon image for Voice or Video Invitation Icon

- **Type:** boolean
- **Default value:** false

#### lp_voice_video_accept_button_render_original_image
Defines if use original image lp_voice_video_accept_call_button_image or lp_voice_video_join_call_button_image for Accept Button on Voice & Video Invitation

- **Type:** boolean
- **Default value:** false

#### lp_voice_video_decline_button_render_original_image
Defines if use lp_voice_video_decline_call_button_image or lp_voice_video_end_call_button_image for Decline Button on Voice & Video Invitation

- **Type:** boolean
- **Default value:** false

#### lp_voice_video_end_call_button_type
Defines which icon to display on Join Button for Voice & Video Invitation

0: Close
1: Hangup

- **Type:** integer
- **Default value:** 0
- **Preconditions:** This type is only shown on the Voice & Video Invite when Consumer has an active Call

#### lp_voice_video_invitation_bubble_background_color
Defines background color for Voice & Video Bubble

- **Type:** color
- **Default value:** light gray
