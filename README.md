# Docker for unionpay php

## PREPARE

Perpare docker vol folder

```bash
mkdir -p ~/vol/unionpay/
mkdir ~/vol/unionpay/files/
mkdir ~/vol/unionpay/logs/
```

Copy file to vol folder

```
unzip assets
cp -r assets/web ~/vol/unionpay/
cp -r assets/certs ~/vol/unionpay/
```

## RUN

```bash
docker run -d --rm --name php -v ~/vol/unionpay:/opt/ -p 9000:9000 playniuniu/unionpay-php
```

Visit url: [http://127.0.0.1:9000/upacp_demo_b2b/index_02_b2b.php](http://127.0.0.1:9000/upacp_demo_b2b/index_02_b2b.php)
