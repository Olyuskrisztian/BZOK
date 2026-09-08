 # Hálózati terv dokumentáció

## Csapattagok

* Ölyüs Krisztián (pm)
* Budai Zoltán

---

## A cég bemutatása

**Cégnév:** **ReworkTech Kft.**

A ReworkTech Kft. egy informatikai vállalat, amely számítógépes hálózatok tervezésével és kiépítésével, számítógépek javításával, valamint informatikai támogatással foglalkozik. A cég célja, hogy ügyfelei számára megbízható és biztonságos informatikai megoldásokat biztosítson.

A vállalat összesen **20 alkalmazottat** foglalkoztat, akik különböző részlegeken dolgoznak, például vezetőség, adminisztráció, ügyfélszolgálat, szerviz és informatikai részleg. A cég négy telephelyen működik Magyarországon: Budapesten található a központi iroda, emellett Pécsen, Rotterdamban és Szegeden is rendelkezik irodával.

A ReworkTech Kft. modern hálózati eszközöket használ, és nagy hangsúlyt fektet a gyors, biztonságos és megbízható működésre. A telephelyeket egy közös vállalati hálózat köti össze, így az alkalmazottak könnyen elérhetik a szükséges adatokat és szolgáltatásokat.

## A telephelyek

### 1. Budapest – Központi iroda (Székhely)

Ez a vállalat központja, ahol a vezetőség, az adminisztráció és a szerverek találhatók. Innen irányítják a cég működését.

**Helyiségek:**

* Vezetőségi iroda
* Titkárság
* Adminisztrációs iroda
* Informatikai iroda
* Szerverhelyiség

### 2. Pécsi iroda

A pécsi telephely az ügyfélszolgálatért és az értékesítésért felel. A munkatársak itt fogadják az ügyfeleket és kezelik a megrendeléseket.

**Helyiségek:**

* Ügyfélszolgálati iroda
* Értékesítési iroda
* Vezetői iroda
* Tárgyaló

### 3. Rotterdam szervizközpont

A debreceni telephelyen történik a számítógépek javítása, karbantartása és az alkatrészek raktározása.

**Helyiségek:**

* Alkatrészraktár
* Informatikai iroda
* Vezetői iroda
* Tesztlabor

### 4. Szegedi fejlesztőközpont

A szegedi telephelyen dolgoznak a szoftverfejlesztők és a rendszergazdák. Itt készülnek a vállalat saját programjai és hálózati megoldásai.

**Helyiségek:**

* Fejlesztői iroda
* Rendszergazdai iroda
* Projektmenedzseri iroda
* Vezetői iroda
* Szerverterem

## Tervezett hálózati eszközök

A vállalat hálózatának kiépítéséhez az alábbi hálózati eszközöket tervezzük használni:

* 4 db Router (telephelyenként 1 db)
* 8 db 24 portos Switch
* 20 db Asztali számítógép (PC)
* 8 db Laptop
* 2 db Szerver

  * 1 db DHCP/DNS szerver
  * 1 db Fájlszerver
* 4 db Hálózati nyomtató
* 4 db Wi-Fi Access Point
* 1 db Hardveres tűzfal (Cisco ASA)
* 4 db Rack szekrény
* Cat6 UTP kábelek
* Hálózati kábelrendezők
* Optikai kábel a telephelyek közötti WAN kapcsolat kialakításához
* Hálózati rack polcok
* Szerver szekrény
* Internet modem

## Tervezett technológiák

A hálózat működéséhez az alábbi technológiák kerülnek alkalmazásra:

### Redundancia

A budapesti központban két switch és két router biztosítja a hálózat folyamatos működését. Meghibásodás esetén a másik eszköz automatikusan átveszi a feladatokat.

### IPv4

A vállalat belső hálózatában IPv4 címzést használunk. Minden telephely külön IP-hálózatot kap, így egyszerűbb a hálózat kezelése és az eszközök azonosítása.

### IPv6

