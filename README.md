<div align="center">
  <img src="https://example.com/asterisk_logo.png" alt="Asterisk Logo">
</div>

# Asterisk AMI Listener Python Script

[![License](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Python Version](https://img.shields.io/badge/Python-3.x-green.svg)](https://www.python.org/downloads/)
[![Dependencies](https://img.shields.io/badge/Dependencies-py__asterisk__ami%2C%20mysql--connector--python-orange)](https://pypi.org/project/py-asterisk-ami/)
[![MariaDB Version](https://img.shields.io/badge/MariaDB-%3E%3D%2010.0-yellow.svg)](https://mariadb.org/)

Bu Python scripti, Asterisk Manager Interface (AMI) üzerinden gelen olayları (events) dinleyen ve bu olayları MariaDB veritabanına yazan bir uygulamadır.

## 🚀 Kurulum

1. Python 3.x sürümünü bilgisayarınıza kurun, eğer kurulu değilse: [Python Resmi Websitesi](https://www.python.org/downloads/)

2. Gerekli Python paketlerini yükleyin. Terminal veya Komut İstemcisinde aşağıdaki komutu çalıştırın:
```bash
pip install py_asterisk_ami mysql-connector-python
```

MariaDB veritabanı sunucusu üzerinde bir veritabanı oluşturun ve gerekli tabloları oluşturmak için db_schema.sql dosyasını kullanın.

▶️ Kullanım

ami_listener.py dosyasını çalıştırın:

Script, Asterisk AMI'yi dinlemeye başlayacak ve gelen olayları (events) dinleyecektir.

Gelen olaylar MariaDB veritabanına cdr tablosuna yazılacaktır.

⚙️ Ayarlar
Scriptin çalışması için bazı ayarları yapılandırabilirsiniz:

- AMI_HOST: Asterisk AMI sunucu adresi veya IP adresi.
- AMI_PORT: Asterisk AMI sunucu portu (genellikle 5038).
- AMI_USERNAME: Asterisk AMI kullanıcı adı.
- AMI_PASSWORD: Asterisk AMI kullanıcı şifresi.
- DB_HOST: MariaDB veritabanı sunucu adresi veya IP adresi.
- DB_PORT: MariaDB veritabanı sunucu portu (genellikle 3306).
- DB_USERNAME: MariaDB veritabanı kullanıcı adı.
- DB_PASSWORD: MariaDB veritabanı kullanıcı şifresi.
- DB_DATABASE: MariaDB veritabanı adı.
B
u ayarları ami_listener.py dosyasının başında bulunan değişkenleri düzenleyerek yapabilirsiniz.

📄 Lisans
Bu proje, MIT Lisans altında lisanslanmıştır.
