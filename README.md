# WolfOS

*In short: WolfOS is a Polish-language desktop Linux distribution based on Arch Linux, made by DarkWolf. It aims to be easy to use, hard to break (btrfs snapshots before every update) and ready for gaming and local AI on AMD, NVIDIA and Intel graphics. This repository is the update server of WolfOS: the Releases contain the signed pacman packages that `wolf update` downloads. Licence: Apache-2.0. Artwork (wallpapers, logos) is not included.*

Stworzone przez **DarkWolf**.

## Czym jest WolfOS

WolfOS to dystrybucja Linuksa oparta na Arch Linux: nowoczesna, szybka, a jednocześnie prosta w obsłudze. Ma pokazać, że system z najświeższym jądrem i sterownikami nie musi wymagać nauki pacmana ani ręcznego naprawiania po każdej aktualizacji.

## Do czego służy

- **Codzienna praca i gry.** Steam z Protonem, Heroic (Epic, GOG), Lutris, MangoHud, GameMode, a dla kart AMD także LACT. Gotowe do instalacji jednym kliknięciem w Centrum Wilka.
- **Lokalne AI.** ROCm, Ollama i LM Studio na kartach AMD (i zestawy sterowników dla NVIDIA oraz Intel).
- **Stabilność.** System plików btrfs i migawki (snapper) przed każdą aktualizacją. Gdy coś się zepsuje, `wolf back` albo wpis w menu startowym przywracają stan sprzed niej. Dwa jądra: najnowsze i LTS w zapasie.
- **Prywatność.** Telemetria wyłączona w Firefoksie i narzędziach AI, zapora sieciowa (ufw) włączona od razu.

## Najważniejsze cechy

- **Instalator graficzny** krok po kroku: dysk, pulpit, sterowniki karty graficznej (AMD, Intel, NVIDIA, wykrywane automatycznie), konto (także bez hasła, z automatycznym logowaniem). Obsługuje tylko UEFI i czyści wybrany dysk.
- **Pulpity:** KDE Plasma (zalecany), GNOME albo COSMIC. Edycja **Lite** z pulpitem Xfce na słabsze komputery (od 2 GB RAM).
- **Polecenie `wolf`** zamiast nauki pacmana: `wolf install`, `wolf update`, `wolf back`, `wolf search`, `wolf remove`. Obsługuje repozytoria Archa, AUR i Flathub.
- **Centrum Wilka:** aktualizacje, migawki, programy (wyszukiwarka i gotowe grupy), zapora, tryb zasilania, Bluetooth, stan kart graficznych.
- Bluetooth, tryby zasilania, zram, Flatpak z Flathubem skonfigurowane od startu.

## Aktualizacje

WolfOS aktualizuje się w miejscu (model „rolling”), nie trzeba instalować nowej wersji. Pliki samego WolfOS (polecenie `wolf`, Centrum Wilka, motyw, ustawienia) są pakietami pacmana w repozytorium `wolfos`, które leży w wydaniu tego repozytorium. Wszystko aktualizuje jedno polecenie:

```
wolf update
```

Pakiety są podpisane kluczem projektu (`wolfos-keyring`), a system przyjmuje tylko poprawnie podpisane.

## Status

Projekt jest w budowie i testowany głównie w maszynach wirtualnych. Używasz go na własną odpowiedzialność, a instalator czyści wybrany dysk, więc najpierw wypróbuj system w trybie live. Obrazy ISO nie są tu publikowane (są zbyt duże, a repozytorium służy jako serwer aktualizacji). Kod źródłowy jest na razie rozwijany lokalnie.

## Licencja

Kod i konfiguracja WolfOS (narzędzia, instalator, Centrum Wilka, skrypty, ustawienia) są na licencji **Apache License 2.0** (plik `LICENSE`).

- **Tapety i logo nie są częścią tego repozytorium ani wydań** i nie są objęte tą licencją.
- WolfOS korzysta z Arch Linux i oprogramowania innych autorów, które pozostaje na ich własnych licencjach.
- Projekt jest niezależny i nie jest powiązany z Arch Linux. Nazwy i znaki towarowe należą do ich właścicieli.

## Autor

**DarkWolf**
