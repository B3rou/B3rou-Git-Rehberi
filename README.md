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

> [!IMPORTANT]
> **Komutları Ezberleme, Zihniyeti Kavra!** <br>
> Bu rehberde `rebase`, `cherry-pick`, `orphan` gibi ağır ve tehlikeli komutlar göreceksin. Senden bunları ezberlemeni **kesinlikle beklemiyorum.** İnterneti açıp bir komutun parametresine bakmak 5 saniyelik bir iştir. Asıl mühendislik yeteneği; internette neyi arayacağını bilmek, Git'in klasörleri nasıl yönettiğini zihninde canlandırabilmek ve o mental modeli kurabilmektir. O yüzden, komutları ezberlemek yerine, **Git'in nasıl çalıştığını anlamaya odaklanmanı** öneriyorum.

---

## Nasıl Kullanılır?
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
Tek bir çizgide gitmek zorunda değilsin. Projeni izole alanlara ayırıp güvenle çalışmayı öğren.
* **[2.0 - Branch Anatomisi](./docs/2-multiverse/2.0-branch-mantigi.md)**
    * *Pointer nedir? HEAD nereye bakıyor?*
    * *Branch oluşturma ve geçiş yapma*
* **[2.1 - Birleştirme Sanatı (Merge)](./docs/2-multiverse/2.1-merge-ve-conflict.md)**
    * *Fast-Forward vs 3-Way Merge*
    * *Conflict (Çakışma) Yönetimi ve Çözümü*
* **[2.2 - Gelişmiş Branch Yönetimi](./docs/2-multiverse/2.2-gelismis-branching.md)**
    * *`stash`: Yarım kalan işleri güvenle zulalamak.*
    * *`rebase`: Tarihçeyi ütüleyip düz bir çizgiye çevirmek.*
    * *`cherry-pick`: Başka bir branch'ten nokta atışı commit almak.*
* **[2.3 - Alternatif Gerçeklikler: Orphan Branch ve Temizlik](./docs/2-multiverse/2.3-orphan-dallar.md)**
    * *`orphan`: Geçmişi olmayan, bağımsız branch'ler yaratmak.*
    * *`clean` ve `branch -d`: Çalışma alanının ve reponun bahar temizliği.*
* **[2.4 - Yetenek Ağacım: Bölüm Özeti](./docs/2-multiverse/2.4-bolum-ozeti.md)**
    * *Bu Bölümde Neler Öğrendik?*
    * *Hızlı Bir Bakış: Kavramlar Sözlüğü*

### Bölüm 3: Bulutlara Çıkış (Remote & İşbirliği)
Kodun artık sadece senin bilgisayarında değil. Takım arkadaşlarınla aynı evrende çarpışmadan kod yazmayı öğren.
* **[3.0 - GitHub ile Dans](./docs/3-remote/3.0-remote-temelleri.md)**
    * *SSH Key Kurulumu ve Güvenlik*
    * *Remote, Fetch, Pull, Push: Sunucuyla konuşmak*
* **[3.1 - Ekip Kültürü ve PR](./docs/3-remote/3.1-collaboration.md)**
    * *Pull Request (PR) Açma ve Code Review*
    * *Forking Workflow (Açık kaynak projelere katkı sağlamak)*

### Bölüm 4: Time Travel (Zaman Manipülasyonu)
Hata yaptın. Sorun değil, geçmişi değiştirebiliriz.
* **[4.0 - Geri Alma Sanatı](./docs/4-time-travel/4.0-geri-almak.md)**
    * *`checkout` / `restore` (Eski dosyalara göz atmak ve kurtarmak)*
    * *`revert` (Tarihi bozmadan güvenli geri alma)*
* **[4.1 - Yıkıcı Zaman Yolculuğu](./docs/4-time-travel/4.1-reset-mantigi.md)**
    * *`reset` komutunun 3 atlısı: Soft, Mixed, Hard*
    * *`amend`: Son commiti (sözü) gizlice değiştirmek*
* **[4.2 - The Safety Net (Güvenlik Ağı)](./docs/4-time-travel/4.2-reflog.md)**
    * *`reflog`: Silinen commitleri ve kayıp evrenleri mezardan çıkarmak (Git'in kara kutusu).*

### Bölüm 5: The Detective (Advanced)
Bir mühendis gibi hata ayıklamak.
* **[5.0 - Suçluyu Bulmak](./docs/5-detective/5.0-debugging.md)**
    * *`blame`: "Bu satırı kim yazdı?"*
    * *`bisect`: 1000 commit arasında hatayı binary search ile bulmak.*

### Bonus: Everyday Git (Hap Bilgiler)
* *Sadece en sık kullanılan komutlar ve Cheat Sheet (15 Dakikada Git)*

---

### Hazır mısın?
Terminalini aç, kahveni koy. İlk ders için aşağıdaki bağlantıya tıkla. <br>
👉 **[Ders 1.0: Kurulum ve Konfigürasyon](./docs/1-genesis/1.0-kurulum-ve-ayarlar.md)**

---

### 📌 Projenin Anlık Durumu

| Bölüm | Konu | Durum |
| :--- | :--- | :---: |
| **01** | [Genesis](./docs/1-genesis/) | 🟢 Tamamlandı |
| **02** | [Multiverse](./docs/2-multiverse/) | 🟢 Tamamlandı |
| **03** | [Remote & İşbirliği](./docs/3-remote/) | 🟡 Yapım Aşamasında |
| **04** | [Time Travel](./docs/4-time-travel/) | 🔴 Beklemede |
| **05** | [Detective](./docs/5-detective/) | 🔴 Beklemede |
| **Bonus** | [Everyday Git](./docs/6-everyday-git/) | 🔴 Beklemede |

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