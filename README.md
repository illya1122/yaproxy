# yaproxy

Yet Another Proxy — инструмент, который автоматически:
- скачивает списки прокси
- проверяет SOCKS5 прокси
- выбирает наиболее стабильный и быстрый
- предоставляет готовый рабочий прокси

## Возможности

- Автоматическая загрузка proxy-листов
- Проверка SOCKS5 прокси
- Фильтрация по скорости и доступности
- Выбор наиболее стабильного прокси
- CLI-использование
- Возможность сборки в исполняемый файл

## Скомпилировать

#### Linux / macOS

```bash
git clone https://github.com/illya1122/yaproxy.git
cd yaproxy
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
python yaproxy.py
````

#### Windows

```bat
git clone https://github.com/illya1122/yaproxy.git
cd yaproxy
python -m venv venv
venv\Scripts\activate
pip install -r requirements.txt
python yaproxy.py
```

## Установка скомпилированной программы

#### Linux x86

```bash
curl -L -o yaproxy https://github.com/illya1122/yaproxy/releases/download/v1.1/yaproxy-linux-x86-64
chmod +x yaproxy
./yaproxy
```

#### macOS (intel)

```bash
curl -L -o yaproxy https://github.com/illya1122/yaproxy/releases/download/v1.1/yaproxy-mac-x86-64
chmod +x yaproxy
./yaproxy
```

#### Linux arm (aarch64)

```bash
curl -L -o yaproxy https://github.com/illya1122/yaproxy/releases/download/v1.1/yaproxy-linux-aarch64
chmod +x yaproxy
./yaproxy
```

#### Windows

```bash
wget https://github.com/illya1122/yaproxy/releases/download/v1.1/yaproxy-windows-x86-64.exe -O yaproxy.exe
yaproxy.exe
```

Программа:

* скачивает proxy-листы
* проверяет SOCKS5 прокси
* выводит лучший доступный прокси

## Принцип работы

1. Загружаются публичные proxy-листы
2. Извлекаются SOCKS5 прокси
3. Каждый прокси проверяется на доступность и задержку
4. Выбирается наиболее стабильный и быстрый

## Лицензия

MIT License
