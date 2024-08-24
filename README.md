## İçindekiler
- [Yazılım Mimarı Nedir?](#what-is-a-software-architect)
- [Mimarlık Seviyeleri](#levels-of-architecture)
- [Tipik Faaliyetler](#typical-activities)
- [Önemli Beceriler](#important-skills)
  - [(1) Tasarım](#1-design)
  - [(2) Karar Vermek](#2-decide)
  - [(3) Basitleştir](#3-simplify)
  - [(4) Kod](#4-code)
  - [(5) Belge](#5-document)
  - [(6) İletişim](#6-communicate)
  - [(7) Tahmin Et ve Değerlendir](#7-estimate-and-evaluate)
  - [(8) Denge](#8-balance)
  - [(9) Danışmanlık ve Koçluk](#9-consult-and-coach)
  - [(10) Market](#10-market)
- [Mimarın Teknoloji Yol Haritası](#architects-technology-roadmap)
- [Çözüm Mimarı Türleri](#types-of-solution-architects)
- [Önerilen Kitaplar](#suggested-books)

# Yazılım Mimarı Nedir?
* Bir yazılım mimarı, üst düzey tasarım seçimleri yapan ve yazılım kodlama standartları, araçlar ve platformlar dahil olmak üzere teknik standartları belirleyen bir yazılım uzmanıdır.
_(Kaynak: Vikipedi: Yazılım Mimarı)_
* Yazılım mimarisi, bir sistemin bileşenleri, bunların birbirleriyle ve çevreyle ilişkileri ve sistemin tasarımını ve gelişimini belirleyen ilkelerle temsil edilen temel organizasyonudur.
_(Kaynak: Yazılım Mimarisi El Kitabı)_

# Mimarlık Seviyeleri
Mimarlık çeşitli soyutlama “seviyelerinde” yapılabilir. Seviye gerekli becerilerin önemini etkiler. Pek çok kategorizasyon mümkün olduğundan benim favori segmentasyonum şu 3 seviyeyi içerir:
* **Uygulama Düzeyi**: Mimarinin en düşük düzeyi. Tek bir uygulamaya odaklanın. Çok detaylı, düşük seviyeli tasarım. İletişim genellikle tek bir geliştirme ekibi içinde gerçekleşir.
* **Çözüm Düzeyi**: Mimarinin orta düzeyi. Bir iş ihtiyacını (iş çözümü) karşılayan bir veya daha fazla uygulamaya odaklanın. Bazıları yüksek, ancak çoğunlukla düşük seviyeli tasarım. İletişim birden fazla geliştirme ekibi arasındadır.
* **[Kurumsal Düzey](https://github.com/justinamiller/EnterpriseArchitecture)**: Mimarinin en üst seviyesi. Birden fazla çözüme odaklanın. Çözüm veya uygulama mimarları tarafından detaylandırılması gereken üst düzey, soyut tasarım. İletişim organizasyon çapındadır.

Bazen mimarlar farklı paydaşlar arasında “tutkal” olarak da görülüyor. Üç örnek:

* **Yatay**: İş dünyası ile geliştiriciler veya farklı geliştirme ekipleri arasındaki köprü iletişimi.
* **Dikey**: Geliştiriciler ve yöneticiler arasında köprü iletişimi.
* **Teknoloji**: Farklı teknolojileri veya uygulamaları birbiriyle entegre edin

# Tipik Faaliyetler
Bir mimarın ihtiyaç duyduğu gerekli becerileri anlamak için öncelikle tipik faaliyetleri anlamamız gerekir. Aşağıdaki liste benim açımdan en önemli faaliyetleri içermektedir:

* Geliştirme teknolojisini ve platformunu tanımlayın ve karar verin
* Kodlama standartları, araçlar, inceleme süreçleri, test yaklaşımı vb. gibi geliştirme standartlarını tanımlayın.
* İş gereksinimlerini tanımlama ve anlama desteği
* Sistemleri tasarlayın ve gereksinimlere göre kararlar alın
* Mimari tanımları, tasarımı ve kararları belgeleyin ve iletin
* Mimariyi ve kodu kontrol edin ve gözden geçirin; örneğin, tanımlanmış kalıpların ve kodlama standartlarının düzgün şekilde uygulanıp uygulanmadığını kontrol edin
* Diğer mimarlar ve paydaşlarla işbirliği yapın
* Geliştiricilere koçluk yapın ve onlara danışın
* Daha yüksek seviyeli tasarımı daha düşük seviyeli tasarıma detaylandırın ve iyileştirin

   
_Not: Mimarlık, özellikle çevik yazılım geliştirmede uygulandığında sürekli bir faaliyettir. Bu nedenle bu faaliyetler tekrar tekrar yapılmaktadır._

# Önemli Beceriler
Planlanan faaliyetleri desteklemek için özel beceriler gereklidir. Deneyimlerime, kitaplara ve tartışmalara dayanarak bunu her yazılım mimarının sahip olması gereken şu on beceriye indirgeyebiliriz:
  * Tasarım
  * Karar vermek
  * Basitleştir
  * Kod
  * Belge
  * İletişim
  * Tahmin etmek
  * Denge
  * Danışın
  * Pazar

## (1) Tasarım
İyi bir tasarımı ne yapar? Bu muhtemelen en önemli ve zorlayıcı sorudur. Teori ve pratik arasında bir ayrım yapacağım. Deneyimlerime göre her ikisinin bir karışımına sahip olmak çok değerlidir. Teoriyle başlayalım:

* **Temel tasarım modellerini bilin**: Desenler, bir mimarın sürdürülebilir sistemler geliştirmek için ihtiyaç duyduğu en önemli araçlardan biridir. Desenler sayesinde, yaygın sorunları kanıtlanmış çözümlerle çözmek için tasarımları yeniden kullanabilirsiniz. John Vlissides, Ralph Johnson, Richard Helm, Erich Gamma tarafından yazılan “Tasarım Desenleri: Yeniden Kullanılabilir Nesneye Dayalı Yazılımın Öğeleri” kitabı, yazılım geliştirmeyle uğraşan herkesin mutlaka okuması gereken bir kitap. Desenler 20 yıldan fazla bir süre önce yayınlanmış olmasına rağmen hala modern yazılım mimarisinin temelini oluşturmaktadır. Örneğin, birçok alanda uygulanan veya daha yeni modelin temelini oluşturan Model-Görünüm-Denetleyici (MVC) modeli bu kitapta anlatılmıştır; Model-Görünüm-GörünümModel (MVVM).
* **Desenleri ve anti-kalıpları daha derinlemesine inceleyin**: Tüm temel Dörtlü Çete kalıplarını zaten biliyorsanız, daha fazla yazılım tasarım modeliyle bilginizi genişletin veya ilgi alanınızda daha derinlere inin. Uygulama entegrasyonuyla ilgili en sevdiğim kitaplardan biri Gregor Hohpe'nin yazdığı “Kurumsal Entegrasyon Kalıpları”dır. Bu kitap, ister bazı eski sistemlerden eski usul dosya alışverişi ister modern bir mikro hizmet mimarisi olsun, iki uygulamanın veri alışverişi yapması gerektiğinde çeşitli alanlarda uygulanabilir.
* **Kalite ölçütlerini bilin**: Mimariyi tanımlamak işin sonu değildir. Kılavuzların ve kodlama standartlarının tanımlanmasının, uygulanmasının ve kontrol edilmesinin nedenleri vardır. Bunu kalite ve işlevsel olmayan gereksinimler nedeniyle yapıyorsunuz. Bakımı yapılabilir, güvenilir, uyarlanabilir, emniyetli, test edilebilir, ölçeklenebilir, kullanılabilir vb. bir sisteme sahip olmak istiyorsunuz. Ve tüm bu kalite özelliklerine ulaşmanın tek parçası iyi bir mimari çalışması uygulamaktır. Vikipedi'de kalite ölçümleri hakkında daha fazla bilgi edinmeye başlayabilirsiniz.
Teori önemlidir. Fildişi Kule Mimarı olmak istemiyorsanız pratik yapmak da aynı derecede, hatta daha da önemlidir.
* **Farklı teknoloji yığınlarını deneyin ve anlayın**: Daha iyi bir mimar olmak istiyorsanız bunun en önemli aktivite olduğunu düşünüyorum. (Yeni) teknoloji yığınlarını deneyin ve bunların iniş çıkışlarını öğrenin. Farklı veya yeni teknoloji, farklı tasarım yönleri ve desenleriyle birlikte gelir. Büyük olasılıkla sadece soyut slaytları çevirerek değil, kendi başınıza deneyerek ve acıyı veya rahatlamayı hissederek hiçbir şey öğrenmezsiniz. Bir mimar sadece geniş değil aynı zamanda bazı alanlarda derin bilgiye de sahip olmalıdır. Tüm teknoloji yığınlarında uzmanlaşmak değil, bölgenizdeki en önemlileri sağlam bir şekilde anlamak önemlidir. Ayrıca, bölgenizde olmayan teknolojileri de deneyin; örneğin, SAP R/3 ile ilgiliyseniz JavaScript'i de denemelisiniz (veya tam tersi). Yine de her iki taraf da SAP S/4 Hana'daki son gelişmelere şaşıracak. Örneğin, kendiniz deneyebilir ve openSAP'ta ücretsiz bir kursa katılabilirsiniz. Meraklı olun ve yeni şeyler deneyin. Ayrıca birkaç yıl önce hoşlanmadığınız şeyleri de deneyin.
* **Uygulanan kalıpları analiz edin ve anlayın**: Angular gibi mevcut çerçevelere bir göz atın. Pratikte birçok modeli inceleyebilirsiniz; örneğin Gözlemlenebilirler. Çerçevede nasıl uygulandığını, neden yapıldığını anlamaya çalışın. Ve eğer gerçekten kararlıysanız, koda daha derinlemesine bakın ve nasıl uygulandığını anlayın.
* **Meraklı olun ve Kullanıcı Gruplarına katılın**. [Meetup](https://www.meetup.com/)

## (2) Karar ver
Bir mimarın kararlar alabilmesi ve projeleri veya tüm organizasyonu doğru yöne yönlendirebilmesi gerekir.

* **Neyin önemli olduğunu bilin**: Önemsiz kararlar veya faaliyetlerle zaman kaybetmeyin. Neyin önemli olduğunu öğrenin. Bildiğim kadarıyla bu bilgilerin yer aldığı bir kitap yok. Kişisel favorilerim, bir şeyin önemli olup olmadığını değerlendirirken genellikle dikkate aldığım şu 2 özelliktir:
  1. Kavramsal Bütünlük: Eğer bunu bir şekilde yapmaya karar verirseniz, bazen farklı şekilde yapmak daha iyi olsa bile ona bağlı kalın. Bu genellikle daha basit bir genel konsepte yol açar, anlaşılırlığı kolaylaştırır ve bakımı kolaylaştırır.
 2. Tekdüzelik: Örneğin adlandırma kurallarını tanımlayıp uygularsanız, bu büyük veya küçük harfle ilgili değil, bunun her yere aynı şekilde uygulanmasıyla ilgilidir.
* **Önceliklendir**: Bazı kararlar son derece kritiktir. Yeterince erken önlem alınmazlarsa, daha sonra kaldırılması pek mümkün olmayan ve bakım için bir kabusa dönüşen geçici çözümler oluşur veya daha kötüsü, geliştiriciler bir karar alınana kadar çalışmayı bırakırlar. Böyle durumlarda bazen hiçbir karar vermemek yerine “kötü” bir karara varmak daha da iyidir. Ancak iş bu duruma gelmeden önce yaklaşan kararlara öncelik vermeyi düşünün. Bunu yapmanın farklı yolları var. Çevik yazılım geliştirmede yaygın olarak kullanılan Ağırlıklı En Kısa Önce İş (WSJF) modeline bir göz atmanızı öneririm. Özellikle zaman kritikliği ve risk azaltma önlemleri, mimari kararların önceliğini tahmin etmek için kritik öneme sahiptir.
* **Yetkinliğinizi bilin**: Yetkinliğiniz olmayan şeylere karar vermeyin. Bu çok önemlidir çünkü dikkate alınmazsa mimar olarak konumunuzu önemli ölçüde bozabilir. Bunu önlemek için meslektaşlarınızla hangi sorumluluklara sahip olduğunuzu ve neyin rolünüzün bir parçası olduğunu netleştirin. Birden fazla mimar varsa, o anda görevlendirildiğiniz mimarinin düzeyine saygı duymalısınız. Daha düşük düzeydeki bir mimar olarak, kararlar yerine daha yüksek düzeydeki mimariye yönelik önerilerde bulunsanız iyi olur. Ayrıca, kritik kararları her zaman bir akranınızla kontrol etmenizi öneririm.
* **Birden fazla seçeneği değerlendirin**: Karar verme söz konusu olduğunda her zaman birden fazla seçeneği ortaya koyun. Dahil olduğum vakaların çoğunda birden fazla olası (iyi) seçenek vardı. Tek seçenekle gitmek iki açıdan kötüdür: Birincisi, işinizi iyi yapmamışsınız gibi görünür, ikincisi ise doğru karar vermenizi engeller. Ölçüler tanımlanarak seçenekler içgüdüsel hisler yerine gerçeklere dayalı olarak karşılaştırılabilir; lisans maliyetleri veya vade. Bu genellikle daha iyi ve daha sürdürülebilir kararlara yol açar. Ayrıca kararın farklı paydaşlara satılmasını kolaylaştırır. Ayrıca seçenekleri doğru değerlendirmediyseniz konu tartışma olduğunda tartışmaları kaçırabilirsiniz.

## (3) Basitleştir
Occam'ın Usturası'nın basitliği tercih etmeyi ifade eden problem çözme ilkesini aklınızda bulundurun. Prensibi şu şekilde yorumluyorum: Eğer problemle ilgili çözemediğiniz çok fazla varsayım varsa, çözümünüz muhtemelen yanlış olacak veya gereksiz karmaşık bir çözüme yol açacaktır. İyi bir çözüme ulaşmak için varsayımların azaltılması (basitleştirilmesi) gerekir.

* **Çözümünü sallayın**: Çözümleri basitleştirmek için genellikle çözümü "sallamak" ve onlara farklı konumlardan bakmak yardımcı olur. Çözümü yukarıdan aşağıya ve yine aşağıdan yukarıya düşünerek şekillendirmeye çalışın. Bir veri akışınız veya süreciniz varsa önce soldan sağa, sonra tekrar sağdan sola düşünün. Şu tür sorular sorun: "Mükemmel bir dünyada çözümünüze ne olur?" Veya: “X şirketi/kişisi ne yapardı?” (Burada X muhtemelen rakibiniz değil, GAFA (Google, Apple, Facebook ve Amazon) şirketlerinden biridir.) Her iki soru da sizi Occam's Razor'un önerdiği gibi varsayımları azaltmaya zorluyor.
* **Geri adım atın**: Yoğun ve uzun tartışmaların ardından genellikle son derece karmaşık karalamalar ortaya çıkar. Bunları asla nihai sonuçlar olarak görmemelisiniz. Bir adım geri atın: Büyük resme tekrar bakın (soyut düzey). Hala mantıklı mı? Daha sonra soyut düzeyde tekrar gözden geçirin ve yeniden düzenleyin. Bazen bir tartışmayı durdurup ertesi gün devam etmek faydalı olabilir. En azından beynimin işleyebilmesi ve daha iyi, daha şık ve daha basit çözümler üretebilmesi için biraz zamana ihtiyacı var.
* **Böl ve Fethet**: Sorunu daha küçük parçalara bölerek basitleştirin. Daha sonra bunları bağımsız olarak çözün. Daha sonra küçük parçaların birbiriyle eşleşip eşleşmediğini doğrulayın. Bunun için genel resme bakmak için bir adım geri atın.
* **Yeniden düzenleme kötü değildir**: Daha iyi bir fikir bulunamazsa, daha karmaşık bir çözümle başlamak tamamen uygundur. Çözüm sorun yaratıyorsa daha sonra çözümü yeniden düşünebilir ve öğrendiklerinizi uygulayabilirsiniz. Yeniden düzenleme kötü değildir. Ancak yeniden düzenlemeye başlamadan önce, (1) sistemin düzgün işlevselliğini sağlayabilecek yeterli sayıda otomatik teste sahip olduğunuzu ve (2) paydaşlarınızın desteğini almayı unutmayın. Yeniden düzenleme hakkında daha fazla bilgi edinmek için “Yeniden Düzenleme”yi okumanızı öneririm. Mevcut Kodun Tasarımını İyileştirme”, Martin Fowler.

## (4) Kod
Mimarinin en soyut seviyesi olan Kurumsal Mimar olarak bile geliştiricilerin günlük olarak ne yaptığını bilmelisiniz. Ve bunun nasıl yapıldığını anlamadıysanız iki büyük sorunla karşılaşabilirsiniz:
  1. Geliştiriciler sözlerinizi kabul etmeyecektir.
  2. Geliştiricilerin zorluklarını ve ihtiyaçlarını anlamıyorsunuz.

* **Bir yan projeniz olsun**: Bunun amacı, bugün ve gelecekte geliştirmenin nasıl yapıldığını öğrenmek için yeni teknolojileri ve araçları denemektir. Deneyim, gözlemlerin, duyguların ve hipotezlerin birleşimidir (Kurt Schneider tarafından “Yazılım Mühendisliğinde Deneyim ve Bilgi Yönetimi”). Bir öğreticiyi veya bazı artıları ve eksileri okumak iyidir. Ama bu sadece “kitap bilgisidir”. Ancak bazı şeyleri kendi başınıza denerseniz duyguları deneyimleyebilir ve bir şeyin neden iyi ya da kötü olduğuna dair hipotezler geliştirebilirsiniz. Ve bir teknolojiyle ne kadar uzun süre çalışırsanız hipoteziniz o kadar iyi olur. Bu, günlük işlerinizde daha iyi kararlar almanıza yardımcı olacaktır. Programlamaya başladığımda hiçbir kod tamamlamam yoktu ve geliştirmeyi hızlandırmak için yalnızca bazı yardımcı program kitaplıklarım vardı. Açıkçası, bu arka planla bugün yanlış kararlar verirdim. Bugün tonlarca programlama dilimiz, çerçevemiz, aracımız, sürecimiz ve uygulamamız var. Ancak belli bir deneyiminiz varsa ve ana trendler hakkında kabaca bir genel bakışa sahipseniz, konuşmanın bir parçası olabilir ve gelişimi doğru yöne yönlendirebilirsiniz.
* **Denemek için doğru şeyleri bulun**: Her şeyi deneyemezsiniz. This is simply impossible. You need a more structured approach. One source I recently discovered is the [Technology Radar](https://www.thoughtworks.com/radar) ThinkWorks'ten. Teknolojileri, araçları, platformları, dilleri ve çerçeveleri dört kategoriye ayırıyorlar:
  * Benimseyin: “kurumsal kullanıma hazır olma konusunda güçlü bir duygu”.
  *Deneme: “İşletme riski kaldırabilecek tek bir projede denemelidir”.
  * Değerlendirin: “kurumunuzu nasıl etkilediğini keşfedin”
  * Basılı tutun: “dikkatli işlem yapın”.

Bu kategorizasyonla, yeni şeyler hakkında genel bir bakış elde etmek ve bir sonraki trendin hangi trendin keşfedileceğini daha iyi değerlendirmeye hazır olup olmadıklarını öğrenmek daha kolaydır.


## (5) Belge
Mimari dokümantasyon bazen daha fazla, bazen daha az önemlidir. Önemli belgeler örneğin mimari kararlar veya kod yönergeleridir. İlk dokümantasyon genellikle kodlama başlamadan önce gereklidir ve sürekli olarak iyileştirilmesi gerekir. Kod aynı zamanda belge olabileceğinden diğer belgeler de otomatik olarak oluşturulabilir; UML sınıf diyagramları.

* **Temiz Kod**: Kod, doğru kullanıldığında en iyi belgedir. İyi bir mimar iyi ve kötü kodu ayırt edebilmelidir. İyi ve kötü kod hakkında daha fazla bilgi edinmek için gerçekten harika bir kaynak, Robert C. Martin'in "Temiz Kod" kitabıdır.
* **Mümkün olduğunda belgeler oluşturun**: Sistemler hızla değişiyor ve belgeleri güncellemek zor. İster API'ler ister CMDB (Yapılandırma yönetimi veritabanı) biçimindeki sistem ortamları hakkında olsun: Temel bilgiler genellikle ilgili belgeleri elle güncel tutmak için çok hızlı değişir. Örnek: API'ler için, model odaklıysanız tanım dosyasına dayalı olarak veya doğrudan kaynak kodundan belgeleri otomatik olarak oluşturabilirsiniz. Bunun için pek çok araç mevcut, bence Swagger ve RAML daha fazlasını öğrenmek için iyi bir başlangıç ​​noktası.
* **Gerektiği kadar çok, mümkün olduğu kadar az**: Karar belgeleri gibi belgelemeniz gereken her ne varsa, aynı anda yalnızca tek bir şeye odaklanmaya çalışın ve yalnızca bu tek şey için gerekli bilgileri ekleyin. Kapsamlı dokümantasyonun okunması ve anlaşılması zordur. Ek bilgiler ekte saklanmalıdır. Özellikle karar belgeleri için tonlarca argüman ortaya koymak yerine ikna edici bir hikaye anlatmak daha önemlidir. Dahası, bu size ve onu okumak zorunda olan iş arkadaşlarınıza çok zaman kazandırır. Geçmişte yaptığınız bazı belgelere (kaynak kodu, modeller, karar belgeleri vb.) bir göz atın ve kendinize şu soruları sorun: "Bunu anlamak için gerekli tüm bilgiler dahil mi?", "Hangi bilgiler gerçekten gerekli ve hangileri? hangisi ihmal edilebilir?” ve “Belgelerde kırmızı çizgi var mı?”.
* **Mimari çerçeveler hakkında daha fazla bilgi edinin**: Bu nokta diğer tüm "teknik" noktalara da uygulanabilir. TOGAF veya Zachmann gibi çerçeveler, katma değerleri yalnızca dokümantasyonla sınırlı olmasa da, dokümantasyon tarafında ağır gelen “araçlar” sağladığı için bunu buraya koyuyorum. Böyle bir çerçevede sertifika almak size mimarlığı daha sistematik bir şekilde ele almayı öğretir.

## (6) İletişim kurun
Gözlemlerime göre bu, en hafife alınan becerilerden biridir. Tasarım konusunda mükemmelseniz ancak fikirlerinizi iletemezseniz, düşüncelerinizin etkisi muhtemelen daha az olacaktır, hatta başarılı olamayacaktır.

* **Fikirlerinizi nasıl ileteceğinizi öğrenin**: Bir tahta veya yazı tahtası üzerinde işbirliği yaparken, sizin ve meslektaşlarınızın düşüncelerini yapılandırmak için onu nasıl doğru şekilde kullanacağınızı bilmek çok önemlidir. “UZMO — Kaleminizle Düşünmek” kitabını bu alandaki becerilerimi geliştirmek için iyi bir kaynak olarak buldum. Bir mimar olarak genellikle yalnızca bir toplantıya katılmakla kalmazsınız, genellikle toplantıyı yönlendirmeniz ve yönetmeniz gerekir.
* **Büyük gruplara konuşmalar yapın**: Fikirlerinizi küçük veya büyük bir gruba sunmak sizin için mümkün olmalıdır. Eğer bundan rahatsızlık duyuyorsanız en yakın arkadaşınıza sunum yapmaya başlayın. Grubu yavaşça büyütün. Bu ancak yaparak ve kişisel konfor alanınızı terk ederek öğrenebileceğiniz bir şeydir. Kendinize karşı sabırlı olun, bu süreç biraz zaman alabilir.
* **Doğru iletişim düzeyini bulun**: Farklı paydaşların farklı ilgi alanları ve görüşleri vardır. Bunların kendi seviyelerinde ayrı ayrı ele alınması gerekir. İletişim kurmadan önce bir adım geri çekilin ve paylaşmak istediğiniz bilgilerin soyutluk, içerik, hedefler, motivasyonlar vb. açısından doğru düzeyde olup olmadığını kontrol edin. Örnek: Bir geliştirici genellikle çözümün çok küçük ayrıntılarıyla ilgilenirken, bir yönetici genellikle çözümün çok küçük ayrıntılarıyla ilgilenir. hangi seçeneğin en fazla tasarruf sağladığını bilmeyi tercih eder.
* **Sık sık iletişim kurun**: Kimsenin haberi yoksa parlak bir mimarinin hiçbir değeri yoktur. Hedef mimariyi ve onun arkasındaki düşünceleri düzenli olarak ve her organizasyonel seviyeye dağıtın. Geliştiricilere, mimarlara ve yöneticilere istenen veya tanımlanmış yolu göstermek için toplantılar planlayın.
* **Şeffaf olun**: Düzenli iletişim, şeffaflığın eksikliğini yalnızca kısmen giderir. Kararların arkasındaki nedeni şeffaf hale getirmelisiniz. Özellikle insanlar karar alma sürecine dahil değilse, kararı ve arkasındaki mantığı anlamak ve takip etmek zordur.
* **Sunum yapmaya her zaman hazırlıklı olun**: Her zaman soruları olan birileri vardır ve siz de hemen doğru cevapları vermek istersiniz. Her zaman en önemli slaytları gösterebileceğiniz ve açıklayabileceğiniz birleştirilmiş bir sette bulundurmaya çalışın. Size çok zaman kazandırır ve kendinize güvenlik sağlar.

## (7) Tahmin Et ve Değerlendir
* **Temel proje yönetimi ilkelerini öğrenin**: Mimar veya lider geliştirici olarak fikirlerinizi hayata geçirmek için sıklıkla sizden tahminler istenir: Ne kadar süre, ne kadar, kaç kişi, hangi beceriler, vb.? Elbette yeni araçlar veya çerçeveler sunmayı planlıyorsanız bu tür "yönetim" sorularına bir yanıtınızın olması gerekir. Başlangıçta günler, aylar veya yıllar gibi kaba bir tahmin verebilmelisiniz. Ve bunun yalnızca uygulamayla ilgili olmadığını, gereksinim mühendisliği, test etme ve hataları düzeltme gibi dikkate alınması gereken daha fazla faaliyet olduğunu unutmayın. Bu nedenle kullanılan yazılım geliştirme sürecindeki etkinlikleri bilmelisiniz. Daha iyi tahminler elde etmek için uygulayabileceğiniz şeylerden biri geçmiş verileri kullanmak ve tahmininizi bundan çıkarmaktır. Geçmiş verileriniz yoksa Barry W. Boehm'in COCOMO'su gibi yaklaşımları da deneyebilirsiniz. Çevik bir projede görevlendirildiyseniz, nasıl tahminde bulunacağınızı ve doğru şekilde plan yapacağınızı öğrenin: Mike Cohn'un "Çevik Tahmin Etme ve Planlama" kitabı bu alanda sağlam bir genel bakış sağlar.
* **“Bilinmeyen” mimariyi değerlendirin**: Mimar olarak aynı zamanda mimarilerin mevcut veya gelecekteki bağlam(lar)a uygunluğunu da değerlendirebilmelisiniz. Bu kolay bir iş değildir ancak her mimari için ortak olan bir dizi soruyu elinizin altında bulundurarak buna hazırlanabilirsiniz. Ve bu sadece mimariyle ilgili değil, aynı zamanda sistemin nasıl yönetildiğiyle de ilgili, çünkü bu aynı zamanda size kalite hakkında da fikir veriyor. Her zaman bazı soruların hazır ve kullanıma hazır olmasını öneririm. Genel sorular için bazı fikirler:
  1. Tasarım uygulamaları: Mimari hangi kalıpları takip ediyor? Sonuç olarak ve doğru şekilde kullanılıyorlar mı? Tasarım kırmızı çizgiyi mi takip ediyor yoksa kontrolsüz bir büyüme mi var? Endişelerin net bir yapısı ve ayrımı var mı?
  2. Geliştirme uygulamaları: Kural yönergeleri mevcut ve takip ediliyor mu? Kod nasıl versiyonlanır? Dağıtım uygulamaları?
  3. Kalite güvencesi: Test otomasyonu kapsamı? Statik kod analizi mevcut ve iyi sonuçlar var mı? Akran değerlendirmeleri mevcut mu?
  4. Güvenlik: Hangi güvenlik konseptleri mevcut? Yerleşik güvenlik? Sızma testleri veya otomatik güvenlik analizi araçları mevcut ve düzenli olarak kullanılıyor mu?

## (8) Bakiye
* **Kalitenin bir bedeli vardır**: Daha önce kalite ve işlevsel olmayan gereksinimlerden bahsetmiştim. Eğer mimariyi abartırsanız, bu maliyetleri artıracak ve muhtemelen geliştirme hızını düşürecektir. Mimari ve işlevsel gereksinimleri dengelemeniz gerekir. Aşırı mühendislikten kaçınılmalıdır.
* **Çelişkili hedefleri çözün**: Çelişkili hedeflere klasik bir örnek, kısa ve uzun vadeli hedeflerdir. Projeler genellikle en basit çözümü oluşturma eğilimindeyken mimarın aklında uzun vadeli bir vizyon vardır. Çoğu zaman basit çözüm, uzun vadeli çözüme uymaz ve daha sonra çöpe atılma riskiyle karşı karşıyadır (batık maliyetler). Uygulamanın yanlış yönde olmasını önlemek için iki şeyin dikkate alınması gerekir:
  1. Geliştiricilerin ve iş dünyasının, çözümlerini uyarlamak için uzun vadeli vizyonu ve bunların faydalarını anlamaları gerekir.
  2. Mali etkiyi anlamak için bütçeden sorumlu yöneticilerin sürece dahil olması gerekir. Uzun vadeli vizyonun %100'ünün doğrudan yerinde olması gerekli değildir, ancak geliştirilen parçanın buna uyması gerekir.
* **Çatışma yönetimi**: Mimarlar genellikle farklı geçmişlere sahip birden fazla grup arasındaki birleştiricidir. Bu, farklı iletişim düzeylerinde çatışmalara yol açabilir. Uzun vadeli, stratejik hedefleri de yansıtan dengeli bir çözüm bulmak için, çatışmanın üstesinden gelmeye yardımcı olmak genellikle mimarların görevidir. İletişim teorisine dair çıkış noktam Schulze von Thun'un “Dört Kulak Modeli”ydi. Bu modele dayanarak pek çok şey gösterilebilir ve çıkarılabilir. Ancak bu teorinin iletişim seminerleri sırasında deneyimlenmesi gereken bazı pratiklere ihtiyacı var.

## (9) Danışmanlık ve Koçluk
Proaktif olmak muhtemelen danışmanlık ve koçluk söz konusu olduğunda yapabileceğiniz en iyisidir. diye sorulursa çoğu zaman çok geç kalınmıştır. Ve mimari alanda temizlik yapmak, kaçınmak isteyeceğiniz bir şeydir. Gelecek haftaları, ayları hatta yılları bir şekilde öngörmeniz, kendinizi ve organizasyonunuzu sonraki adımlara hazırlamanız gerekiyor.

* **Bir vizyona sahip olun**: Bir projede görevlendirildiyseniz, ister geleneksel şelale benzeri yaklaşım ister çevik olsun, ulaşmak istediğiniz orta ve uzun vadeli hedeflerinize dair her zaman bir vizyona sahip olmanız gerekir. Bu detaylı bir kavram değil, daha ziyade herkesin işleyebileceği bir yol haritasıdır. Her şeyi bir anda başaramayacağınız için (bu bir yolculuk) olgunluk modellerini kullanmayı tercih ediyorum. Kolayca tüketilebilecek net bir yapı kazandırırlar ve her an ilerlemenin mevcut durumunu verirler. Farklı yönler için farklı modeller kullanıyorum; geliştirme uygulamaları veya sürekli teslimat. Olgunluk modelindeki her seviyenin, ulaşıp ulaşmadığınızı ölçmeyi kolaylaştırmak için SMART kriterlerini takip eden açık gereksinimleri vardır. Bulduğum güzel bir örnek, sürekli teslimatla ilgili.
* **Bir uygulama topluluğu (CoP) oluşturun**: Ortak bir ilgi grubu arasında deneyim ve bilgi alışverişi, fikirlerin dağıtımına ve yaklaşımların standartlaştırılmasına yardımcı olur. Örneğin, tüm JavaScript geliştiricilerini ve mimarlarını yaklaşık üç ayda bir bir odada toplayabilir ve geçmişteki ve mevcut zorlukları, bunların nasıl ele alındığını veya yeni metodolojileri ve yaklaşımları tartışabilirsiniz. Mimarlar vizyonlarını paylaşabilir, tartışabilir ve uyumlu hale getirebilir; geliştiriciler deneyimlerini paylaşabilir ve meslektaşlarından öğrenebilir. Böyle bir tur, daha güçlü bir ağ oluşturulmasına ve fikirlerin yayılmasına yardımcı olduğundan hem kuruluş için hem de bireyin kendisi için son derece faydalı olabilir. Ayrıca CoP kavramını çevik bir ortamda açıklayan SAFe Çerçevesindeki Uygulama Toplulukları makalesine de göz atın.
* **Açık kapı oturumları düzenleyin**: Yanlış anlamaların veya belirsizliğin kaynaklarından biri de iletişim eksikliğidir. Sabit bir zaman aralığını engelleyin, ör. Akranlarınızla güncel konuları paylaşmak için her hafta 30 dakika. Bu oturumun herhangi bir gündemi yoktur, her şey tartışılabilir. Küçük sorunları yerinde çözmeye çalışın. Daha karmaşık konularda takipler planlayın.

## (10) Piyasa
Fikirleriniz harika ve bunları iyi bir şekilde ilettiğiniz halde hala kimse takip etmek istemiyor mu? O zaman muhtemelen pazarlama becerileriniz yok.

* **Motive edin ve ikna edin**: Şirketler sizi bir ürünü satın almaya nasıl ikna eder? Değerini ve faydalarını gösterirler. Ancak sadece 5 madde işaretiyle değil. Güzelce sarıyorlar ve sindirimi mümkün olduğunca kolaylaştırıyorlar.
  1. Prototipler: Fikrinizin bir prototipini gösterin. Prototip oluşturmak için birçok araç var. SAP'yi seven kuruluşlar bağlamında, güzel görünümlü ve tıklanabilir UI5 uygulamalarını hızlı ve kolay bir şekilde oluşturabileceğiniz build.me'ye göz atın.
  2. Bir video gösterin: “Sıkıcı slaytlar” yerine fikrinizi veya en azından yönünüzü gösteren bir video da gösterebilirsiniz.
Ancak lütfen pazarlamayı abartmayın: Uzun vadede içerik kraldır. Eğer sözleriniz gerçekleşmezse bu durum uzun vadede itibarınıza zarar verecektir.
* **Fikirleriniz için savaşın ve ısrarcı olun**: İnsanlar bazen fikirlerinizi beğenmezler veya onları takip edemeyecek kadar tembel olurlar. Eğer fikirlerinize gerçekten inanıyorsanız sürekli onların peşinden gitmeli ve “mücadele etmelisiniz”. Bu bazen gereklidir. Uzun vadeli hedefleri olan mimari kararlar genellikle en kolay kararlar değildir: Geliştirilmesi daha karmaşık olduğundan geliştiriciler bunları sevmez. Kısa vadede daha pahalı oldukları için yöneticiler onları sevmiyor. Kalıcı olmak ve müzakere etmek sizin görevinizdir.
* **Müttefik bulun**: Fikirlerinizi kendi başınıza oluşturmak veya uygulamak zor, hatta imkansız olabilir. Başkalarını destekleyebilecek ve ikna etmeye yardımcı olabilecek müttefikler bulmaya çalışın. Ağınızı kullanın. Henüz bir tane yoksa, şimdi oluşturmaya başlayın. Fikirleriniz hakkında (açık fikirli) akranlarınızla konuşarak başlayabilirsiniz. Eğer hoşlarına giderse veya en azından bir kısmı, başkaları tarafından sorulduğunda fikrinizi destekleyeceklerdir (“X'in fikri ilginçti.”). Eğer beğenmedilerse nedenini sorun: Belki bir şeyleri kaçırmışsınızdır? Veya hikayeniz yeterince ikna edici değil mi? Bir sonraki adım karar gücüne sahip müttefikler bulmaktır. Açık fikirli bir tartışma isteyin. Tartışmadan korkuyorsanız bazen konfor alanınızdan çıkmanız gerektiğini unutmayın.
* **Tekrar Edin, İnanın**: "[...] araştırmalar, bir görüşe tekrar tekrar maruz kalmanın, o görüşün kaynağı yalnızca tek bir kişi olsa bile, insanları bu görüşün daha yaygın olduğuna inandırdığını gösteriyor." (Kaynak: The Financial Brand) Yeterince sıklıkta birkaç mesaj yayınlarsanız, insanları daha kolay ikna etmeye yardımcı olabilirsiniz. Ancak şunu unutmayın: Benim açımdan böyle bir strateji, berbat bir pazarlama numarası olarak geri tepebileceği için akıllıca kullanılmalıdır.


# Architect's Technology Roadmap
 * [**Software Architect Roadmap. Complete guide to become a Software Architect**](https://roadmap.sh/software-architect) by Kamran Ahmed.

![Architect roadmap](./src/archRoadmap.jpg)

# Types of Solution Architects
![TypesSolution](./src/typesofsolutionarchitects.jpg)


# Önerilen Kitaplar
 * **Yeniden düzenleme. Mevcut Kodun Tasarımını İyileştirme**, Martin Fowler
 * **Kurumsal Entegrasyon Modelleri** Gregor Hohpe tarafından yazılmıştır
 * **Tasarım Desenleri: Yeniden Kullanılabilir Nesneye Dayalı Yazılımın Öğeleri** Yazan: John Vlissides, Ralph Johnson, Richard Helm, Erich Gamma
 * **Yazılım Mühendisliğinde Deneyim ve Bilgi Yönetimi** - Kurt Schneider
 * **Temiz Kod**, Robert C. Martin
 * **UZMO — Kaleminizle Düşünmek**
 * **Çevik Tahmin ve Planlama** - Mike Cohn
 * **Veri Yoğun Uygulamalar Tasarlamak** - Martin Kleppmann (Veri, analitik ve veri bilimi ile ilgili herhangi bir şey yapıyorsanız bu kitabı mutlaka okumalısınız).
