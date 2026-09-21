# AD Atlas

**Active Directory saldırı yollarını uygulamalı bir CTF zinciri olarak anlatan, tek dosyalık çevrimdışı eğitim sunumu.**

Nmap → Responder → SMB Relay → Initial Access → Local PrivEsc → Credential Dumping →
BloodHound → Kerberoasting → ACL/DACL → Shadow Credentials → Pass-the-Hash/Ticket →
PsExec/WMI/WinRM → DCSync → Golden Ticket — ve ek AD saldırıları (AS-REP Roasting,
MITM6, GPO Abuse, SIDHistory, Skeleton Key). Her konu **nasıl oluşur → lab uygulaması →
tespit ve önleme** akışıyla işlenir.

## Kullanım

Kurulum yok, sunucu yok, internet yok:

**[`index.html`](index.html) dosyasını indir ve çift tıkla.** Tarayıcıda tamamen
çevrimdışı açılır — tüm görseller, stiller ve kod tek dosyanın içinde gömülüdür.

> İndirmek için: yukarıdaki `index.html`'e tıkla → **Download raw file** (indirme ikonu).
> Ya da tüm repoyu **Code → Download ZIP** ile indir.

### Klavye kısayolları

| Tuş | İşlev |
| --- | --- |
| `←` `→` / `Space` | Slayt değiştir |
| `A` | Konu listesini aç |
| `F` / `F11` | Tam ekran |

## ⚠️ Sorumluluk reddi

Bu içerik **yalnızca eğitim ve yetkili güvenlik testi** amaçlıdır. Sunumdaki tüm makine
adları, IP adresleri, alan adları ve örnek çıktılar **izole bir eğitim laboratuvarına**
aittir; gerçek bir sisteme ait kimlik bilgisi içermez. Anlatılan teknikleri yalnızca
**sahibi olduğunuz veya açık yazılı izniniz olan** sistemlerde uygulayın.

## Teknik

Tek `index.html`: React tek-sayfa uygulaması, tüm CSS/JS ve görseller (base64) gömülü.
Herhangi bir modern tarayıcıda `file://` üzerinden çalışır.
