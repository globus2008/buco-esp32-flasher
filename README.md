# BUCO ESP32 — Firmware Installer

IB+ Bus Gateway firmware for the **ERQOS EQSP32-CE** industrial controller. The gateway is
compatible with Somfy motor controllers (blinds, shutters, awnings), driving them over the RS485
IB+ bus, and provides a built-in web interface for configuration and control — no app, no cloud.
This is an independent product, not affiliated with or endorsed by Somfy.

## Install the firmware (browser, no tools needed)

**→ Open the installer: <https://globus2008.github.io/buco-esp32-flasher/>**

1. Use **Google Chrome** or **Microsoft Edge** (Firefox/Safari don't support USB flashing).
2. Connect the EQSP32 to your computer with a **USB cable**.
3. Click **Install** on the page and select the serial port.
4. Wait ~2 minutes. Do not disconnect the device.

If no serial port appears, install the USB driver:
[CP210x](https://www.silabs.com/developer-tools/usb-to-uart-bridge-vcp-drivers) or
[CH340](https://www.wch-ic.com/downloads/CH341SER_ZIP.html).

**Note:** installing erases all data on the device, including any previous configuration.

## After installation

The device starts its own Wi-Fi access point — connect to it and open `http://192.168.4.1`, or
connect the device to your LAN via Ethernet and open `http://buco-esp32.local`.

## Updates

Later firmware updates don't need USB: open the device's maintenance panel at
`http://<device-ip>:8000` and upload the `*-ota.bin` file from this repository (default
password `admin` — we recommend changing it with the [EQConnect](https://erqos.com/eqconnect/)
app).

## Hardware

The EQSP32-CE controller is available directly from [erqos.com](https://erqos.com/product/eqsp32ce/).

---

<details>
<summary><strong>🇨🇿 Čeština</strong></summary>

Firmware brány sběrnice IB+ pro průmyslový kontrolér **ERQOS EQSP32-CE**. Brána je kompatibilní
s motor controllery Somfy (žaluzie, rolety, markýzy), které ovládá po sběrnici RS485 IB+, a má
vestavěné webové rozhraní — bez aplikace, bez cloudu. Jde o nezávislý produkt, který není
oficiálním výrobkem společnosti Somfy.

**Instalace:** otevřete <https://globus2008.github.io/buco-esp32-flasher/> v prohlížeči Chrome
nebo Edge, připojte EQSP32 přes USB, klikněte na **Install** a vyberte sériový port. Instalace
trvá ~2 minuty a smaže veškerá data v zařízení. Pokud se port nezobrazí, nainstalujte ovladač
CP210x nebo CH340 (odkazy výše).

**Po instalaci:** zařízení vytvoří vlastní Wi-Fi síť — připojte se a otevřete
`http://192.168.4.1`, nebo přes Ethernet otevřete `http://buco-esp32.local`.

**Aktualizace:** další aktualizace už USB nevyžadují — nahrajte soubor `*-ota.bin` přes servisní
panel na `http://<ip-zařízení>:8000` (výchozí heslo `admin`, doporučujeme změnit v aplikaci
EQConnect).

</details>

<details>
<summary><strong>🇩🇪 Deutsch</strong></summary>

IB+-Bus-Gateway-Firmware für den Industriecontroller **ERQOS EQSP32-CE**. Das Gateway ist mit
Somfy-Motorsteuerungen (Jalousien, Rollläden, Markisen) kompatibel und steuert sie über den
RS485-IB+-Bus; es bietet eine integrierte Weboberfläche — ohne App, ohne Cloud. Dies ist ein
unabhängiges Produkt und kein offizielles Somfy-Produkt.

**Installation:** Öffnen Sie <https://globus2008.github.io/buco-esp32-flasher/> in Chrome oder
Edge, verbinden Sie den EQSP32 per USB, klicken Sie auf **Install** und wählen Sie den seriellen
Port. Die Installation dauert ~2 Minuten und löscht alle Daten auf dem Gerät. Erscheint kein
Port, installieren Sie den CP210x- oder CH340-Treiber (Links oben).

**Nach der Installation:** Das Gerät startet einen eigenen WLAN-Zugangspunkt — verbinden Sie
sich und öffnen Sie `http://192.168.4.1`, oder per Ethernet `http://buco-esp32.local`.

**Updates:** Spätere Updates benötigen kein USB — laden Sie die Datei `*-ota.bin` über das
Wartungspanel unter `http://<geräte-ip>:8000` hoch (Standardpasswort `admin`, Änderung per
EQConnect-App empfohlen).

</details>

<details>
<summary><strong>🇫🇷 Français</strong></summary>

Micrologiciel de passerelle bus IB+ pour le contrôleur industriel **ERQOS EQSP32-CE**. La
passerelle est compatible avec les contrôleurs de moteurs Somfy (stores, volets, bannes) qu'elle
pilote via le bus RS485 IB+, et offre une interface web intégrée — sans application, sans cloud.
Il s'agit d'un produit indépendant, non affilié à Somfy.

**Installation :** ouvrez <https://globus2008.github.io/buco-esp32-flasher/> dans Chrome ou
Edge, connectez l'EQSP32 en USB, cliquez sur **Install** et sélectionnez le port série.
L'installation dure ~2 minutes et efface toutes les données de l'appareil. Si aucun port
n'apparaît, installez le pilote CP210x ou CH340 (liens ci-dessus).

**Après l'installation :** l'appareil crée son propre point d'accès Wi-Fi — connectez-vous et
ouvrez `http://192.168.4.1`, ou via Ethernet `http://buco-esp32.local`.

**Mises à jour :** les mises à jour ultérieures ne nécessitent plus d'USB — téléversez le
fichier `*-ota.bin` via le panneau de maintenance sur `http://<ip-appareil>:8000` (mot de passe
par défaut `admin`, changement recommandé via l'application EQConnect).

</details>

<details>
<summary><strong>🇭🇷 Hrvatski</strong></summary>

Firmware IB+ sabirničkog pristupnika za industrijski kontroler **ERQOS EQSP32-CE**. Pristupnik
je kompatibilan sa Somfy motornim kontrolerima (žaluzine, rolete, tende) kojima upravlja preko
RS485 IB+ sabirnice i ima ugrađeno web sučelje — bez aplikacije, bez oblaka. Ovo je neovisan
proizvod i nije službeni Somfy proizvod.

**Instalacija:** otvorite <https://globus2008.github.io/buco-esp32-flasher/> u Chromeu ili
Edgeu, spojite EQSP32 USB kabelom, kliknite **Install** i odaberite serijski port. Instalacija
traje ~2 minute i briše sve podatke na uređaju. Ako se port ne pojavi, instalirajte CP210x ili
CH340 upravljački program (poveznice iznad).

**Nakon instalacije:** uređaj pokreće vlastitu Wi-Fi pristupnu točku — spojite se i otvorite
`http://192.168.4.1`, ili preko Etherneta `http://buco-esp32.local`.

**Ažuriranja:** kasnija ažuriranja ne zahtijevaju USB — prenesite datoteku `*-ota.bin` preko
servisnog panela na `http://<ip-uređaja>:8000` (zadana lozinka `admin`, preporučujemo promjenu
putem aplikacije EQConnect).

</details>

<details>
<summary><strong>🇵🇱 Polski</strong></summary>

Oprogramowanie bramy magistrali IB+ dla przemysłowego sterownika **ERQOS EQSP32-CE**. Brama
jest kompatybilna ze sterownikami silników Somfy (żaluzje, rolety, markizy), którymi steruje
przez magistralę RS485 IB+, i ma wbudowany interfejs webowy — bez aplikacji, bez chmury. Jest to
produkt niezależny, nie jest to oficjalny produkt firmy Somfy.

**Instalacja:** otwórz <https://globus2008.github.io/buco-esp32-flasher/> w Chrome lub Edge,
podłącz EQSP32 przez USB, kliknij **Install** i wybierz port szeregowy. Instalacja trwa ~2
minuty i usuwa wszystkie dane z urządzenia. Jeśli port się nie pojawi, zainstaluj sterownik
CP210x lub CH340 (linki powyżej).

**Po instalacji:** urządzenie uruchamia własny punkt dostępowy Wi-Fi — połącz się i otwórz
`http://192.168.4.1`, lub przez Ethernet `http://buco-esp32.local`.

**Aktualizacje:** kolejne aktualizacje nie wymagają USB — wgraj plik `*-ota.bin` przez panel
serwisowy pod adresem `http://<ip-urządzenia>:8000` (domyślne hasło `admin`, zalecamy zmianę w
aplikacji EQConnect).

</details>
