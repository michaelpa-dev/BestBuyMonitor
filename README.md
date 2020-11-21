[![N|Solid](https://media.discordapp.net/attachments/735590383396061234/775049214824546325/michaelpa.png)](https://twitter.com/michaelpa_WMG)
# Best Buy Monitor

### Get Started 
Make sure you're in the correct directory before trying to install this program. Many people have issues with directories. If you use Git Bash on windows, I reccomend navigating to your home directory before installing. Typing `cd` and then hitting enter should get you there.

## Prerequisites
Make sure you have these currently installed on the machine you plan to run this application on. If you have any problems with installation or unfamiliar with this there are some resources below.

[Node (LTS)](https://nodejs.org/en/) 12.16.2

[Mongo DB](https://www.mongodb.com/)

[Git](https://git-scm.com/)


### Installing
```
git clone https://github.com/michaelpa-dev/BestBuyMonitor.git
npm install
```

# How to use with Discord

  - Create a Discord server channel webhook and copy to clipboard 
  - Open the setting.json file located in the config folder
  - Under the `Webhook` field, paste your discord webhook url in the " "
  - In the array of `Skus` paste all of the Skus of the items that you wish to observe comma seperated 
    - it should look something like this `"Skus":[6429434,6437910,6432447,6430623,6436192,6434363,6428846, 6429440],`
  - Open up your favorite console application and navigate to the project.
  - A default `interval` of 10 seconds is applied.

`Webhook:` Discord webhook url where all notifications sent from the monitor will go.
`Skus:` A comma seperated collection of all the items you want monitored.
`Interval:` Time in milliseconds between each time the monitor will check on your list of products you've entered.
```
{
    "Discord":{
        "Webhook": ""
    },
    "Skus":[],
    "Interval": 5000
}
```

## Running the application
 Running the application is as easy as navigating to the directory where you have it installed in your favorite console application and starting up the node application.
 ```
 cd ~/BestBuyMonitor
 node app.js
 ```
