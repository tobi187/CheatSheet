
## Beim Builden schägt Verbindung zu APT fehl
[Lösung von](https://medium.com/@faithfulanere/solved-docker-build-could-not-resolve-archive-ubuntu-com-apt-get-fails-to-install-anything-9ea4dfdcdcf2)

```bash
docker build --network=host .
```