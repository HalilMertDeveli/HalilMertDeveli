<div align="center">

# Halil Mert Develi

**.NET Backend & Full-Stack Software Engineer · Flutter & cross-platform mobile**
<br/>
<sub>.NET Backend ve Full-Stack Yazılım Mühendisi · Flutter ve çapraz platform mobil · İstanbul, Türkiye</sub>

<br/>

<a href="https://halilmertdeveli.com.tr"><img src="https://img.shields.io/badge/Portfolio-halilmertdeveli.com.tr-111111?style=flat-square" alt="Portfolio" /></a>
<a href="https://www.linkedin.com/in/halil-mert-develi-00983a225/"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
<a href="mailto:halilmertdeveliii@gmail.com"><img src="https://img.shields.io/badge/Email-D14836?style=flat-square&logo=gmail&logoColor=white" alt="Email" /></a>

<br/><br/>

<img src="https://skillicons.dev/icons?i=cs,dotnet,postgres,flutter,dart,nextjs,react,ts,firebase,supabase,docker,githubactions&theme=dark" alt="C#, .NET, PostgreSQL, Flutter, Dart, Next.js, React, TypeScript, Firebase, Supabase, Docker, GitHub Actions" />

<br/><br/>

<a href="#english">English</a> · <a href="#turkce">Türkçe</a>

</div>

| | |
|---|---|
| **Focus · Odak** | C# / ASP.NET Core backends, Flutter mobile apps · C# / ASP.NET Core backend'leri, Flutter mobil uygulamalar |
| **Domain · Alan** | LED display industry: support tooling, B2B commerce, service management · LED ekran sektörü: destek araçları, B2B ticaret, servis yönetimi |
| **Location · Konum** | Istanbul, Türkiye · İstanbul, Türkiye |
| **Open to · İlgi** | .NET backend, full-stack and Flutter roles · .NET backend, full-stack ve Flutter pozisyonları |

---

<a id="english"></a>

## About me

I'm a Computer Engineer who builds backend systems with **C# and ASP.NET Core**, and cross-platform mobile apps with **Flutter**.

Most of my work happens in the LED display industry: support tooling, B2B commerce and service-management platforms, where the hard part is modelling a messy domain correctly. I care about layered architecture, explicit domain models, tests that run against real databases, and APIs that are boring to consume.

## Core engineering skills

| Area | Skills |
|---|---|
| Backend & APIs | ASP.NET Core, REST, Razor Pages / MVC, EF Core, authentication and role-based authorization |
| Architecture | Clean / Onion / layered architecture, domain modelling, idempotent operations, ports and adapters |
| Data | PostgreSQL, SQL Server, Cloud Firestore, Supabase, migrations and integration tests on real databases |
| Mobile | Flutter and Dart for Android and iOS, Firebase, some native Android with Kotlin and Jetpack Compose |
| Web front end | Next.js, React, TypeScript |
| Delivery | Docker, GitHub Actions CI, Vercel container deployments |
| Integrations | Payment providers, email, WhatsApp and LLM APIs with validation and failure handling |

## Featured projects

### Open source

