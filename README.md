# Platinum Financial Applications Archive

> Архив установочных файлов **Platinum Financial Applications** для MS-DOS / ранних PC-систем, включая модуль Premier Inter-Company Processing и русскоязычные дополнения.

[![Archive](https://img.shields.io/badge/type-software%20archive-2f80ed)](#содержимое)
[![Platform](https://img.shields.io/badge/platform-MS--DOS-lightgrey)](#как-использовать)
[![Version](https://img.shields.io/badge/readme-3.02--4.01-green)](#что-известно)
[![Status](https://img.shields.io/badge/status-preserved-yellow)](#дисклеймер)

## О репозитории

Этот репозиторий сохраняет старый комплект **Platinum Financial Applications**: установщик, служебные файлы, модуль `PLATINUM`, архивы русификации/дополнений и справочные материалы.

Папка в репозитории называется [`Platinum Financial Aplications/`](Platinum%20Financial%20Aplications/) с оригинальной опечаткой `Aplications`. Имя оставлено как есть, чтобы не ломать структуру старого комплекта.

## Что известно

Из файла [`PLATINUM/README.IL`](Platinum%20Financial%20Aplications/PLATINUM/README.IL):

- продукт: **PLATINUM PREMIER INTER-COMPANY PROCESSING**;
- версии, упомянутые в README: `3.02`, `3.02 rev a`, `4.00`, `4.01`;
- даты из README: 1992-12-16, 1993-06-15, 1994-03-01, 1994-06-01;
- совместимость: Premier General Ledger / Platinum applications версии `3.02` или новее.

## Содержимое

| Раздел | Что внутри |
| --- | --- |
| `INSTALL.EXE`, `PKUNZIP.EXE`, `FILES.INS`, `INDATA.INS` | основной установочный комплект |
| `PLATINUM/` | модуль Premier Inter-Company Processing и README.IL |
| `PLATINUM/PRMCON/PRMCON.ZIP` | дополнительный архив модуля |
| `Дополнения/` | русскоязычные дополнения и отдельный установщик |
| `Дополнения/2/` | дополнительные ZIP-пакеты, HLP и PDF-ресурсы |
| `CHECKSUMS.txt` | SHA-256 суммы файлов архива |
| `FILES.md` | подробная карта файлов репозитория |

## Структура

```text
.
├── CHECKSUMS.txt
├── FILES.md
├── README.md
└── Platinum Financial Aplications/
    ├── INSTALL.EXE
    ├── PKUNZIP.EXE
    ├── PLATINUM/
    │   ├── README.IL
    │   ├── ILINTERC.EXZ
    │   └── PRMCON/
    │       └── PRMCON.ZIP
    └── Дополнения/
        ├── APRUS.ZIP
        ├── ARRUS.ZIP
        └── 2/
            ├── PLRUS.ZIP
            ├── PO_RUS.ZIP
            ├── RUS_EXE0.ZIP
            └── PLATINUM/
                ├── HELP/
                └── RESOURCE/
```

## Как использовать

1. Работайте с файлами в изолированной среде: DOSBox, виртуальная машина или отдельный тестовый DOS-носитель.
2. Перед запуском проверьте файлы по [`CHECKSUMS.txt`](CHECKSUMS.txt).
3. Начинайте с основного установщика:

```text
Platinum Financial Aplications/INSTALL.EXE
```

4. Русскоязычные дополнения находятся в:

```text
Platinum Financial Aplications/Дополнения/
```

## Контрольные суммы

Проверить отдельный файл в PowerShell:

```powershell
Get-FileHash -Algorithm SHA256 -LiteralPath "Platinum Financial Aplications\INSTALL.EXE"
```

Полный список SHA-256 находится в [`CHECKSUMS.txt`](CHECKSUMS.txt).

## Дисклеймер

Репозиторий является архивной копией старого программного обеспечения. Файлы предоставлены для сохранения, изучения и восстановления legacy-сред. Все права на Platinum Financial Applications, утилиты, документацию и торговые марки принадлежат их законным правообладателям.

Запускайте старые исполняемые файлы только в безопасной изолированной среде.
