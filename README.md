# steem price feed 
steem price feed for witness. It's written in Node.JS

## basic
* Use coinmarketcap api.
* Use Nods.JS
* Package dependencies : request, steem

## install
Download the git repository, then edit config.json.
```
git clone https://github.com/koinbot/steempricefeed.git
cd steempricefeed
npm install
cp config.example.json config.json
nano config.json
```

## config
name : "your steem acoount name"  
wif : "your steem private key"  
interval : minute 

e.g.
```
{
    "name": "koinbot",
    "wif": "5J********************",
    "interval": 60
}
```


## run
```node feedprice.js```  
or  
```forever start feedprice.js```  //A simple CLI tool for ensuring that a given script runs continuously

