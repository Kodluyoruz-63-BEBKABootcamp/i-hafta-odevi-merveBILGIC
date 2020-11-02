#  Docker'a ait kavramlar 
Docker uygulamaları geliştirme, yayına alma ve çalıştırma gibi süreçleri container üzerinden yürütmeyi sağlayan bir platrformdur. Temel felsefesi işletim sisteminden soyutlanarak 
her biri ayrı containerler üzerinde çalışabilen birbirinden etkilenmeyecek ayrı uygulama yayın alanları oluşturmasını sağlamaktır.
İşletim sistemlerinden bağımsız olarak Docker mimarisinin temelinde Daemon process’i bulunur.
Linux’da hem Daemon hem de Docker CLI (Command Line Interface) direkt Linux üzerinde koşmaktadır.
Windows ve Mac OS X’te ise Docker CLI Windows ve Mac OS X işletim sistemlerinde, Daemon ise bir sanallaştırma teknolojisi (Hypervisor) ile Linux üzerinde koşar. 
Bunun sebebi ise Daemon’un Linux çekirdeğine ihtiyaç duymasıdır.
##### Imaje: Docker üzerinde konteyner ayağı kaldırmak için bir imaja ihtiyaç duyulur. 
Imajlar içinde uygulamanızın çalışması için kütüphane, ortam değişkenleri ve konfigürasyon dosyalarını barındıran çalıştırılabilir paketlerdir.
##### Container: Temel olarak konteyner, imajın çalıştırılabilir örneğidir. 
Docker Rest API veya CLI aracılığıyla konteynerler oluşturup, başlatıp, durdurabilir veya başka bir yere taşıyabiliriz.
###### Konteynerizasyon’un Avantajları ?
Esneklik: En karmaşık uygulamalar bile konteynır üzerinden yayınlanabilir.
Hafif Yük: Konteynırlar Linux Kernel çekirdeğini kullanır ve paylaşırlar. Sanal Makineler de ki gibi her birinin ayrı bir işletim sistemi olmaz.
Taşınabilirlik: Local’inde çalıştırıp, bulut sunucu üzerinde yayınlayıp ve her yerde çalıştırabilirsin.
Ölçeklenebilirlik: Çalışan servislerimizinin üzerinde ki trafiğe göre yeni konteynerler ortaya çıkarılabilir.
##### Docker Registry
Docker, imaj dosyalarını Docker Registry’de depolar.  

