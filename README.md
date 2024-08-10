# Overview
Provides the one-click scriptes of Docker compose containers and related configuration.

## Directory structure
```
web-playground
├─ playground-infrastructure
   ├─ playground-{}
   │  ├─ docker-compose.yml
   │  ├─ .env
   │  ├─ run.bat
   │  ├─ run.sh
   │  └─ sql (Optional)
   │  │  └─ init.sql  
   │  └─ ...
   ├─ ...
   ├─ .env
   ├─ docker-compose.yml
   ├─ run.bat
   └─ run.sh
```

* `playground-{}`: `{}` means some technology stack
  * `docker-compose.yml`: Docker compose yaml
  * `.env`: The `.env` file provides environment variables for `{}` technology stack
  * `run.bat`: The one-click bat script for Windows
  * `run.sh`: The one-click shell script for Linux
  * `sql`: *Optional*. Directory to store sql scripts.

## Usage
### One-click start a complete development environment
* For Windows
``` sh
cd .\playground-infrastructure\
.\run.bat
```

* For Linux
``` sh
cd .\playground-infrastructure\
.\run.sh
```

### One-click start specific technology stack
Take mysql as an example

* For Windows
``` sh
cd .\playground-infrastructure\playground-mysql\
.\run.bat
```

* For Linux
``` sh
cd .\playground-infrastructure\playground-mysql\
.\run.sh
```