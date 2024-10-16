# Copy number workshop


Use the following command to run rstudio using docker:

```
docker run --platform linux/x86_64 --rm -p 8787:8787 -e DISABLE_AUTH=true \
    -v `pwd`:`pwd` -v `pwd`/packages:/user-library -v `pwd`:/home/rstudio -w `pwd` \
    amcpherson/scworkshop:latest
```

Then navigate to localhost:8787 in your browser.

