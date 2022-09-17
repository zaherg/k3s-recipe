Me learning K3s 🤷‍♂️

You can deploy all of them by running `deploy` from the command line, but you need to be careful

> You need to create a new `deployment.yml` file for cloudflare and add your own token

## Available recipe

1. for Redis, check [redis-deployment](redis/).
2. for Postgres, check [postgres-deployment](postgres/).
3. for MySQL, check [mysql-deployment](mysql/).
4. for Rethinkdb, check [rethinkdb-deployment](rethinkdb/).
4. for Meilisearch, check [meilisearch-deployment](meilisearch/).
5. for Cloudflare Tunnel, check [cloudflare-deployment](cloudflare/).
6. for n8n Server, check [n8n-deployment](n8n/).
7. for fider Server, check [fider-deployment](fider/).
8. for fider Server, check [mastodon-deployment](mastodon/).

> **Note**
> 1. Remember to create the required databases for: `n8n`,  `fider` and `mastodon` !!!
> 2. The deploy script won't deploy `mastodon` automatically you have to do it manually.

## Server structure

I have no specific instruction on how you need to build your own cluster, but it is recommened that you have at least 3 nodes, it is better if you colsulte the [architecture](https://rancher.com/docs/k3s/latest/en/architecture/) section on K3s docs.


## Note:
I have got the base from [Pi4Cluster](https://rpi4cluster.com/k3s/k3s-redis/?utm_source=github&utm_id=zaher/k3s-recipe) guide about deploying redis to k3s, and then used it to build my own recipe for both Postgres and MySQL.

So thanks to [Vladimir Strycek](https://rpi4cluster.com/?utm_source=github&utm_id=zaher/k3s-recipe) and his valuable site.