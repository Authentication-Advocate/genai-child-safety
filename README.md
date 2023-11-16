# GenAI Child Safety

## Context
Machine Learning (ML) and Generative Artificial Intelligence (GenAI) has arrived, and will continue to develop. While the most cutting edge capabilities reside in the proprietary sphere of private companies, open source versions of the same capabilities exist. We cannot stop the evolution of these technologies without infringing freedom of speech; they're here to stay and will continue to improve. 

This content seeks to provide actionable recommendations for the protection of children in this new world, considering several risks. The intended audience is parents, and the intended outcome is an understanding of potential risks and things you can do to manage those risks.

### Why does this exist?
[We saw this video and didn't like it](https://www.linkedin.com/posts/thecisolife_thepowerofai-privacy-cybersecurity-activity-7126190147158601729-RskX/?utm_source=share&utm_medium=member_ios), specifically it provokes a lot of fear and doesn't give much advice on what to do about it. We label [this work FUD (promoting of fear, uncertainty, and doubt)](https://www.microsoft.com/en-us/research/wp-content/uploads/2016/02/FUD_APleaForIntolerance.pdf), and as cybersecurity practitioners we belive FUD holds the conversation back instead of moving it forward.

### Limits of this guide
This guide is intended for "normal people"; not companies, celebrities, or governments.
If you believe any of:
* A bad actor may specifically target YOU or your family, as opposed to being a target of opportunity / victim of chance
* A credible threat of a bad actor physically accessing a person or device

Then you are beyond the security considerations of this guide and should seek additional guidance from cybersecurity professionals.

## Risks
### Impersonation of a family member
#### Audio / Phone Calls
With sufficient samples of a person's voice it is possible generate audio signals from text which sounds substantially similar to the person's voice. [This capability is offered as part of Apple's OS platform](https://support.apple.com/en-us/HT213878) because it is a powerful tool for people with a limited or diminished ability to speak. It will be available to bad actors as well.

##### Threat Scenario
A bad actor may acquire sufficient samples of a person speaking to build a GenAI model capable of generating arbitrary speech which sounds like the person's voice. Audio generated in this way could be used to manipulate a member of the person's family to take action such as sending money to the bad actor.

##### How to mitigate
###### Incoming Phone Calls
[Phone numbers are easily spoofed when someone is calling you](https://www.fcc.gov/spoofing). Even if you receive a phone call which appears to originate from a member of your family, you should not be entirely confident that the call originated with your family member.

If you are preparing to send money to someone based entirely on a phone call, ask them to [communicate with you through an authenticated channel](#authentication-approaches) or [simply call them back at a number you already know is associated with that person](#outgoing-phone-calls).

###### Outgoing Phone Calls
It is substantially more difficult to cause a phone call you initiate to a given phone number to reach an unintended/bad recipient. Ensuring that you've reached someone at a particular phone number can be as simply as calling them back at that same number. DO NOT ACCEPT A NEW PHONE NUMBER for a person during a potential threat scenario; ideally only save a new phone number for a person in an [authenticated interaction](#authentication-approaches).

Two risks to consider, which are [beyond the scope of this guide](#limits-of-this-guide):
* A bad actor could have physical access to a phone and receive your phone call with it
* A bad actor could use a [SIM swap scam](https://en.wikipedia.org/wiki/SIM_swap_scam) to take over a cellular account; however this would represent a level of targeting and effort beyond the scope of this guide.

##### How to prevent
It is only possible to impersonate a person's voice with sufficient recordings of their speech. To avoid a person's voice being subject to impersonation with GenAI, see [guidance on limiting exposure of likeness](#limiting-likeness-exposure).


## Authentication Approaches
These are ways to authenticate someone you are communicating with. [Given the limited applicability of this guide](#limits-of-this-guide), these approaches may be significantly below the bar necessary to provide reasonable assurance for such entities, but are intended to be reasonable and appropriate advice for people unlikely to be targeted by a sophisticated adversary. These are intended to counter the evolution of threats like [tech support scams](https://consumer.ftc.gov/articles/how-spot-avoid-and-report-tech-support-scams).

### Both people have access to text messaging (SMS/MMS)
* Send text messages back-and-forth with a phone number YOU ALREADY KNOW IS ASSOCIATED with the person to confirm whatever is being requested

### Both people have access to email
* Send emails back-and-forth with an email address YOU ALREADY KNOW IS ASSOCIATED with the person to confirm whatever is being requested

### Both people are on Apple devices
* [Communicate via iMessage](apple.md#imessage) to confirm whatever is being requested
* [Communicate via FaceTime](facetime.md#imessage) to confirm whatever is being requested

## Limiting Likeness Exposure
GenAI creates the risk of impersonation only if sufficient source data of a person's likeness is available to enable generation of content. By limiting a bad actors's access to digital data of:
* A person's face
* A person's voice
* A person's face in motion speaking with their voice

You can make it difficult or impossible to impersonate a person. Limiting a bad actor's access to your likeness is a way to prevent impersonation.

### Don't share
Practice abstinence with regards to sharing photos, audio, or video recordings of yourself and your loved ones. This won't work for everyone, but is technically the most effective way to limit this risk.

### Don't publish (share publicly)
If you produce content specifically intended for public distribution, that content could be used to impersonate people visible and speaking in the content with GenAI in the future. This is a risk that comes with becoming a public figure by a person's likeness being published.

### Share smart
Only share photos, audio, or video recordings of yourself and your loved ones with specific people you wish to have access that information; people you trust to not use it maliciously.

In practical terms, do not post content publicly but instead share with specific friends/followers AND prune those lists of people occasionally.

#### Guidance by-platform
##### [Instagram](https://www.consumerreports.org/electronics-computers/privacy/instagram-privacy-settings-a3036233134/#:~:text=Don't%20let%20Strangers%20See%20Your%20Posts)
##### [Facebook](https://www.consumerreports.org/electronics-computers/privacy/facebook-privacy-settings-a1775535782/#limit-who-sees-your-photos-and-posts)
##### [TikTok](https://www.consumerreports.org/electronics/privacy/how-to-use-tiktok-privacy-settings-a8690365773/)
Note: Content shared on TikTok is generally intended to be public; so most posting of content on TikTok should [be considered publishing](#dont-publish-share-publicly).