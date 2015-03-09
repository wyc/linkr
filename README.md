linkr - A simple IRC/Slack bridge
====

## Requirements
- >= Go ~1.2
- Slack account w/bot access
- IRC w/option nickserv registration

## Running linkr
1. Go to your org's Slack page
2. Add a Slack API integration under DIY
3. Choose a name for the bot and grab the API token
4. Setup the environmental variables. Note that IRC_NETWORK is host:port,
   TLS-only.
5. Install the project:
```
$ go get github.com/wyc/linkr
$ linkr
```

## Notes
- This adds a security risk if your IRC channels are public. You need to be
  invited to an organization's Slack to participate while IRC has a freer
  nature. Consider using invite-only/password channels.

## To do:
- Use CLI flags where they make sense
- Nicer error messages that explain what went wrong
- Handle more types of IRC/Slack events
- Cache Slack names and other metadata?
