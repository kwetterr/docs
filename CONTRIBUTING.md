![logo](./assets/logo_full.png)
# Contributing to Kwetter
We love your input! We want to make contributing to this project as easy and transparent as possible, whether it's:
- Reporting an issue
- Discussing the current state of the code
- Submitting a fix
- Proposing new features

## Code of Conduct
The code of conduct is described in [`CODE_OF_CONDUCT.md`](CODE_OF_CONDUCT.md).

## Commiting
This project is using the [conventional commits](https://www.conventionalcommits.org/en/v1.0.0-beta.2/) standard. Please follow these steps to ensure your
commit messages are standardized.

## Pull Requests
1. Fork the repo and create your branch in lowercase with a descriptive name.
2. Add some test examples.
3. Ensure to describe your pull request.

## Quickstart Local Development
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

### Note
For running individual services checkout their own repositories.
