# docker-wine-win32
The easiest way to run PE32 console files in docker

```
docker build -t my/wine:test .

docker run --rm -it --security-opt seccomp=unconfined -v /your_app.exe:/app.exe my/wine:test wine /app.exe
```
