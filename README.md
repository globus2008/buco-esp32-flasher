# BUCO ESP32 — Firmware Installer

Gateway firmware for the **ERQOS EQSP32** industrial controller (for example the EQSP32-CE). It
controls Somfy blinds, shutters, awnings and windows over the IB+ bus, over the SDN (RS485) bus,
or through Somfy TaHoma boxes (io-homecontrol, RTS), and connects them to building management
systems over BACnet, KNX, Modbus and Home Assistant. Configuration and control run in a web
interface built into the device — no app is needed; the internet or a cloud service is used only
by optional functions (for example TaHoma cloud accounts or the weather forecast). This is an
independent product, not affiliated with or endorsed by Somfy.

## Install the firmware (browser, no tools needed)

**→ Open the installer: <https://globus2008.github.io/buco-esp32-flasher/>**

1. Use **Google Chrome** or **Microsoft Edge** (Firefox/Safari don't support USB flashing).
2. Connect the EQSP32 to your computer with a **USB cable**.
3. Click **Install** on the page and select the serial port.
4. Wait ~2 minutes. Do not disconnect the device.

If no serial port appears, install the USB driver:
[CP210x](https://www.silabs.com/developer-tools/usb-to-uart-bridge-vcp-drivers) or
[CH340](https://www.wch-ic.com/downloads/CH341SER_ZIP.html).

The installer page asks you to accept the disclaimer before the installation is enabled.

**Note:** installing replaces the device's current configuration. Load/Save backups and stored
credentials (user accounts, Wi-Fi, e-mail, TaHoma) stay on the device: after the update, restore
the configuration with Settings → Options → Load/Save → Load. To keep a copy off the device as
well, use Copy to computer first.

## After installation

The device starts its own Wi-Fi access point — connect to it and open `http://192.168.4.1`, or
connect the device to your LAN via Ethernet and open `http://buco-esp32.local`.

## Updates

Later firmware versions are installed the same way, over USB from the installer page — this
updates the firmware and the web interface together. The device shows whether a newer version
exists under Settings → Options → System Settings → Update Firmware.

## Hardware

The EQSP32 controller (for example the EQSP32-CE) is available directly from
[erqos.com](https://erqos.com/product/eqsp32ce/).

---

<details>
<summary><strong>🇨🇿 Čeština</strong></summary>

Firmware brány pro průmyslový kontrolér **ERQOS EQSP32** (například EQSP32-CE). Ovládá žaluzie,
rolety, markýzy a okna Somfy po sběrnici IB+, po sběrnici SDN (RS485) nebo přes centrální jednotky
Somfy TaHoma (io-homecontrol, RTS) a propojuje je se systémy řízení budov přes BACnet, KNX, Modbus
a Home Assistant. Nastavení i ovládání probíhá ve webovém rozhraní přímo v zařízení — není potřeba
žádná aplikace; internet nebo cloudovou službu využívají jen volitelné funkce (například cloudové
účty TaHoma nebo předpověď počasí). Jde o nezávislý produkt, který není oficiálním výrobkem
společnosti Somfy.

**Instalace:** otevřete <https://globus2008.github.io/buco-esp32-flasher/> v prohlížeči Chrome
nebo Edge, připojte EQSP32 přes USB, klikněte na **Install** a vyberte sériový port. Instalace
trvá ~2 minuty; stránka nejprve vyžaduje souhlas s prohlášením o vyloučení odpovědnosti.
Instalace nahradí současnou konfiguraci, zálohy Load/Save a uložené přihlašovací údaje ale
v zařízení zůstanou: po aktualizaci konfiguraci obnovte přes Settings → Options → Load/Save → Load
(kopii mimo zařízení si můžete předem uložit přes Copy to computer). Pokud se port nezobrazí,
nainstalujte ovladač CP210x nebo CH340 (odkazy výše).

**Po instalaci:** zařízení vytvoří vlastní Wi-Fi síť — připojte se a otevřete
`http://192.168.4.1`, nebo přes Ethernet otevřete `http://buco-esp32.local`.

**Aktualizace:** další verze se instalují stejně, přes USB ze stránky instalátoru — aktualizuje se
tím firmware i webové rozhraní. Zda existuje novější verze, zobrazí zařízení v Settings → Options →
System Settings → Update Firmware.

</details>

<details>
<summary><strong>🇩🇪 Deutsch</strong></summary>

Gateway-Firmware für den Industriecontroller **ERQOS EQSP32** (zum Beispiel EQSP32-CE). Sie
steuert Somfy-Jalousien, -Rollläden, -Markisen und -Fenster über den IB+-Bus, über den SDN-Bus
(RS485) oder über Somfy-TaHoma-Boxen (io-homecontrol, RTS) und verbindet sie über BACnet, KNX,
Modbus und Home Assistant mit Gebäudeleitsystemen. Konfiguration und Bedienung erfolgen in einer im
Gerät integrierten Weboberfläche — eine App ist nicht nötig; Internet oder Cloud-Dienste nutzen nur
optionale Funktionen (zum Beispiel TaHoma-Cloud-Konten oder die Wettervorhersage). Dies ist ein
unabhängiges Produkt und kein offizielles Somfy-Produkt.

**Installation:** Öffnen Sie <https://globus2008.github.io/buco-esp32-flasher/> in Chrome oder
Edge, verbinden Sie den EQSP32 per USB, klicken Sie auf **Install** und wählen Sie den seriellen
Port. Die Installation dauert ~2 Minuten; die Seite verlangt vorher die Zustimmung zum
Haftungsausschluss. Die Installation ersetzt die aktuelle Konfiguration, Load/Save-Sicherungen und
gespeicherte Zugangsdaten bleiben jedoch auf dem Gerät: Stellen Sie die Konfiguration nach dem
Update über Settings → Options → Load/Save → Load wieder her (eine Kopie außerhalb des Geräts
können Sie vorher mit Copy to computer speichern). Erscheint kein Port, installieren Sie den
CP210x- oder CH340-Treiber (Links oben).

**Nach der Installation:** Das Gerät startet einen eigenen WLAN-Zugangspunkt — verbinden Sie
sich und öffnen Sie `http://192.168.4.1`, oder per Ethernet `http://buco-esp32.local`.

**Updates:** Spätere Versionen werden genauso installiert, per USB über die Installationsseite —
dabei werden Firmware und Weboberfläche gemeinsam aktualisiert. Ob eine neuere Version existiert,
zeigt das Gerät unter Settings → Options → System Settings → Update Firmware.

</details>

<details>
<summary><strong>🇫🇷 Français</strong></summary>

Firmware de passerelle pour le contrôleur industriel **ERQOS EQSP32** (par exemple l'EQSP32-CE).
Il commande les stores, volets, stores bannes et fenêtres Somfy via le bus IB+, via le bus SDN
(RS485) ou via des boîtiers Somfy TaHoma (io-homecontrol, RTS), et les relie aux systèmes de
gestion technique du bâtiment via BACnet, KNX, Modbus et Home Assistant. La configuration et la
commande se font dans une interface web intégrée à l'appareil — aucune application n'est
nécessaire ; Internet ou un service cloud ne sont utilisés que par des fonctions optionnelles (par
exemple les comptes cloud TaHoma ou les prévisions météo). Il s'agit d'un produit indépendant, non
affilié à Somfy.

**Installation :** ouvrez <https://globus2008.github.io/buco-esp32-flasher/> dans Chrome ou
Edge, connectez l'EQSP32 en USB, cliquez sur **Install** et sélectionnez le port série.
L'installation dure ~2 minutes ; la page demande d'abord d'accepter la clause de
non-responsabilité. L'installation remplace la configuration actuelle, mais les sauvegardes
Load/Save et les identifiants enregistrés restent dans l'appareil : après la mise à jour,
restaurez la configuration via Settings → Options → Load/Save → Load (une copie hors de l'appareil
peut être enregistrée au préalable avec Copy to computer). Si aucun port n'apparaît, installez le
pilote CP210x ou CH340 (liens ci-dessus).

**Après l'installation :** l'appareil crée son propre point d'accès Wi-Fi — connectez-vous et
ouvrez `http://192.168.4.1`, ou via Ethernet `http://buco-esp32.local`.

**Mises à jour :** les versions ultérieures s'installent de la même manière, en USB depuis la
page d'installation — le firmware et l'interface web sont mis à jour ensemble. L'appareil indique
si une version plus récente existe sous Settings → Options → System Settings → Update Firmware.

</details>

<details>
<summary><strong>🇭🇷 Hrvatski</strong></summary>

Firmware pristupnika za industrijski kontroler **ERQOS EQSP32** (na primjer EQSP32-CE). Upravlja
Somfy žaluzinama, roletama, tendama i prozorima preko IB+ sabirnice, preko SDN sabirnice (RS485)
ili preko Somfy TaHoma uređaja (io-homecontrol, RTS) te ih povezuje sa sustavima za upravljanje
zgradama preko BACnet, KNX, Modbus i Home Assistant. Konfiguracija i upravljanje odvijaju se u web
sučelju ugrađenom u uređaj — aplikacija nije potrebna; internet ili uslugu u oblaku koriste samo
opcionalne funkcije (na primjer TaHoma računi u oblaku ili vremenska prognoza). Ovo je neovisan
proizvod i nije službeni Somfy proizvod.

**Instalacija:** otvorite <https://globus2008.github.io/buco-esp32-flasher/> u Chromeu ili
Edgeu, spojite EQSP32 USB kabelom, kliknite **Install** i odaberite serijski port. Instalacija
traje ~2 minute; stranica prije toga traži prihvaćanje izjave o odricanju od odgovornosti.
Instalacija zamjenjuje trenutnu konfiguraciju, ali sigurnosne kopije Load/Save i spremljeni
pristupni podaci ostaju na uređaju: nakon ažuriranja vratite konfiguraciju putem Settings →
Options → Load/Save → Load (kopiju izvan uređaja možete prethodno spremiti pomoću Copy to
computer). Ako se port ne pojavi, instalirajte CP210x ili CH340 upravljački program (poveznice
iznad).

**Nakon instalacije:** uređaj pokreće vlastitu Wi-Fi pristupnu točku — spojite se i otvorite
`http://192.168.4.1`, ili preko Etherneta `http://buco-esp32.local`.

**Ažuriranja:** kasnije verzije instaliraju se na isti način, preko USB-a sa stranice za
instalaciju — time se zajedno ažuriraju firmware i web sučelje. Postoji li novija verzija, uređaj
prikazuje u Settings → Options → System Settings → Update Firmware.

</details>

<details>
<summary><strong>🇭🇺 Magyar</strong></summary>

Átjáró firmware az **ERQOS EQSP32** ipari vezérlőhöz (például az EQSP32-CE-hez). Somfy
redőnyöket, rolókat, napellenzőket és ablakokat vezérel az IB+ buszon, az SDN (RS485) buszon vagy
Somfy TaHoma központi egységeken keresztül (io-homecontrol, RTS), és BACnet, KNX, Modbus és Home
Assistant útján épületfelügyeleti rendszerekhez kapcsolja őket. A beállítás és a vezérlés az
eszközbe épített webes felületen történik — alkalmazás nem szükséges; internetet vagy
felhőszolgáltatást csak az opcionális funkciók használnak (például TaHoma felhőfiókok vagy az
időjárás-előrejelzés). Ez független termék, nem hivatalos Somfy termék.

**Telepítés:** nyissa meg a <https://globus2008.github.io/buco-esp32-flasher/> oldalt Chrome-ban
vagy Edge-ben, csatlakoztassa az EQSP32-t USB-kábellel, kattintson az **Install** gombra, és
válassza ki a soros portot. A telepítés kb. 2 percig tart; az oldal előtte a felelősségkizáró
nyilatkozat elfogadását kéri. A telepítés lecseréli az aktuális konfigurációt, a Load/Save mentések
és a tárolt hozzáférési adatok azonban az eszközön maradnak: a frissítés után állítsa vissza a
konfigurációt a Settings → Options → Load/Save → Load funkcióval (az eszközön kívüli másolatot
előtte a Copy to computer funkcióval mentheti). Ha a port nem jelenik meg, telepítse a CP210x vagy
CH340 illesztőprogramot (hivatkozások fent).

**Telepítés után:** az eszköz saját Wi-Fi hozzáférési pontot indít — csatlakozzon, és nyissa meg
a `http://192.168.4.1` címet, vagy Etherneten a `http://buco-esp32.local` címet.

**Frissítések:** a későbbi verziók ugyanígy, USB-n keresztül a telepítő oldalról telepíthetők —
ez a firmware-t és a webes felületet együtt frissíti. Hogy van-e újabb verzió, azt az eszköz a
Settings → Options → System Settings → Update Firmware menüben mutatja.

</details>

<details>
<summary><strong>🇵🇱 Polski</strong></summary>

Oprogramowanie bramy dla przemysłowego sterownika **ERQOS EQSP32** (na przykład EQSP32-CE).
Steruje żaluzjami, roletami, markizami i oknami Somfy przez magistralę IB+, magistralę SDN (RS485)
lub przez centrale Somfy TaHoma (io-homecontrol, RTS) i łączy je z systemami zarządzania budynkiem
przez BACnet, KNX, Modbus i Home Assistant. Konfiguracja i sterowanie odbywają się w interfejsie
webowym wbudowanym w urządzenie — aplikacja nie jest potrzebna; z internetu lub usługi chmurowej
korzystają tylko funkcje opcjonalne (na przykład konta chmurowe TaHoma lub prognoza pogody). Jest
to produkt niezależny, nie jest to oficjalny produkt firmy Somfy.

**Instalacja:** otwórz <https://globus2008.github.io/buco-esp32-flasher/> w Chrome lub Edge,
podłącz EQSP32 przez USB, kliknij **Install** i wybierz port szeregowy. Instalacja trwa ~2
minuty; strona najpierw wymaga akceptacji oświadczenia o wyłączeniu odpowiedzialności. Instalacja
zastępuje bieżącą konfigurację, ale kopie zapasowe Load/Save i zapisane dane dostępowe pozostają
w urządzeniu: po aktualizacji przywróć konfigurację przez Settings → Options → Load/Save → Load
(kopię poza urządzeniem możesz wcześniej zapisać za pomocą Copy to computer). Jeśli port się nie
pojawi, zainstaluj sterownik CP210x lub CH340 (linki powyżej).

**Po instalacji:** urządzenie uruchamia własny punkt dostępowy Wi-Fi — połącz się i otwórz
`http://192.168.4.1`, lub przez Ethernet `http://buco-esp32.local`.

**Aktualizacje:** kolejne wersje instaluje się tak samo, przez USB ze strony instalatora — to
aktualizuje jednocześnie oprogramowanie i interfejs webowy. Czy dostępna jest nowsza wersja,
urządzenie pokazuje w Settings → Options → System Settings → Update Firmware.

</details>

<details>
<summary><strong>🇸🇰 Slovenčina</strong></summary>

Firmvér brány pre priemyselný riadiaci systém **ERQOS EQSP32** (napríklad EQSP32-CE). Ovláda
žalúzie, rolety, markízy a okná Somfy cez zbernicu IB+, cez zbernicu SDN (RS485) alebo cez
centrálne jednotky Somfy TaHoma (io-homecontrol, RTS) a prepája ich so systémami riadenia budov
cez BACnet, KNX, Modbus a Home Assistant. Nastavenie aj ovládanie prebieha vo webovom rozhraní
priamo v zariadení — nie je potrebná žiadna aplikácia; internet alebo cloudovú službu využívajú len
voliteľné funkcie (napríklad cloudové účty TaHoma alebo predpoveď počasia). Ide o nezávislý
produkt, nie oficiálny produkt Somfy.

**Inštalácia:** otvorte <https://globus2008.github.io/buco-esp32-flasher/> v Chrome alebo Edge,
pripojte EQSP32 USB káblom, kliknite na **Install** a vyberte sériový port. Inštalácia trvá
~2 minúty; stránka najprv vyžaduje súhlas s vyhlásením o vylúčení zodpovednosti. Inštalácia
nahradí súčasnú konfiguráciu, zálohy Load/Save a uložené prihlasovacie údaje však v zariadení
zostanú: po aktualizácii konfiguráciu obnovte cez Settings → Options → Load/Save → Load (kópiu
mimo zariadenia si môžete vopred uložiť cez Copy to computer). Ak sa port nezobrazí, nainštalujte
ovládač CP210x alebo CH340 (odkazy vyššie).

**Po inštalácii:** zariadenie spustí vlastný prístupový bod Wi-Fi — pripojte sa a otvorte
`http://192.168.4.1`, alebo cez Ethernet `http://buco-esp32.local`.

**Aktualizácie:** ďalšie verzie sa inštalujú rovnako, cez USB zo stránky inštalátora —
aktualizuje sa tým firmvér aj webové rozhranie. Či existuje novšia verzia, zobrazí zariadenie
v Settings → Options → System Settings → Update Firmware.

</details>