yararlanılan [kaynak](https://medium.com/devopsturkiye/temel-d%C3%BCzeyde-docker-mant%C4%B1%C4%9F%C4%B1-ve-kavramlar%C4%B1-bde5418858d4) için tıklayınız.

# .Net Core versiyonları ve bu versiyonlar arasındaki farklılıklar
NET Core, Microsoft ve .NET tarafından desteklenen açık kaynaklı bir gelişim platformudur.
Cross Platform özelliği ile çapraz platformlarda çalışabilir. Yani Windows, macOS, Linux gibi ortamlarda çalışabilmektedir. 
Eğer yapmak istediğiniz uygulamanın birden fazla platformda çalışmasını istiyor iseniz .NET Core ile uygulama geliştirebilirsiniz.
.NET Core .NET Framework, Xamarin, Mono ile .NET standart kütüphanesi nedeni ile uyumlu olarak çalışır.
.NET Core MIT ve Apache 2 lisansları altında yer alan açık kaynaklı bir platformdur.
.NET Core modüler bir yapıya sahiptir ve sadece bir uygulamada istediğiniz, ihtiyacınız olan paketleri kullanabilirsiniz. Gereksiz paketler ile uğraşmazsınız.
Gelişim arayüzü Command line style dediğimiz (CLI) gelişim arayüzüdür. Yani komut satırı stilidir.
Desteklenen tüm platformlarda kullanılabilen komut satırı araçlarını sağlamaktadır.
Böylelikle yazılımı geliştiren kullanıcılar minimum ek yüklemeler ile uygulamalarını test edebilirler ve geliştirebilirler.
2002'de Microsoft , Windows uygulamaları oluşturmak için bir geliştirme platformu olan .NET Framework'ü piyasaya sürdü . 
Bugün .NET Framework, 4.8 sürümündedir ve hala Microsoft tarafından desteklenmektedir .
2014 yılında Microsoft, .NET Framework için çapraz platform, açık kaynaklı bir halef yazmaya başladı. Bu yeni .NET uygulaması, 3.1 sürümüne ulaşana kadar .NET Core olarak adlandırıldı. 
.NET Core 3.1'den sonraki bir sonraki sürüm, şu anda önizleme aşamasında olan .NET 5.0'dır. 4 numaralı sürüm, .NET'in bu uygulaması ile .NET Framework 4.8 arasındaki karışıklığı önlemek için atlandı. 
Artık .NET'in ana uygulaması olduğunu açıklığa kavuşturmak için "Çekirdek" adı bırakıldı.
# .NET 5 'e geçişte hedeflenenler
.NET 5, .NET Core'un evrimidir. Bu makale, 3.1'den sonra .NET Core'un bir sonraki sürümü olan .NET 5'e nelerin dahil olduğunu ayrıntılarıyla anlatmaktadır.
.NET Framework 4.x ile karışıklığı önlemek için sürüm numarası 5.0'dır. Ve "Core" isminden çıkarılır çünkü ileride .NET'in ana uygulamasıdır.
ASP.NET Core, ASP.NET MVC 5 ile karıştırılmasını önlemek için "Core" adını korur. Ayrıca Entity Framework Core, Entity Framework 5 ve 6 ile karıştırılmasını önlemek için "Core" adını korur.
.NET 5, .NET Core veya .NET Framework'ten daha fazla uygulama ve daha fazla platform.
-Tek dosyalı uygulamalar
-Windows ARM64 ve ARM64 temelleri
Aşağıdakiler için kapsamlı performans iyileştirmeleri:
- Çöp Toplama (GC)
- System.Text.Json
- System.Text.RegularExpressions
- Zaman uyumsuz ValueTask havuzu oluşturma
Konteyner boyutu optimizasyonları
Uygulama kırpma
C # derleyici geliştirmeleri
 Döküm hata ayıklaması için araç desteği
Platform, boş değer atanabilir referans türleri için% 80 ek açıklamalıdır
[kaynak](https://docs.microsoft.com/en-us/dotnet/core/dotnet-five)
# Markdown yazımı ve kullanımı
Markdown, web yazarları için bir metin-HTML dönüştürme aracıdır. Markdown, okuması kolay, yazması kolay bir düz metin formatı kullanarak yazmanıza,
ardından bunu yapısal olarak geçerli XHTML'ye (veya HTML) dönüştürmenize olanak tanır.
Dolayısıyla, "Markdown" iki şeydir: (1) düz metin biçimlendirme sözdizimi; ve (2) düz metin formatını HTML'ye dönüştüren Perl ile yazılmış bir yazılım aracı.
Markdown'un biçimlendirme sözdizimiyle ilgili ayrıntılar için Sözdizimi sayfasına bakın .
[yazım kuralları](https://guides.github.com/features/mastering-markdown/) 
# Yazılım alanında takip edilenler
- [Andrii siriak](https://github.com/siriak)
- [Tim Koehler](https://github.com/tim-koehler)
- [Andrew Arnott](https://github.com/AArnott)
- [Peter Thaleikis](https://github.com/spekulatius)

# iş ilanları 
- profizi [Linkedin](https://www.linkedin.com/jobs/view/2254857289/)
- PV complete [Linkedin](https://www.linkedin.com/jobs/view/2252515384/)
- Protel bilgisayar [kariyer.net](https://www.kariyer.net/is-ilani/protel-bilgisayar-a-s--net-developer-2192751)
- Mars [kariyer.net](https://www.kariyer.net/is-ilani/mars-kidemli-net-yazilim-muhendisi-2516067)

# Microsft azure hizmetleri
Microsoft Azure, Amazon Web Services (AWS) ve Google Cloud Platform'a benzer şekilde çalışan bir bulut platform ve bilgi işlem hizmetidir.
Alışıla gelmiş bulut servislerinin ve geleneksel tanımının aksine Microsoft Azure bulut platformuna ihtiyaç duyan şirketler, 
organizasyonlar ve hatta bulut platformun avantajlarından faydalanmak isteyen kişisel kullanıcılar için tasarlanmıştır. 
Microsoft Azure’dan edinmiş olduğunuz bulut platformunu kendi ihtiyaçlarınız doğrultusunda dilediğiniz gibi kullanabilirsiniz.
Bulut platformu size web sunucularını barındırma, e-mail sunucusu oluşturma, veritabanı sunucusu, dosya depolama sunucusu, 
sanal makineler, kullanıcı dizinleri, web uygulamaları, mobil uygulamalar veya istediğiniz herhangi farklı servisler olarak hizmet edebilirler. 
Satın aldığınız bulut platformu yalnızca kendi amaçlarınız için gizli olarak Private Cloud şeklinde kullanabileceğiniz gibi
tüm kullanıcıların erişimine açık olarak kullanabilirsiniz.
Azure Bulut platform servisinin adı ilk önce “Windows Azure” olarak belirlenmiş ancak sonradan “Microsoft Azure” olarak değiştirilmiştir. Azure’un isim değişikliğinin nedeni Windows’un dışında birçok işlev için kullanılabilmesinden kaynaklanıyor. Örneğin Azure platformuna kurduğunuz bir sanal sunucuyu Windows işletim sistemiyle güçlendirebileceğiniz gibi Linux veya farklı bir OS ile güçlendirebilirsiniz.
