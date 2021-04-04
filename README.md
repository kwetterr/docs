![logo](./assets/logo_full.png)



<h1 align="center">Official documentation for Kwetter.</h1>
<h3 align="center">
  <a href=""md">Contribute</a>
  <span> · </span>
  <a href="">Community</a>
  <span> · </span>
  <a href="">Documentation</a>
</h3>

## Structure
| Codebase                                                      |      Description          | 
| :-----------------------------------------------------------: | :-----------------------: | 
| [docs](https://github.com/kwetterr/docs)                      | Official Documentation    |
| [ui](https://github.com/kwetterr/ui)                          | VueJS front-end           |
| [user-service](https://github.com/kwetterr/user-service)      | .NET core API             |
| [friend-service](https://github.com/kwetterr/friend-service)  | .NET core API             |
| [kwat-service](https://github.com/kwetterr/kwat-service)      | NodeJS API                |

## Contributions
Checkout our quickstart in [CONTRIBUTING.md](CONTRIBUTING.md) and checkout out individual repositories next.

## Quickstart with Docker
<b>Prerequisites</b>
- [Docker](docker.com)
```zsh
mkdir Kwetterr && cd Kwetterr
 
git clone https://github.com/kwetterr/docs
git clone https://github.com/kwetterr/ui
git clone https://github.com/kwetterr/user-service
git clone https://github.com/kwetterr/friend-service
git clone https://github.com/kwetterr/kwat-service
```

Run all microservices at once.
```zsh
docker-compose build
docker-compose up
```

## Quickstart with Kubernetes
<b>Prerequisites</b>
- [Kubernetes](kubernetes.io)
- Make sure to copy `.env.example` and create `.env` with the filled in values.

Build all images.
```zsh

cd user-service
docker build -t user-service .
cd ..

cd kwat-service
docker build -t kwat-service .
cd ..

#docker build -t friend-service .
cd ui
docker build -t ui .
cd ..
```
### Note
If you get the error `zsh: command not found:` allow comments with:
```zsh
set -k
```