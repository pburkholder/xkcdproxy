# ComicProxy

Proxies traffic to https://xkcd.com via https://&lt;appname&gt;.app.cloud.gov

## Usage

Edit `prod_var.yml` and use your own name for the app. Then deploy the app:

```sh
cf push --vars-file prod_var.yml
```

Navigate to: https://&lt;appname&gt;.app.cloud.gov/2166, say, to see the _Stack_ comic.

## Authentication

None. Filters based on ingress IP address.
