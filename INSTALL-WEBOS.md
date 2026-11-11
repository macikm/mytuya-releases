# Instalace Smart Dashboard na LG webOS

Smart Dashboard otevře https://mytuya.com z nabídky aplikací televizoru. Vyžaduje připojení k internetu a je přizpůsobený ovladači LG Magic Remote.

## Co potřebujete

- Televizi LG s webOS a počítač ve stejné síti.
- Bezplatný účet [LG Developer](https://webostv.developer.lge.com/).
- [webOS Dev Manager pro Windows, macOS nebo Linux](https://github.com/webosbrew/dev-manager-desktop/releases/latest).
- Soubor `.ipk` z části **Assets** příslušného [release](https://github.com/macikm/mytuya-releases/releases). Archivy Source code nejsou instalační balíčky.

## 1. Připravte televizi

V LG Content Store / Apps nainstalujte aplikaci **Developer Mode**. Spusťte ji a přihlaste se účtem LG Developer.

Zapněte **Dev Mode Status**. Po restartu televize znovu otevřete Developer Mode a zapněte **Key Server**. Poznamenejte si IP adresu a zobrazený kód **Passphrase**.

## 2. Připojte počítač

Spusťte webOS Dev Manager a přidejte televizi v režimu Developer Mode. Zadejte IP adresu a podle průvodce kód Passphrase. Rozlišují se velká a malá písmena.

Pokud jsou vyžadované další údaje, port je `9922` a uživatelské jméno `prisoner`.

## 3. Nainstalujte aplikaci

V sekci **Apps** vyberte **Install / Install App** a otevřete stažený soubor `.ipk`.

Po dokončení spusťte **Smart Dashboard** z nabídky aplikací na televizi a postupujte podle přihlášení na obrazovce.

## Platnost Developer Mode

Vývojářský režim má omezenou platnost. Zbývající čas je v poli **Remain Session**. Před vypršením připojte TV k internetu a stiskněte **EXTEND**.

Po vypršení a vypnutí Developer Mode při restartu televize aplikace nainstalované tímto způsobem odinstaluje. Pak je nutné režim znovu zapnout a aplikaci znovu nainstalovat.

## Když se nedaří

Zkontrolujte IP adresu, zapnutý Key Server a stejnou síť. Síť pro hosty může komunikaci mezi zařízeními blokovat. Při potížích s načítáním dashboardu ověřte internetové připojení TV.

[Podrobný návod na webu](https://www.martinmacko.cz/mytuya-dashboard/instalace-lg-webos/) | [Dokumentace Developer Mode od LG](https://webostv.developer.lge.com/develop/getting-started/developer-mode-app)
