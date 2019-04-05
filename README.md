# docker-verdaccio-s3

This is a Private NPM container that can backup to s3 (or any object storage provider compatible with s3a)

The container will sync content down upon starting, and perform a backup sync every 5 minutes.

```
docker run  --name verdaccio \ 
            -e S3_BUCKET=<s3 bucket name> \
            -p 80:4873 \
            teamxinc/verdaccio-s3-github
```


## Required Environment Variables

| Variable Name | Example Value |
|---------------|---------------|
| GITHUB_OAUTH_ORG |  |
| GITHUB_OAUTH_CLIENT_ID |  |
| GITHUB_OAUTH_CLIENT_SECRET |  |