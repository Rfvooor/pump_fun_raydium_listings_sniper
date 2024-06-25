
# Auto Pump.fun Listing Sniper
This is a raydium listing sniper, with:
- filtering for pump.fun launches
- filtering based on market cap in SOL 
- filtering for socials
- take profit and stop loss 
This repo was forked from WARP sniper and modified as such. 
Running 24/7 on your own server, keeping keys in your control. 

# Setup 
Setup is a super simple process, taking at most 15-20 mins depending on technical ability. 
For any questions:
TG: https://t.me/+GwZPCWSKElxjNjY5 or DM me @rfvooor 
Twitter: https://x.com/rfvoooor

For further questions/documentation on what some of the settings are, read thru [the warp readme](https://github.com/warp-id/solana-trading-bot)

## Obtain bot equipment (5 mins)
Get a VM (virtual machine) from a provider such as AWS, Google, Heroku, Digital Ocean.
Many of these platforms provide free sign-up credits and so there shouldn't be costs related to this for a while.
(Would recommend digital ocean, very easy option and this guide wil focus on DO)
- Once signed into DO, you should see a button in the top that says "Create" and a dropdown menu should appear
- Click droplets
![Screenshot 2024-06-24 153405](https://github.com/Rfvooor/AutoTelegramSniper/assets/173009279/01c9df7b-93c5-4c01-a42b-aa8438f6ce37)
- Choose any location, Ubuntu with version 24.04 and the cheapest option under Basic should be good enough.
- Choose Password Auth if unfamiliar with SSH keys
- Click create
  
## Obtain the bot (5 min)
Once you have a VM, you're going to want to install Docker. 
There's many ways to do this but you can use the following command: ```sudo snap install docker```

Next to clone the repo and navigate to it, run: 
```git clone https://github.com/Rfvooor/pump_fun_raydium_listings_sniper.git && cd pf_ray_list_snipe```

Before you continue, look at the .env file and fill it out, updating settings and your private key

Once docker is installed, you're going to want to build the image: ```sudo docker build -t pflistingsniper .```
Once downloaded you can run the bot: ```sudo docker run -t pflistingsniper```

*I used docker here as although you can nativly build/run in ts/js, raydium SDK is annoying in module format and I use a polyfil 
that is automatically applied in the docker version* 
    
## Feedback
I am very open to know what should be improved or what features you'd like to see.
Please put these here: https://github.com/Rfvooor/pump_fun_raydium_listings_sniper/issues
Or, if you aren't a github user, DM me on any of my socials and I'll add it!

## Donations
if this helped you pls donate here :)

3mjGMCWZNwSqKA3dpUrgciUEUaH2iNZZb8viapGJJpNk










