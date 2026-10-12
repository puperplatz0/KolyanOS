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
| **Готов к играм** | Steam, Wine, Gamemode, MangoHud — из коробки |
| **Лёгкий** | Xfce + минимум фоновых процессов |
| **Быстрый** | Загрузка прямо в рабочий стол, без логинов |
| **AUR из коробки** | `yay` предустановлен, ставь что угодно |
| **Swap на изи** | Скрипт создания swap-файла одной командой |
| **Красивый** | Собственный брендинг, тёмная тема, обоями от KolyanOS |

---

## Что внутри

**Оконная среда**
- Xfce 4 + Xfce Goodies
- LightDM + GTK Greeter

**Гейминг**
- Steam
- Wine + Winetricks
- Gamemode (lib32 тоже)
- MangoHud (lib32 тоже)
- Vulkan: AMD, Intel (lib32 тоже)
- Mesa (lib32 тоже)

**Инструменты**
- Firefox
- Konsole
- Dolphin
- Ark
- btop
- yay (AUR-хелпер)

**Драйверы**
- xf86-video-amdgpu
- xf86-video-intel
- xf86-video-nouveau
- linux-firmware + amd/intel microcode

---

## Установка

### Скачать

Последний релиз: [**Releases**](https://github.com/puperplatz0/KolyanOS/releases)

ISO разбит на части (ограничение GitHub в 2 ГБ на файл).

### Windows

1. Скачай **все части** `.part_*` и `merge.bat`
2. Положи всё в одну папку
3. Запусти `merge.bat` двойным кликом
4. Получишь `KolyanOS-0.0.2.iso`
5. Запиши его на флешку (8 ГБ+) через [balenaEtcher](https://etcher.balena.io/)
6. Загрузись с флешки

### Linux

```bash
# Склеиваем части
cat KolyanOS-0.0.2.iso.part_* > KolyanOS-0.0.2.iso

# Записываем на флешку (замени /dev/sdX на свою!)
sudo dd if=KolyanOS-0.0.2.iso of=/dev/sdX bs=4M status=progress oflag=sync
