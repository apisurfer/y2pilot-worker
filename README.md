# y2pilot Cloudflare worker

y2pilot is a smart YouTube playlist manager app. You can [try it out here](https://y2pilot.com)

This worker serves as API for fetching Youtube oembed data and for persisting playlists to Cloudflare's KV store.
Codebase of the frontend app written in Vue can be found here: [lvidakovic/y2pilot](https://github.com/lvidakovic/y2pilot)

I decided to share this as open source even though it's far from a solid and clean codebase. It was developed over a long stretch of time, in my spare time and as a first experimental project in Cloudflare Workers.

In case you decide to tamper with it, fork it, extend it or submit a PR don't hesitate to reach out and ask questions. I'll be happy to answer and help if need be, currently I don't have time to rethink and refactor the codebase.


## Local setup

```
cp wrangler.toml-example wrangler.toml
# create your Cloudflare Worker and KV namespaces
# set Cloudflare account, worker and namespace IDs inside your wrangler.toml file
npm install
```

### Compiles and reloads for development

```
npm run dev
```

To deploy to prod follow official Wrangler documentation(Wrangler CLI).
