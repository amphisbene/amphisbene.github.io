# Tools

## Add a new post

```bash
cp _posts/2022-09-06-welcome.md _posts/$(echo -n $(date +%Y-%m-%d)-title.md)
```

## Test this blog locally

```bash
docker run --rm \
    -v "$PWD:/srv/jekyll:Z" \
    -p 4000:4000 \
    jekyll/jekyll \
    jekyll serve

curl http://[::1]:4000/
```

# About this blog
This blog uses Reverie, by Amit Merchant.
