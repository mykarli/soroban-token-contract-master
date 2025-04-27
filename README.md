# Soroban Token Contract (Freeze Özellikli)

Bu proje, Stellar Soroban SDK kullanılarak yazılmış temel bir Token Contract projesidir.  
**Freeze özelliği** eklenerek daha güvenli ve kontrol edilebilir hale getirilmiştir.

---

## 🛠 Özellikler

- **Token Başlatma (initialize)**: Admin belirleme, isim ve sembol atama.
- **Mint (mint)**: Yeni token üretimi.
- **Transfer (transfer)**: Token gönderimi.
- **Balance (balance)**: Adres bakiyesi sorgulama.
- **Allowance ve Approve**: Harcama yetkilendirme sistemi.
- **Transfer From (transfer_from)**: Harcama yetkilendirme üzerinden transfer işlemi.

---

## 🧩 Ekstra Eklenen Özellik: **Freeze Fonksiyonu**

Bu projeye ek olarak geliştirilmiştir:

- **freeze(address)** → Belirli bir adresi dondurur. Dondurulan adres token transfer edemez.
- **unfreeze(address)** → Dondurulan adresin transfer yapmasını tekrar açar.
- **is_frozen(address)** → Bir adresin donuk (frozen) durumda olup olmadığını kontrol eder.
- **transfer()** fonksiyonuna ekstra güvenlik katmanı eklendi:  
  Eğer gönderen adres **frozen** durumdaysa, transfer işlemi reddedilir.

### ➔ Bu sayede:
- Sistem daha güvenli olur.
- Kötü amaçlı transferler engellenebilir.
- Admin müdahalesi ile kriz anlarında adresler bloklanabilir.

---

## 🚀 Kullanım

Projeyi derlemek için:

```bash
cargo build

