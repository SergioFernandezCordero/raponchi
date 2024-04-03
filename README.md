# Raponchi
Just stupid, fake and absolutely futile information about frogs

## To run

### Setup the following environment variables:

- TIMEZONE: Timezone. Defaults to system timezone
- LOGLEVEL: Log level. Defaults to INFO
- FROGWORD: Keyword to be used. Defaults to "rana"
- PATH_TO_FROGS: Temporary path where frog images will be stored. Defaults to "dataset"
- FROG_NUMBER: Number of frog images downloaded in each batch. Defaults to 5
- FROG_SCHEDULER_INTERVAL: How frequently the scheduler will poll for pending jobs. Defaults to 30 seconds
- FROG_NAMES_URL: Online source for frog names. Should be a URL to a plain text file with names, one per line.
- TW_CONSUMER_KEY: Twitter Consumer Key
- TW_CONSUMER_SECRET: Twitter Consumer Secret
- TW_ACCESS_TOKEN: Twitter Access Token
- TW_ACCESS_TOKEN_SECRET: Twitter Access Token Secret
- ELK_URL: URL of ElasticSearch cluster used to send logs. TLS assumed. If ELK_URL and ELK_PORT are defined, ELK logger will be configured.
- ELK_PORT: Port of the ElasticSearch cluster used to send logs. If ELK_URL and ELK_PORT are defined, ELK logger will be configured.
- ELK_INDEX: Name of the index used to store logs. Defaults to raponchi-log

### Install dependencies:

```
pip install -r requirements.txt
```

### An run:

```
python raponchi.py
```

### Further resources

See [tweepy](https://docs.tweepy.org/en/stable/index.html) documentation for further information, you lazy
