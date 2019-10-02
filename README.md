# curl-http3-docker

## Contains

* CURL
* BoringSSL (HTTP3 Patch)
* Brotli
* NgHTTP2
* Cloudflare Quiche

## How to use

### Example

The base command when starting the container is `curl`. An example of a curl command could be:

```
curl -svo /dev/null --http3 https://cloudflare-quic.com/
```

When using this container the command would be:

```
docker run --rm -it theh00k/curl-http3 -svo /dev/null --http3 https://cloudflare-quic.com/
```

Bash Integration

To add this as a local command you can add the following to your `.bashrc`

```
alias curl3="docker run --rm -it theh00k/curl-http3"
```

This will allow you to use:

```
curl3 -svo /dev/null --http3 https://cloudflare-quic.com/
```