| Project | What it is | Stack |
| --- | --- | --- |
| [**LEDCare OS**](https://github.com/HalilMertDeveli/LEDCare-OS) | Service-management platform for LED screen technical support: a web app, a mobile app and an API, with CI that runs backend tests on real PostgreSQL, web E2E tests and an Android build. In development. | ASP.NET Core · EF Core · PostgreSQL · SignalR · Next.js · React · Flutter |
| [**ASP.NET-APP-FOR-LED**](https://github.com/HalilMertDeveli/ASP.NET-APP-FOR-LED) | Live support website for Colorlight, NovaStar and Huidu LED control systems: request form, Google sign-in, realtime customer chat and an admin panel. [Live site](https://asp-net-app-for-led.vercel.app) | ASP.NET Core 8 · Razor Pages · Supabase · Resend · Vercel |
| [**TaskManagementSystem**](https://github.com/HalilMertDeveli/TaskManagementSystem) | My Computer Engineering capstone: a task manager with Admin and Member roles, built with Onion architecture. | ASP.NET Core MVC · MediatR · FluentValidation · EF Core · SQL Server |
| [**yazilim-sitesi**](https://github.com/HalilMertDeveli/yazilim-sitesi) | My portfolio site, with small playable demos of my products and a printable recruiter brief. [Live site](https://halilmertdeveli.com.tr) | ASP.NET Core 8 · Razor Pages · vanilla JS · Docker |

### Private product work

The source of these lives in private repositories. You can try small demos of the first four on [my portfolio](https://halilmertdeveli.com.tr).

| Project | What it is | Stack | Status |
| --- | --- | --- | --- |
| **Mevora** | Dating app that shows why two people match and keeps exact location private; matching, safety rules and moderation run on the server. | Flutter · Firebase · Cloud Functions (TypeScript) | Pre-launch |
| **LED B2B Platform** | Managed B2B platform that turns an LED screen request into a configured, priced order, with suppliers and costs hidden from the customer. | .NET 10 · ASP.NET Core · EF Core · PostgreSQL | Not publicly available |
| **Motor** | E-commerce site for a motorcycle parts business, with parts searched by make, model and year. | .NET 10 · ASP.NET Core · EF Core · PostgreSQL · Docker | Demo stage |
| **LED Support Bot** | WhatsApp intake system that collects a technician's diagnostic details, then hands the conversation to a human. | .NET 8 · ASP.NET Core · PostgreSQL · Node.js | In testing |
| **ClearPay** | Demo digital wallet on a double-entry ledger, with web and Flutter clients. | .NET 8 · SQL Server · Hangfire · Flutter | Demo |

## Engineering highlights

- **Tests against real infrastructure.** The LED B2B Platform's suite runs locally against PostgreSQL (last recorded run: 2,691 passed). [LEDCare OS](https://github.com/HalilMertDeveli/LEDCare-OS) runs backend tests on real PostgreSQL, contract and web E2E tests, mobile analysis and an Android build in GitHub Actions.
- **Money handled carefully.** ClearPay derives balances from a double-entry ledger instead of updating them, and transfers are idempotent: a replayed request returns `409`.
- **Pricing safety through types.** In the LED B2B Platform, supplier cost, platform margin and customer price are separate value objects, so cost and sale price can't be mixed up.
- **Trust moved to the server.** Mevora computes matches, applies safety rules and validates purchases in Cloud Functions rather than on the client.
- **Deterministic first, AI second.** The LED Support Bot parses sizes, counts and IDs with plain code; an LLM is only called behind a cost gate, with a strict JSON schema and validation.

## GitHub activity

<p>
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://streak-stats.demolab.com/?user=HalilMertDeveli&theme=github-dark-blue&hide_border=true&border_radius=8" />
    <img src="https://streak-stats.demolab.com/?user=HalilMertDeveli&theme=default&hide_border=true&border_radius=8" alt="GitHub contribution streak for HalilMertDeveli" />
  </picture>
</p>

## Portfolio & contact

- **Portfolio** — [halilmertdeveli.com.tr](https://halilmertdeveli.com.tr)
- **LinkedIn** — [halil-mert-develi](https://www.linkedin.com/in/halil-mert-develi-00983a225/)
- **Email** — [halilmertdeveliii@gmail.com](mailto:halilmertdeveliii@gmail.com)

Open to conversations about .NET backend, full-stack and Flutter roles.

<p align="right"><a href="#english">Back to top ↑</a></p>

---

<a id="turkce"></a>

## Hakkımda

**C# ve ASP.NET Core** ile backend sistemleri, **Flutter** ile çapraz platform mobil uygulamalar geliştiren bir Bilgisayar Mühendisiyim.

Çalışmalarımın çoğu LED ekran sektöründe geçiyor: destek araçları, B2B ticaret ve servis yönetimi platformları. Bu işlerde asıl zorluk, karmaşık bir alanı doğru modellemek. Katmanlı mimariye, açık domain modellerine, gerçek veritabanlarına karşı çalışan testlere ve kullanımı sürpriz içermeyen, sade API'lere önem veriyorum.

## Temel mühendislik becerileri

| Alan | Beceriler |
|---|---|
| Backend ve API'ler | ASP.NET Core, REST, Razor Pages / MVC, EF Core, kimlik doğrulama ve rol tabanlı yetkilendirme |
| Mimari | Clean / Onion / katmanlı mimari, domain modelleme, idempotent işlemler, ports and adapters |
| Veri | PostgreSQL, SQL Server, Cloud Firestore, Supabase, migration'lar ve gerçek veritabanlarında entegrasyon testleri |
| Mobil | Android ve iOS için Flutter ve Dart, Firebase, Kotlin ve Jetpack Compose ile bir miktar native Android |
| Web ön yüz | Next.js, React, TypeScript |
| Teslimat | Docker, GitHub Actions CI, Vercel container dağıtımları |
| Entegrasyonlar | Doğrulama ve hata yönetimiyle ödeme sağlayıcıları, e-posta, WhatsApp ve LLM API'leri |

## Öne çıkan projeler

### Açık kaynak

| Proje | Nedir | Teknoloji |
| --- | --- | --- |
| [**LEDCare OS**](https://github.com/HalilMertDeveli/LEDCare-OS) | LED ekran teknik desteği için servis yönetimi platformu: web uygulaması, mobil uygulama ve API; CI üzerinde gerçek PostgreSQL ile backend testleri, web E2E testleri ve Android build'i çalışır. Geliştirme aşamasında. | ASP.NET Core · EF Core · PostgreSQL · SignalR · Next.js · React · Flutter |
| [**ASP.NET-APP-FOR-LED**](https://github.com/HalilMertDeveli/ASP.NET-APP-FOR-LED) | Colorlight, NovaStar ve Huidu LED kontrol sistemleri için canlı destek sitesi: talep formu, Google ile giriş, gerçek zamanlı müşteri sohbeti ve yönetim paneli. [Canlı site](https://asp-net-app-for-led.vercel.app) | ASP.NET Core 8 · Razor Pages · Supabase · Resend · Vercel |
| [**TaskManagementSystem**](https://github.com/HalilMertDeveli/TaskManagementSystem) | Bilgisayar Mühendisliği bitirme projem: Onion mimarisiyle geliştirilmiş, Yönetici ve Üye rollerine sahip görev yönetim uygulaması. | ASP.NET Core MVC · MediatR · FluentValidation · EF Core · SQL Server |
| [**yazilim-sitesi**](https://github.com/HalilMertDeveli/yazilim-sitesi) | Ürünlerimin küçük, denenebilir demolarını ve yazdırılabilir bir işe alım özetini içeren portföy sitem. [Canlı site](https://halilmertdeveli.com.tr) | ASP.NET Core 8 · Razor Pages · vanilla JS · Docker |

### Gizli ürün çalışmaları

Bu projelerin kaynak kodu gizli depolardadır. İlk dördünün küçük demolarını [portföyümde](https://halilmertdeveli.com.tr) deneyebilirsiniz.

| Proje | Nedir | Teknoloji | Durum |
| --- | --- | --- | --- |
| **Mevora** | İki kişinin neden eşleştiğini gösteren ve kesin konumu gizli tutan bir tanışma uygulaması; eşleştirme, güvenlik kuralları ve moderasyon sunucuda çalışır. | Flutter · Firebase · Cloud Functions (TypeScript) | Yayın öncesi |
| **LED B2B Platform** | Bir LED ekran talebini yapılandırılmış ve fiyatlandırılmış bir siparişe dönüştüren, tedarikçi ve maliyetleri müşteriden gizleyen yönetilen B2B platformu. | .NET 10 · ASP.NET Core · EF Core · PostgreSQL | Herkese açık değil |
| **Motor** | Parçaların marka, model ve yıla göre arandığı, motosiklet yedek parça işletmesi için e-ticaret sitesi. | .NET 10 · ASP.NET Core · EF Core · PostgreSQL · Docker | Demo aşamasında |
| **LED Support Bot** | Teknisyenin arıza bilgilerini toplayıp görüşmeyi bir insana devreden WhatsApp talep sistemi. | .NET 8 · ASP.NET Core · PostgreSQL · Node.js | Test aşamasında |
| **ClearPay** | Çift taraflı kayıt (double-entry ledger) üzerine kurulu, web ve Flutter istemcili demo dijital cüzdan. | .NET 8 · SQL Server · Hangfire · Flutter | Demo |

## Mühendislik notları

- **Gerçek altyapıya karşı testler.** LED B2B Platform'un test paketi yerelde PostgreSQL'e karşı çalışır (son kayıtlı çalıştırma: 2.691 başarılı test). [LEDCare OS](https://github.com/HalilMertDeveli/LEDCare-OS), GitHub Actions üzerinde gerçek PostgreSQL ile backend testlerini, contract ve web E2E testlerini, mobil analizi ve Android build'ini çalıştırır.
- **Paraya özen.** ClearPay bakiyeleri güncellemek yerine çift taraflı kayıttan türetir; transferler idempotent'tir: tekrar gönderilen istek `409` döner.
- **Tiplerle fiyat güvenliği.** LED B2B Platform'da tedarikçi maliyeti, platform marjı ve müşteri fiyatı ayrı value object'lerdir; bu sayede maliyet ve satış fiyatı karıştırılamaz.
- **Güven sunucuda.** Mevora eşleşmeleri hesaplamayı, güvenlik kurallarını uygulamayı ve satın alma doğrulamasını istemci yerine Cloud Functions'ta yapar.
- **Önce deterministik, sonra yapay zekâ.** LED Support Bot ölçüleri, adetleri ve kimlikleri düz kodla ayrıştırır; LLM yalnızca bir maliyet kapısının arkasında, katı bir JSON şeması ve doğrulamayla çağrılır.

## GitHub etkinliği

Katkı serisi kartı yukarıdaki [GitHub activity](#github-activity) bölümünde yer alır.

## Portföy ve iletişim

- **Portföy** — [halilmertdeveli.com.tr](https://halilmertdeveli.com.tr)
- **LinkedIn** — [halil-mert-develi](https://www.linkedin.com/in/halil-mert-develi-00983a225/)
- **E-posta** — [halilmertdeveliii@gmail.com](mailto:halilmertdeveliii@gmail.com)

.NET backend, full-stack ve Flutter pozisyonlarıyla ilgili görüşmelere açığım.

<p align="right"><a href="#turkce">Başa dön ↑</a></p>

<br/>

<p align="center"><sub>README style: <a href="docs/README_VISUAL_BILINGUAL_STANDARD.md">visual bilingual standard</a> · README biçimi: görsel iki dilli standart</sub></p>
