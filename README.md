# Database Model Analysis - Slack

## Pre-analysis:
- One __user__ has Many __workplace__
- One __user__ has Many __email__
- One __workplace__ has Many __member(user)__
- One __workplace__ has Many __channel__
- One __channel__ has Many __member(user)__
- One __member(user)__ has One __timeline__
- One __timeline__ has Many __thread__
- One __member(user)__ has Many __channels(joined)__
- One __thread__ has Many __member(user)__
- __thread__ must has more than one __member(user)__
- __thread__ is conversation/interaction (direct message/reply on channel)
- One __direct message__ has Many __member(user)__
- One __member(user)__ has Many __direct message__
- One __member(user)__ has One __timeline__
- One __member(user)__ has One __member profile__
- One __member(user)__ has One __member email__
- One __member profile__ has One __profile picture__
- One __member profile__ has One __full name__
- One __member profile__ has One __member name__
- One __member profile__ has One __member description__
- One __member profile__ has One __member status__
- One __member profile__ has One __member phone number__
- One __member profile__ has One __time zone__
- One __member profile__ has One __skype__
- One __user__ has Many __profile__
- profile, workplace which has high priority?
  - user workplace owns user profile?
  - OR user profile owns user workplace?
  > [You can join as many workspaces as you'd like. Your Slack account is linked to your workspace, so you'll create a new Slack account for each workspace you're invited to. Each account is separate, but you can use the same email address to sign up for other workspaces.](https://get.slack.help/hc/en-us/articles/201405046-Joining-multiple-Slack-teams)
- One __member(user)__ has Many __file(upload)__
- One __file(upload)__ has Many __channel__
- One __workplace__ has Many __admin__
- One __workplace__ has One __owner__
- One __workplace__ has Many __guest__
- Enterprice Grid will make workplaceds interconnected!
- One __channel__ has One __#general__
- One __channel__ has One __#random__
- __channel__ has two types: public & private
- __DM(direct message)__ are not visible to outsider
- message is the basis interaction unit:
  > [Communication in Slack happens through messages, whether they’re in channels or DMs.](https://get.slack.help/hc/en-us/articles/115004071768#sending-messages)
- timestamp for every event, message sent/file upload/file share
- workplace feels like the homepage of Facebook
- invitation needs to join a workplace
- One __email__ has Many __workplace__
- One __workplace__ has One __Slack URL__
- __workplace__ can be merged together by owner and admin (Wow)
- anyone can [create a new workplace](https://slack.com/create#email) by providing a email, not registration 
- __Slack URL__ to __workplace__, __email__ verify user, __password__ login
- Slack has access logs
- One __user__ has Many __signin workplace__
- [switch workplaces can between all signined account, even different emails](https://get.slack.help/hc/en-us/articles/201405046-Sign-in-to-multiple-workspaces)
- communication can be DM/channel? or DM and channel
  
## Entity Relationship Diagram(ERD):
![slack erd](/images/slack_erd.png "Slack ERD")

## Entity/Table:
- will fix later

## Associations:
- will fix later

## Links/Resources:
- [What is Slack?](https://get.slack.help/hc/en-us/articles/115004071768)
- [Slack Glossary](https://get.slack.help/hc/en-us/articles/213817348)
