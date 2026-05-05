# Gizlilik Politikası — 言響 仮名 (Kotohibi Kana)

**Yürürlük tarihi:** 4 Mayıs 2026
**Son güncelleme:** 4 Mayıs 2026
**Geliştirici:** Aisu Sensei
**İletişim:** aisuchanchan@gmail.com

---

## 1. Genel bakış

**言響 仮名 (Kotohibi Kana)** — Türkçe konuşan öğrenciler için Hiragana ve Katakana öğrenme uygulamasıdır. Bu uygulama:

- ✅ **Verilerinizi cihazınızda lokal olarak saklar** — kendi sunucumuz veya bulut depolama yoktur.
- ✅ **Reklam göstermez, analitik takibi yapmaz, üçüncü taraf izleme SDK'sı kullanmaz.**
- ✅ **Bilgilerinizi pazarlama amacıyla paylaşmaz veya satmaz.**
- ✅ **Hesabınızı uygulama içinden istediğiniz zaman silebilirsiniz.**

---

## 2. Hangi verileri işliyoruz?

### 2.1 Sizden topladıklarımız (cihazınızda saklanır)

| Veri | Ne zaman | Nerede saklanır |
|------|----------|-----------------|
| Adınız (kullanıcı adı) | Kayıt veya misafir girişi | Cihaz (AsyncStorage) |
| Şifre **(SHA-256 + tuz ile hash'lenmiş)** | Kayıt | Cihaz (AsyncStorage) |
| Öğrenme ilerlemeniz (XP, gün serisi, öğrendiğiniz karakterler, quiz istatistikleri) | Uygulamayı kullanırken | Cihaz (AsyncStorage) |
| Tema/maskot tercihiniz | Tercih değiştirdiğinizde | Cihaz (AsyncStorage) |

**Önemli:** Şifreler düz metin olarak saklanmaz. Cihazınızda tek yönlü hash + per-account rastgele tuz ile saklanır.

### 2.2 Google ile Giriş seçtiyseniz

Google ile giriş yaptığınızda, Google sizden onay aldığı kapsamda şu profil bilgilerini bize gönderir:

- E-posta adresiniz
- Ad/soyad
- Profil fotoğrafı URL'si
- Google hesap kimliği (Google ID)

Bu bilgiler **yalnızca cihazınızda** saklanır; harici bir sunucuya gönderilmez. Google'ın kendi gizlilik politikası: https://policies.google.com/privacy

### 2.3 Otomatik toplanan veriler

**Hiçbiri.** Konum, IP, cihaz kimliği, kullanım analitiği, çökme raporu — toplanmaz.

---

## 3. Verilerinizi neden işliyoruz?

| Amaç | İşlenen veri |
|------|-------------|
| Kullanıcıyı tanıma ve kişiselleştirilmiş ilerleme gösterme | Ad, e-posta (Google), öğrenme ilerlemesi |
| Şifre doğrulama | Şifre hash'i |
| Tema/maskot tercihinizi hatırlama | Tema ID |
| Günün karakteri özelliği | Tarih + rastgele seçilen kana |

Bu işlemlerin yasal dayanağı, KVKK md. 5/2(c) ve GDPR Art. 6(1)(b) uyarınca **sizinle yapılan sözleşmenin ifası** (uygulamayı size sunmak) ve Art. 6(1)(f) uyarınca **meşru menfaat** (uygulamanın çalışması).

---

## 4. Verileriniz kimlerle paylaşılıyor?

**Kimseyle.** Cihazınızdan dışarı çıkmaz.

**İstisna:** Google ile Giriş kullandığınızda, Google ile bir kimlik doğrulama (OAuth) alışverişi olur — bu Google'ın hizmeti gereğidir, biz Google'a sizinle ilgili ek veri göndermeyiz.

Yine teknik olarak:
- **Google Speech / Cihaz Sesi** (`expo-speech`) — kana telaffuzu için cihazınızın yerel ses motorunu kullanır. Yazılan metin işletim sistemine gönderilir; harici bir sunucuya gitmez.

---

## 5. Veriler ne kadar saklanıyor?

- **Hesabınızı silene kadar veya uygulamayı kaldırana kadar** cihazınızda saklanır.
- Hesabınızı sildiğinizde tüm kişisel verileriniz cihazdan kaldırılır (bkz. Bölüm 8).
- Uygulamayı kaldırırsanız, cihaz işletim sistemi AsyncStorage verilerini temizler.

---

## 6. Çocukların gizliliği

Bu uygulama 13 yaş ve üzeri kullanıcılar için tasarlanmıştır. 13 yaş altı çocuklardan bilerek veri toplamayız. Çocuğunuzun veri sağladığını düşünüyorsanız aisuchanchan@gmail.com adresinden bize bildirin; veriler derhal silinir.

---

## 7. Haklarınız

KVKK ve GDPR kapsamında şu haklara sahipsiniz:

- **Erişim**: Hangi verilerinizin işlendiğini öğrenme — uygulama içinde **Profil** ekranında zaten görünür.
- **Düzeltme**: Yanlış veriyi düzeltme — Profil ekranından adınızı/temanızı değiştirebilirsiniz.
- **Silme**: Hesabınızı ve tüm verilerinizi silme — bkz. Bölüm 8.
- **İtiraz**: Veri işlemeye itiraz etme — uygulamayı kaldırarak veya hesabınızı silerek.
- **Şikayet**: KVKK Kurumu'na (Türkiye) veya yerel veri koruma otoritenize başvurma.

Bu hakları kullanmak için aisuchanchan@gmail.com.

---

## 8. Hesabınızı nasıl silersiniz?

### 8.1 Uygulama içinden (önerilen yol)

1. Uygulamayı açın
2. Sağ üstteki **XP** rozetine veya alt sekmedeki Profil'e dokunun
3. **Hesap** bölümünde **❌ Hesabımı Sil** butonuna basın
4. İki adımlı uyarıyı onaylayın
5. Hesabınız ve tüm verileriniz **anında** cihazdan silinir

### 8.2 Uygulamaya erişiminiz yoksa (e-posta yoluyla)

aisuchanchan@gmail.com adresine şu bilgilerle e-posta atın:

- Konu: **"Hesap Silme Talebi — Kotohibi Kana"**
- Talep nedeniniz (zorunlu değil)
- Hesabınızda kullandığınız ad veya Google e-posta adresi

**Not:** Tüm verileriniz cihazınızda saklandığı için biz uzaktan veri silme yapamayız — sizin uygulamayı kaldırmanız gerekir. E-posta üzerinden talep aldığımızda size 7 gün içinde adım adım rehber göndeririz.

### 8.3 Tüm uygulamayı kaldırma

iOS/Android'de uygulamayı kaldırırsanız işletim sistemi tüm yerel verileri otomatik temizler.

---

## 9. Veri güvenliği

- Şifreler **SHA-256 + per-account rastgele 16-byte tuz** ile hash'lenir, asla düz metin saklanmaz.
- Google OAuth, endüstri standardı PKCE akışı ile yapılır.
- Veriler cihazınızda işletim sisteminin sandbox'unda saklanır; başka uygulamalar erişemez.

---

## 10. Politika değişiklikleri

Bu politikayı zaman zaman güncelleyebiliriz. Önemli değişikliklerde uygulama içinde bildirim göstereceğiz. "Son güncelleme" tarihi en üstte görünür.

---

## 11. İletişim

Sorularınız için: **aisuchanchan@gmail.com**

---
---

# Privacy Policy — 言響 仮名 (Kotohibi Kana)

**Effective date:** 4 May 2026
**Last updated:** 4 May 2026
**Developer:** Aisu Sensei
**Contact:** aisuchanchan@gmail.com

## 1. Overview

**言響 仮名 (Kotohibi Kana)** is a Hiragana and Katakana learning app for Turkish-speaking students. This app:

- ✅ **Stores your data locally on your device** — no servers, no cloud.
- ✅ **No ads, no analytics, no third-party tracking SDKs.**
- ✅ **Does not share or sell your information.**
- ✅ **You can delete your account from within the app at any time.**

## 2. What we process

### 2.1 Data you provide (stored on your device)

- Your name (username)
- Password — **stored as SHA-256 hash with per-account random salt**, never plain text
- Learning progress (XP, streak, learned characters, quiz statistics)
- Theme/mascot preference

### 2.2 If you sign in with Google

Google provides us with: email, name, profile picture URL, Google account ID. This is stored **only on your device**; not transmitted to any external server. Google's privacy policy: https://policies.google.com/privacy

### 2.3 Automatically collected

**None.** No location, IP, device ID, analytics, or crash reporting.

## 3. Why we process

To identify you, save your progress, verify your password (hashed), remember preferences, and provide the daily kana feature. Legal basis: contractual necessity (GDPR Art. 6(1)(b)) and legitimate interest (Art. 6(1)(f)).

## 4. Sharing

**No one.** Data does not leave your device, except for the OAuth handshake with Google when you choose to sign in with Google.

## 5. Retention

Until you delete your account or uninstall the app.

## 6. Children's privacy

For users 13+. We do not knowingly collect data from children under 13.

## 7. Your rights

Access, rectification, erasure, objection, complaint to data protection authority. Contact aisuchanchan@gmail.com.

## 8. How to delete your account

**In-app**: Profile → ❌ Delete My Account → confirm twice. Data is removed immediately.

**Via email**: Send to aisuchanchan@gmail.com with subject *"Account Deletion Request — Kotohibi Kana"* and your username or Google email. We will respond within 7 days. Note: since data is stored locally, you must uninstall the app for full data removal.

**Uninstall**: Removing the app deletes all local data via OS sandbox.

## 9. Security

Passwords are hashed (SHA-256 + 16-byte random salt). Google OAuth uses PKCE. Data is in OS sandbox storage.

## 10. Changes

We will notify you in-app of significant changes.

## 11. Contact

aisuchanchan@gmail.com