A hálózat támogatja az IPv6 címzést is, amely lehetővé teszi a jövőbeni bővítést és a modern hálózati eszközök használatát.

### DHCP

A DHCP szerver automatikusan kiosztja az IP-címeket a számítógépeknek és egyéb hálózati eszközöknek. Ennek köszönhetően nem kell minden eszközön kézzel beállítani a hálózati adatokat.

### DNS

A DNS szerver a domainneveket IP-címekké alakítja, így a felhasználóknak nem kell IP-címeket megjegyezniük a hálózati szolgáltatások eléréséhez.

### Ethernet

A telephelyeken a számítógépek és a hálózati eszközök vezetékes Ethernet kapcsolaton keresztül csatlakoznak a switch-ekhez, ami gyors és stabil adatátvitelt biztosít.

### Wi-Fi

Minden telephelyen vezeték nélküli hálózat is működik, amelyet az alkalmazottak laptopokkal és mobil eszközökkel használhatnak. A Wi-Fi hálózat jelszóval védett.

### OSPF (dinamikus útválasztás)

A telephelyek routerei OSPF dinamikus útválasztási protokollt használnak. Ez automatikusan frissíti az útvonalakat, ha a hálózatban változás történik.

### Statikus útválasztás (Static Routing)

Bizonyos útvonalakat kézzel állítunk be a routereken, hogy egyszerűbb legyen a kisebb hálózatok közötti kommunikáció.

### Statikus NAT

A statikus NAT segítségével a szerverek állandó publikus IP-címen érhetők el az internet felől.

### Dinamikus NAT (PAT)

A dolgozók számítógépei dinamikus NAT-ot (PAT) használnak, így több belső eszköz is ugyanazon nyilvános IP-címen keresztül tud csatlakozni az internethez.

### ACL (Access Control List)

Az ACL szabályok segítségével szabályozható, hogy mely felhasználók vagy eszközök férhetnek hozzá bizonyos hálózati erőforrásokhoz, ezzel növelve a hálózat biztonságát.

### VPN

Az otthon dolgozó alkalmazottak VPN kapcsolaton keresztül biztonságosan tudnak csatlakozni a vállalati hálózathoz, így távolról is elérhetik a szükséges adatokat.

### WAN kapcsolat

A négy telephely WAN kapcsolaton keresztül csatlakozik egymáshoz, így az alkalmazottak bármelyik irodából elérhetik a központi szervereket és a vállalati szolgáltatásokat.

### Hardveres tűzfal

A vállalat hálózatát egy hardveres tűzfal védi, amely kiszűri a nem engedélyezett hálózati forgalmat és segít megakadályozni a külső támadásokat.

## Biztonság

A hálózat biztonságát az alábbi megoldások biztosítják:

* ACL szabályok
* Hardveres tűzfal
* VPN kapcsolat
* Jelszóval védett Wi-Fi hálózat (WPA2/WPA3)
* Rendszeres biztonsági mentések

## WAN kapcsolat

A négy telephely WAN kapcsolaton keresztül csatlakozik egymáshoz, így az alkalmazottak bármelyik irodából elérhetik a központi szervereket.

## VPN

Az otthon dolgozó alkalmazottak VPN kapcsolaton keresztül biztonságosan tudnak csatlakozni a vállalati hálózathoz.

## Biztonság

A hálózat biztonságát az alábbi megoldások biztosítják:

* ACL szabályok
* Hardveres tűzfal
* VLAN-ok
* VPN
* Jelszóval védett Wi-Fi hálózat

## Összegzés

A ReworkTech Kft. hálózata négy telephelyből áll, amelyeket WAN kapcsolatok kötnek össze. A budapesti központban több VLAN működik, a hálózat IPv4 és IPv6 címzést is használ, valamint statikus és dinamikus útválasztást valósít meg. A VPN kapcsolat, az ACL-ek és a hardveres tűzfal gondoskodnak a hálózat biztonságáról. A kialakított infrastruktúra megbízható, könnyen bővíthető és megfelel egy modern informatikai vállalat igényeinek.
