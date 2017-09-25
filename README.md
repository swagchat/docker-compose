# Deploy swagchat in a local environment

swagchat is an open source chat components for your apps.

If you are deploying swagchat quickly in a local environment, we recommend using docker-compose.

Please install docker-compose beforehand. ([Install Docker Compose](https://docs.docker.com/compose/install/))


We prepared three patterns for deployment.

### Lv1: Very simple deploy (rosetta)

Only Chat API and RTM API. Use SQLite for datastore.


```
git clone git@github.com:fairway-corp/swagchat-docker-compose.git
cd swagchat-docker-compose/1-rosetta
docker-compose up
```
Please open example.html in browser when deployment is completed.


### Lv2: Use MySQL (panther)

Use MySQL for datastore.

```
git clone git@github.com:fairway-corp/swagchat-docker-compose.git
cd swagchat-docker-compose/2-panther
docker-compose up
```
Please open example.html in browser when deployment is completed.

### Lv3: Use MySQL & NSQ (jackson)

Use MySQL for datastore and NSQ for realtime messeging que.

```
git clone git@github.com:fairway-corp/swagchat-docker-compose.git
cd swagchat-docker-compose/3-jackson
docker-compose up
```
Please open example.html in browser when deployment is completed.


## License

MIT License.
