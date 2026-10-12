<div align="center">

# KolyanOS

**Лёгкий геймерский дистрибутив на базе Arch Linux**

[![Arch Linux](https://img.shields.io/badge/base-Arch%20Linux-1793D1?style=for-the-badge&logo=arch-linux&logoColor=white)](https://archlinux.org)
[![License](https://img.shields.io/badge/license-GPL-green?style=for-the-badge)](LICENSE)

[Скачать](https://github.com/puperplatz0/KolyanOS/releases) · [Баги](https://github.com/puperplatz0/KolyanOS/issues) · [Обсуждения](https://github.com/puperplatz0/KolyanOS/discussions)

</div>

---

## Что такое KolyanOS?

**KolyanOS** — минималистичный геймерский дистрибутив, созданный для тех, кто хочет **играть, а не настраивать систему**. Никаких лишних процессов в фоне, никаких «сюрпризов» — только то, что нужно для игр и работы.

В основе — **Arch Linux**, одна из самых гибких и производительных систем в мире. Поверх — лёгкая **Xfce**, которая не жрёт ресурсы, оставляя их играм.

---

## Особенности

| | |
|---|---|
| **Готов к играм** | Steam, Wine, Gamemode, MangoHud из коробки |
| **Лёгкий** | Xfce + минимум фоновых процессов |
| **Быстрый** | Загрузка прямо в рабочий стол, без логинов |
| **AUR из коробки** | `yay` предустановлен |
| **Swap на изи** | Скрипт создания swap-файла одной командой |
| **Красивый** | Собственный брендинг, тёмная тема |

---

## Что внутри

**Оконная среда**
- Xfce 4 + Xfce Goodies
- LightDM + GTK Greeter

**Програмки**
- Firefox
- Konsole
- Dolphin
- Ark
- btop
- yay (AUR-хелпер)

---

## Установка

### Windows

1. Скачай **все части** `.part_*` и `merge.bat`
2. Положи всё в одну папку
3. Запусти `merge.bat`
4. Получишь `KolyanOS-версия_сборки.iso`

### Linux

```bash
cat KolyanOS-версия_сборки.iso.part_* > KolyanOS-версия_сборки.iso
```
