#  Ucus ve Pilot Yonetim Sistemi

N11 Java Bootcamp kapsamında hazırlanmış OOP ödevidir.  
Amaç, uçuş ve pilot yönetimini UML Class Diagram ile modellemektir.

##  Açıklama
- Uçuşlar, hava yolu şirketleri tarafından gerçekleştirilir  
- Her uçuş: 1 uçak, 1 pilot ve 1 yardımcı pilot içerir  
- Uçuşların kalkış ve varış havaalanları vardır  
- Uçaklar farklı tiplerde olabilir ve durum bilgisi taşır  

##  UML İlişkileri
```text
HavaYoluSirketi 1 ---- 0..* Ucus
HavaYoluSirketi 1 ---- 0..* Ucak
HavaYoluSirketi 1 ---- 0..* Pilot

Ucak 0..* ---- 1 UcakTipi

Ucus 0..* ---- 1 Ucak
Ucus 0..* ---- 1 Havaalani : kalkisHavaalani
Ucus 0..* ---- 1 Havaalani : varisHavaalani
Ucus 0..* ---- 1 Pilot : pilot
Ucus 0..* ---- 1 Pilot : yardimciPilot
```
<img width="1195" height="685" alt="Ekran Resmi 2026-04-23 ÖS 7 48 31" src="https://github.com/user-attachments/assets/d87b932b-f7ca-45d7-b9eb-dedd70fc7d6c" />
