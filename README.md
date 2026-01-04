# 🚗 Araç Kiralama Otomasyon Sistemi

Bu proje, araç kiralama şirketlerinin araç takibini, kiralama işlemlerini ve gelir yönetimini kolaylaştırmak amacıyla geliştirilmiş, **Python** tabanlı bir masaüstü uygulamasıdır.

Veriler **JSON** tabanlı bir veritabanı yapısında tutulur, bu sayede kurulum gerektirmeden çalışır ve veriler kalıcı olarak saklanır.

## 🚀 Özellikler

Uygulama, modüler bir yapıda tasarlanmış olup şu temel fonksiyonlara sahiptir:

* **Araç Yönetimi:** Sisteme yeni araç ekleme, mevcut araç bilgilerini düzenleme ve silme.
* **Kiralama İşlemleri:** Müsait araçları kiralama, müşteri adı ve tarih bilgilerini girerek işlemi başlatma.
* **Otomatik Hesaplamalar:**
    * İki tarih arasındaki gün sayısını hesaplama.
    * Günlük ücret üzerinden toplam kiralama bedelini otomatik çıkarma.
* **İade Süreci:** Kiradaki aracı iade alma ve durumunu tekrar "Müsait"e çevirme.
* **Görsel Takip:** Listede müsait araçlar **yeşil**, kiradaki araçlar **kırmızı** arka plan ile gösterilir.
* **Veri Kalıcılığı:** Program kapatılsa bile tüm kayıtlar `araclar.json` dosyasında saklanır.

## 🛠 Kullanılan Teknolojiler ve Kütüphaneler

Proje tamamen Python ile geliştirilmiştir ve şu kütüphaneleri kullanır:

* **Tkinter:** Grafiksel Kullanıcı Arayüzü (GUI) tasarımı.
* **JSON:** Verilerin dosya tabanlı olarak saklanması.
* **Datetime:** Tarih farkı ve gün hesaplamaları.

## 📂 Proje Yapısı

Kodun yönetilebilirliğini artırmak için **Modüler Mimari** kullanılmıştır:

* `main.py`: Uygulamanın başlatıldığı ana dosya.
* `arayuz.py`: Tüm görsel pencereler, butonlar ve tablo işlemlerinin olduğu sınıf.
* `hesaplamalar.py`: Tarih kontrolü ve ücret hesaplama gibi matematiksel işlemler.
* `dosya_islemleri.py`: JSON dosyasını okuma ve yazma işlemlerini yöneten katman.
* `araclar.json`: Araç ve kiralama verilerinin tutulduğu veri dosyası.

## 💻 Kurulum ve Çalıştırma

Projeyi bilgisayarınızda çalıştırmak için:

1.  Bu depoyu indirin (`git clone` veya Zip olarak).
2.  Bilgisayarınızda Python'un kurulu olduğundan emin olun.
3.  Terminal veya komut satırında proje klasörüne gelin.
4.  Aşağıdaki komutu çalıştırın:

```bash
python main.py
