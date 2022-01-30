# CodeDisc

A slack integration for simple code discussion

### Commands
/codetalk *[github file url]* - start the codetalk discussion on that file (required to be run first)

/showline *[linenumber, can be in range]* - show the snippet from the current file at the specified line

/refer *[github file url]* *[linenumber]* - show the snippet from the specified file at the specified line

/find *[keyword]* - find the lines that contain the keyword

### Installation
 <a href="https://slack.com/oauth/v2/authorize?client_id=2943562887175.2970828686849&scope=commands&user_scope="><img alt="Add to Slack" height="40" width="139" src="https://platform.slack-edge.com/img/add_to_slack.png" srcSet="https://platform.slack-edge.com/img/add_to_slack.png 1x, https://platform.slack-edge.com/img/add_to_slack@2x.png 2x" /></a>

### Manual Set up
1. Deploy to Heroku [![Deploy to Heroku](https://www.herokucdn.com/deploy/button.png)](https://heroku.com/deploy)		
2. Remember that url 		
3. Go to your slack team's slash commands configuration		
4. Add 4 commands, each pointing to these url respectively:		
 * codetalk, [your-deployed-heroku-url]/review		
 * showline, [your-deployed-heroku-url]/showline		
 * refer, [your-deployed-heroku-url]/refer		
 * find, [your-deployed-heroku-url]/search
5. Configure other options as you see fit, and you are done!
