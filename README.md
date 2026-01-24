<div align="center">

# 🐙 B3rou Git Rehberi
### "Komutları ezberleme. Zamanı bükmeyi öğren."

<p>
  <a>Neden?</a> •
  <a>Müfredat</a> •
  <a>Nasıl Çalışır?</a>
</p>

![Git-Header-Visual](https://img.shields.io/badge/Status-Interactive_Learning-success?style=for-the-badge)
![Lang](https://img.shields.io/badge/Language-Turkish-red?style=for-the-badge)

<br>

> *"Git, sadece kodunuzu kaydettiğiniz bir depo değildir. <br>Git, hatalarınızdan dönmenizi sağlayan bir zaman makinesidir."*

</div>

---

## Önsöz: Karanlık Terminalden Korkma
İnternette yüzlerce Git kaynağı var. Çoğu sana *"Commit atmak için `git commit` yaz"* der. Ama sana şunları söylemezler:
* "Yanlış branch'e push atarsan o paniği nasıl yönetirsin?"
* "`HEAD detached` olduğunda kodların silindi mi sanıyorsun?"
* "Bir `merge conflict` gördüğünde bilgisayarı kapatıp kaçmalı mısın?"

Bu rehber, **ezberci bir sözlük** değildir. Rehberin Türkçe olmasını bir eksi değil de artı olarak görmeni istiyorum. Anadilinde rahatça öğrenirken ingilizce yönünü de unutmayan bir materyal hazırladım. Bu materyali gönül rahatlığıyla kendin/derslerin/öğrencilerin için kullanabilirsin.

Burada sadece komutları değil; bir takımın parçası olmayı, repoyu temiz tutmayı ve tarihi (history) korkusuzca manipüle etmeyi öğreneceksin.

---

## Nasıl Kullanılır? (Simülasyon Mantığı)
Bu repo, statik bir ders notu değildir. Burası interaktif bir **Laboratuvar**.

1.  **Lobi (Main Branch):** Şu an bulunduğun yer. Burada teoriyi okuyacak, kahveni yudumlayacaksın.
2.  **Görev Odaları (Mission Branches):** Her dersin sonunda seni özel bir branch'e davet edeceğim.
    * *Örnek:* `git checkout mission/conflict-101`
    * O branch'e geçtiğin an, bulunduğun dünya değişecek. Dosyalar bozulacak, tarihler karışacak.
3.  **Medkit (İlk Yardım):** Eğer görevde sıkışırsan, ana merkezden yardım çağırabileceksin.

---

## 📖 Müfredat: Sıfırdan "Maintainer" Seviyesine (Ya Da Profesyonelliğe)

### Bölüm 1: Genesis (Doğuş)
Terminali açıyoruz, alet çantamızı kuruyoruz ve ilk izimizi bırakıyoruz.
* **[1.0 - Kurulum ve Konfigürasyon](./docs/1-genesis/1.0-kurulum-ve-ayarlar.md)**
    * *Windows, MacOS ve Linux Kurulumu ve Farkları*
    * *Author Bilgisi (`user.name`, `user.email`)*
* **[1.1 - Git'in Felsefesi](./docs/1-genesis/1.1-git-teorisi.md)**
    * *Snapshot vs Delta (Git neden farklı?)*
    * *Git'in Düşünce Yapısı*
    * *The Three States (Çalışma, Sahne, Depo)*
* **[1.2 - İlk Temas](./docs/1-genesis/1.2-ilk-commit.md)**
    * *`git init`: Evreni Yaratmak*
    * *`git add` & `git commit`: Tarihi Mühürlemek*
* **[1.3 - .gitignore](./docs/1-genesis/1.3-gitignore.md)**
    * *.gitignore Dosyası ile Gereksizleri Görmezden Gelmek*
    * *`git rm --cached`: Takibi Silmek*
* **[1.4 - Yetenek Ağacım: Bölüm Özeti](./docs/1-genesis/1.4-bolum-ozeti.md)**
    * *Bu Bölümde Neler Öğrendik?*
    * *Hızlı bir Bakış: Kavramlar Sözlüğü*

### Bölüm 2: Multiverse (Branching)
Tek bir çizgide gitmek zorunda değilsin. Paralel evrenler yarat.
* **[2.0 - Branch Anatomisi](./docs/2-multiverse/2.0-branch-mantigi.md)**
    * *Pointer nedir? HEAD nereye bakıyor?*
    * *Branch oluşturma ve geçiş yapma*
* **[2.1 - Birleştirme Sanatı (Merge)](./docs/2-multiverse/2.1-merge-ve-conflict.md)**
    * *Fast-Forward vs 3-Way Merge*
    * *Conflict (Çakışma) Yönetimi ve Temizliği*
* **[2.2 - Gelişmiş Branch Teknikleri](./docs/2-multiverse/2.2-gelismis-branching.md)**
    * *`stash`: Dağınık masayı toplamadan misafir ağırlamak.*
    * *`orphan`: Geçmişi olmayan, köksüz dallar yaratmak.*
    * *Branch temizliği: Silme ve düzenleme.*

### Bölüm 3: Time Travel (Zaman Manipülasyonu)
Hata yaptın. Sorun değil, geçmişi değiştirebiliriz.
* **[3.0 - Geri Alma Komutları](./docs/3-time-travel/3.0-geri-almak.md)**
    * *`checkout` (Gözlemci Modu)*
    * *`revert` (Güvenli Geri Alma)*
    * *`reset` (Yıkıcı Geri Alma - Soft, Mixed, Hard)*
* **[3.1 - Tarihi Yeniden Yazmak](./docs/3-time-travel/3.1-gelismis-history.md)**
    * *`amend`: Son sözü değiştirmek*
    * *`rebase`: Tarihi düzleştirmek*
    * *`cherry-pick`: Newton'u değil, yalnızca ihtiyacın olan elmayı almak.*
* **[3.2 - The Safety Net (Güvenlik Ağı)](./docs/3-time-travel/3.2-reflog.md)**
    * *`reflog`: Silinen commitleri mezardan çıkarmak (Git'in kara kutusu).*

### Bölüm 4: Remote (Uzak Depolar)
Kodun artık sadece senin bilgisayarında değil.
* **[4.0 - GitHub ile Dans](./docs/4-remote/4.0-remote-temelleri.md)**
    * *SSH Key Kurulumu*
    * *Remote, Fetch, Pull, Push ve Tagging*
* **[4.1 - Ekip Kültürü](./docs/4-remote/4.1-collaboration.md)**
    * *Pull Request (PR) Açma ve Review*
    * *Forking Workflow*
    * *`.gitignore` ile Repo Hijyeni*

### Bölüm 5: The Detective (Advanced)
Bir mühendis gibi hata ayıklamak.
* **[5.0 - Suçluyu Bulmak](./docs/5-detective/5.0-debugging.md)**
    * *`blame`: "Bu satırı kim yazdı?"*
    * *`bisect`: 1000 commit arasında hatayı binary search ile bulmak.*

---

### Hazır mısın?
Terminalini aç, kahveni koy. İlk ders için aşağıdaki bağlantıya tıkla. <br>
👉 **[Ders 1.0: Kurulum ve Konfigürasyon](./docs/1-genesis/1.0-kurulum-ve-ayarlar.md)**

---

### 📌 Projenin Anlık Durumu

| Bölüm | Konu | Durum |
| :--- | :--- | :---: |
| **01** | [Genesis](./docs/1-genesis/) | 🟢 Tamamlandı |
| **02** | [Multiverse](./docs/2-multiverse/) | 🟡 Yapım Aşamasında |
| **03** | Time Travel | 🔴 Beklemede |
| **04** | Remote | 🔴 Beklemede |
| **05** | Detective | 🔴 Beklemede |

---

### Kaynakça & Teşekkür

1. **[Linus Torvalds](https://twitter.com/linus__torvalds):**
   > *2005 yılında Git'i yaratarak yazılım dünyasındaki "zaman yolculuğunu" mümkün kıldığı ve biz mühendislere bu muazzam oyun alanını bıraktığı için.*

2. **[Gemini AI](https://gemini.google.com/):**
   > *Projenin monotonluğunu gidermek, eksik tespitinde ve doldurmada yardımcı olmak, Markdown estetiğini güçlendirmek, dil bilgisi hatalarını ayıklamak ve "Interactive Learning" konseptinde mentorluk sağlamak için kullanılmıştır.*

3. **[Git Resmi Dokümantasyonu](https://git-scm.com/doc):**
   > *Her komutun derinliklerine inmek ve doğru bilgiyi sağlamak için başvurulan birincil kaynak.*

4. **[Wikipedia](https://www.wikipedia.org/):**
   > *Kavramsal açıklamalar, tarihsel perspektif ve meraklısına bilgiler sunan birincil kaynak olduğu için.*