# Get curl with Docker

The docker image is hosted at <https://hub.docker.com/r/curlimages/curl>

You can run the latest version of curl with the following command:

```sh
docker run -it --rm curlimages/curl www.example.com
```

## Running curl seamlessly in docker

It is possible to make an alias to seamlessly run curl inside a container.
Define an alias like the following:

```sh
# Bash alias example
alias curl='docker run -it --rm curlimages/curl'
```

And simply invoke `curl www.example.com` to make a request
