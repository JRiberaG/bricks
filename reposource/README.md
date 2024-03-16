# Reposource

This brick generates boilerplate code for remote and local data sources, as well as repositories. It's meant to be used within a Flutter project following BlueBird architecture.


## Setup 🧑‍💻
Ensure you have the mason_cli installed.

```sh
# 🎯 Activate from https://pub.dev
dart pub global activate mason_cli
```

```sh
# 🍺 Or install from https://brew.sh
brew tap felangel/mason
brew install mason
```


## Installation ☁️

```sh
# Install locally
mason add reposource \
  --git-url https://www.github.com/jriberag/bricks \
  --git-path reposource \
  --git-ref 77397c40dbd92c80f28059c6d4fd0e549f4a8b11
```

```sh
# Install globally
mason add -g reposource \
  --git-url https://www.github.com/jriberag/bricks \
  --git-path reposource \
  --git-ref 77397c40dbd92c80f28059c6d4fd0e549f4a8b11
```


## Usage 🚀

```sh
mason make reposource -o features/<your_feature>/lib/src/
```

## Output 📦

```

--name Auth

.
├── data/
│   ├── datasources/
│   │   ├── local/
│   │   │   ├── auth_local_datasource.dart
│   │   │   └── auth_local_datasource_impl.dart
│   │   ├── remote/
│   │   │   ├── auth_remote_datasource.dart
│   │   │   └── auth_remote_datasource_impl.dart
│   │   └── datasources.dart
│   ├── models/
│   │   ├── requests/
│   │   │   └── base_auth_request_model.dart
│   │   ├── responses/
│   │   │   └── base_auth_response_model.dart
│   │   └── models.dart
│   └── repositories/
│       ├── local/
│       │   └── auth_local_repository_impl.dart;
│       ├── remote/
│       │   └── auth_remote_repository_impl.dart;
│       └── data_repositories.dart
└── domain/
    ├── entities/
    │   └── entities.dart
    └── repositories/
        ├── local/
        │   └── auth_local_repository.dart;
        ├── remote/
        │   └── auth_remote_repository.dart;
        └── domain_repositories.dart
```
