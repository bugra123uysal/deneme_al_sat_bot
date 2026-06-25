# Genel Bakis

## Problem

Her sabah bir pozisyon acmadan once surekli sekmeler arasinda gidip geliyordunuz:
TradingView'de endekslere, baska bir sekmede VIX'e, baskasinda sektorlere, baskasinda
du^nya borsalarina... Bunlarin hepsini bir arada, hizlica okuyabileceginiz tek bir sayfa yoktu.

Bu uygulama o problemi cozmek icin yapildi.

---

## Ne Yapiyor

Tek sayfa, tek bakis. Uygulama acildiginda su verileri otomatik ceker ve ekrana dizer:

### Gunluk Makro Ozet
S&P 500, Nasdaq, Dow Jones, Russell 2000, VIX, 10 yillik faiz, Dolar (DXY),
Altin, Petrol, Bitcoin -- hepsinin anlık degerini ve gunluk degisimini gosterir.
Yanında Risk-On / Risk-Off banner'i: endeksler yukari + VIX asagi ise yesil,
tersi ise kirmizi.

### Sektor Rotasyonu
11 sektorun hepsini (XLK, XLF, XLE, XLV, XLY, XLP, XLI, XLB, XLU, XLRE, XLC)
haftalık performansina gore siralanmis renk-kodlu grid olarak gosterir.
Hangi sektore para girip hangisinden cikiyor -- tek bakista.

### Dunya Borsalari
16 endeks, uc bolgeye ayrilmis: Amerika (S&P, Nasdaq, Russell, Bovespa),
Avrupa (FTSE, DAX, CAC, Euro Stoxx, BIST 100), Asya-Pasifik (Nikkei, KOSPI,
Hang Seng, Shanghai, Nifty, ASX).

### Piyasa Rejimi
S&P 500'un 200 gunluk hareketli ortalamas'in ustunde mi altinda mi oldugunu
gosterir. Yesil banner = bull rejim, kirmizi = bear rejim, sari = gecis.

### VIX Trend Grafigi
Son 5 gunun VIX kapanis degerlerini cizgi grafigi olarak gosterir.
20 altinda = dusuk korku, 20-30 arasi = orta, 30 ustu = panik bolgesi.

### Oncü Hisseler
NVDA, META, TSLA, AMZN, AAPL, MSFT -- piyasanin barometreleri.
Bu hisseler gucluyse genel piyasa sagliklidir.

### Gap-Up Tarayici (Buton)
Onceki kapanis fiyatinin %3 ustu acilis yapan hisseleri tarar.
Episodik Pivot adayi olabilecek hisseleri bulur.

### Hacim Anomalisi Tarayici (Buton)
20 gunluk ortalama hacminin 3 kati uzerinde islem goren hisseleri tarar.
Kurumsal para girisinin izini surmek icin kullanilir.

### Gunun Yorumu
Uygulamanin topladigi verilere dayanarak o gun icin duz yazı ile ozet yazar:
piyasa nasil? Risk var mi? Hangi sektore dikkat etmeli?




Tarayicida  https://genelbakis-j5hx65nam7p9cmv5sdx45f.streamlit.app/    adresine git.

---

## Teknoloji

- Python 3.10+
- Streamlit (arayuz)
- yfinance (Yahoo Finance'ten veri)
- pandas / numpy (hesaplamalar)
- plotly (grafikler)

Ucretli veri aboneligi gerekmez.

---

## Uyari

Bu uygulama egitim ve bilgilendirme amaclidir. Yatirim tavsiyesi degildir.
Gercek emir gondermez. Tum yatirim kararlari size aittir.

---

## Lisans

MIT
