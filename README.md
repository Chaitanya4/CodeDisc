# CodeDisc
A slack integration for discussing code present on GitHub repository.

### Commands
/codedisc *[github file url]* - Enter the github file URL about whose content you want to have discussion with your teammates.(required to be run first)

/showlines *[startlinenumber-endlinenumber]* - It shows code snippet starting from startlinenumber upto the endlinenumber.

/refer *[github file url]* *[startlinenumber-endlinenumber]* - Use it to find the specific code snippet inside the github file. It shows code snippet starting from startlinenumber upto the endlinenumber of the *[github file url]*.

/find *[keyword]* - It find the lines inside the github file that contains the mentioned keyword.

### Installation
<a href="https://slack.com/oauth/v2/authorize?client_id=2943562887175.2970828686849&scope=commands&user_scope=openid"><img alt="Add to Slack" height="40" width="139" src="https://platform.slack-edge.com/img/add_to_slack.png" srcSet="https://platform.slack-edge.com/img/add_to_slack.png 1x, https://platform.slack-edge.com/img/add_to_slack@2x.png 2x" /></a>

### Manual Set up
1. Deploy to Heroku	
2. Remember that url 		
3. Go to your slack team's slash commands configuration		
4. Add 4 commands, each pointing to these url respectively:		
 * codedisc, [your-deployed-heroku-url]/codereview		
 * showline, [your-deployed-heroku-url]/showline		
 * refer, [your-deployed-heroku-url]/refer		
 * find, [your-deployed-heroku-url]/search
5. Configure other options as you see fit, and you are done!
