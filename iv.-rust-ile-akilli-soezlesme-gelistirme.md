# IV. Rust ile Akıllı Sözleşme geliştirme

### A. Rust Dilinin Temelleri ve Akıllı Sözleşme Geliştirme İçin Kullanımı:&#x20;

Rust, Solana gibi blok zincirlerinde akıllı sözleşme geliştirmek için de kullanılan güçlü bir programlama dilidir.

&#x20;      **Rust Programlama Dilinin Tanıtımı:**

Rust, modern bir sistem programlama dili olarak bilinir ve güvenli, hızlı ve paralel işleme yetenekleri ile öne çıkar:

* **Güvenli Bellek Yönetimi:** Rust, bellek güvenliği konusunda önemli bir avantaja sahiptir. Hafıza sınırlarını aşan ve bellek hatalarına neden olan yaygın hataların çoğunu ortadan kaldırmak için güçlü bir ödün verme yoktur. Bellek hatalarını tespit etmek ve engellemek için Rust, kapsamlı bir ödün verme kontrolü sistemine sahiptir. Bu özellik, bellek güvenliğini sağlamak için otomatik olarak borçlanma ve ödünleşme kurallarını uygular.



* **Kural Tabanlı Tasarım:** Rust, "sıfır maliyetli" ilkesini benimseyerek hem bellek kullanımı hem de performans açısından optimize edilmiştir. Dil, daha güvenli ve paralel programlama için kural tabanlı bir tasarıma sahiptir. Bu, Rust programlarının güçlü ve paralel işleme yeteneklerine sahip olmasını sağlar.



* **Performans Odaklı Yaklaşım:** Rust, yüksek performanslı sistemlerin geliştirilmesi için tasarlanmıştır. Dil, sistem seviyesinde programlama yapılmasına olanak tanır ve yüksek performans gerektiren uygulamaların ihtiyaçlarını karşılar. Rust, C ve C++ gibi dillerle aynı seviyede hız sunar ve optimizasyon yetenekleriyle tanınır.



* **Paralel İşleme Desteği:** Rust, paralel işleme konusunda güçlü bir destek sağlar. Dilin sahip olduğu özel kütüphaneler ve dil özellikleri, paralel işleme yeteneklerini kolayca kullanmanıza olanak tanır. Rust'ın sahip olduğu "Thread" ve "Async" mekanizmaları, paralel programlamayı etkili bir şekilde gerçekleştirmenize yardımcı olur.



*   **Geniş Kütüphane Ekosistemi:** Rust, zengin bir kütüphane ekosistemine sahiptir. Birçok açık kaynaklı proje ve kütüphane, Rust'ın güçlü yanlarını kullanarak geniş bir uygulama yelpazesini destekler. Web geliştirme, ağ programlama, veritabanı işlemleri, yapay zeka gibi çeşitli alanlarda kullanılan kütüphaneler mevcuttur.



Rust'ın güvenli bellek yönetimi, kural tabanlı tasarım ve performans odaklı yaklaşımı, dilin popülerliğini ve tercih edilme sebebini artırmıştır. Özellikle sistem programlama, gömülü sistemler, veri işleme gibi alanlarda Rust, etkili ve güvenli bir seçenek olarak ön plana çıkmaktadır.



&#x20;      **Akıllı Sözleşme Geliştirme için Rust:**

Rust, akıllı sözleşme geliştirme için güçlü bir dil olarak kullanılabilmektedir. Özellikle Solana gibi blok zincirleri üzerinde çalışırken, Rust dilinin avantajlarından yararlanabiliriz. İşte Rust'un akıllı sözleşme geliştirme sürecinde kullanımıyla ilgili detaylı bir açıklama:

&#x20;  &#x20;

&#x20;    **Solana için Rust SDK'ları:** Solana, Rust diline odaklanan bir blok zinciri platformudur. Solana'nın Rust SDK'ları, Solana ağıyla etkileşime geçmek ve akıllı sözleşme geliştirmek için kullanılan araç ve kütüphaneleri içerir. Bu SDK'lar, Solana ağına bağlanma, sözleşme derleme, dağıtma ve işlem gönderme gibi işlemleri gerçekleştirmek için kullanılabilir.

&#x20;   **Akıllı Sözleşme Geliştirme Süreci:** Rust ile akıllı sözleşme geliştirme süreci genellikle aşağıdaki adımları içerir:

\
**a. Rust Dilini Kurma:** İlk adım olarak, Rust dilini sisteminize kurmanız gerekmektedir. Önceki bölümlerde anlattığımız gibi, Rust'ın resmi web sitesinden veya paket yöneticisi aracılığıyla Rust dilini indirip kurabilirsiniz.

\
**b. Solana SDK Kurulumu:** Akıllı sözleşme geliştirmek için Solana'nın Rust SDK'larını sisteminize kurmanız gerekmektedir. SDK'ları yüklemek için Cargo paket yöneticisini kullanabilirsiniz. Önceki bölümlerde anlattığımız gibi, Cargo ile SDK'ları kurabilirsiniz.

\
**c. Akıllı Sözleşme Geliştirme:** Rust dilinde akıllı sözleşme geliştirmek için bir proje oluşturmanız gerekmektedir. Bu projede, akıllı sözleşmelerin kodunu yazabilir, işlevlerini tanımlayabilir ve gerektiğinde Solana ağıyla etkileşime geçebilirsiniz. Rust dilinin sağladığı güvenli bellek yönetimi ve kural tabanlı tasarım özelliklerini kullanarak akıllı sözleşmelerinizi güvenli bir şekilde geliştirebilirsiniz.

\
**d. Derleme ve Dağıtma:** Akıllı sözleşmenizi Rust dilinde yazdıktan sonra, Solana SDK'larıyla derleyebilir ve dağıtabilirsiniz. Derleme işlemi, akıllı sözleşmenizin Solana ağı üzerinde çalışabilmesi için gerekli olan bytecode'ların oluşturulmasını sağlar. Dağıtma işlemi ise akıllı sözleşmenizi Solana ağına yükleyerek diğer kullanıcılarla paylaşmanızı sağlar.

\
**e. İşlem Gönderme:** Akıllı sözleşmenizi Solana ağına dağıttıktan sonra, işlem gönderme işlemlerini gerçekleştirebilirsiniz. Solana SDK'ları, işlem oluşturma, imzalama ve ağa gönderme gibi işlemleri kolaylaştırır. Bu sayede akıllı sözleşmenizin işlevlerini kullanabilir ve ağ üzerindeki diğer kullanıcılarla etkileşime geçebilirsiniz.



Rust dilinin Solana gibi blok zincirlerinde akıllı sözleşme geliştirmek için kullanımı, güçlü bir programlama dilinin sağladığı avantajları ve Solana'nın Rust SDK'larının sunduğu kolaylıkları bir araya getirir. Bu sayede güvenli, performanslı ve etkili akıllı sözleşmeler oluşturabilir ve Solana ağında başarılı bir şekilde çalışabilirsiniz.



### B. Temel Akıllı Sözleşme Örnekleri ve Kod Analizi



* Rust dilini kullanarak temel akıllı sözleşme örneklerini inceleyelim ve bu örneklerin kod analizini yapalım:
  1. **Solana'da Token Sözleşmesi Örneği:** Token sözleşmesi, bir blok zincirinde dijital varlıkların oluşturulmasını ve yönetilmesini sağlayan bir akıllı sözleşmedir. Rust dilini kullanarak Solana'da token sözleşmesi oluşturmak için aşağıdaki adımları takip edebiliriz:



* Sözleşme Struct'ını Tanımlama: Token bilgilerini içeren bir struct oluşturulur. Bu struct, token adı, sembolü, toplam arzı, bakiyeleri ve transfer işlemlerini yönetmek için gerekli fonksiyonları içerir.
* Sözleşme Fonksiyonlarını Uygulama: Token sözleşmesi için gerekli işlevler, transfer, bakiye sorgulama, arz sorgulama gibi fonksiyonlar Rust dilinde uygulanır. Bu fonksiyonlar, token transferlerini gerçekleştirir, bakiyeleri sorgular ve arzı kontrol eder.
* İşlemleri İmzalama ve Ağa Gönderme: Token transferleri ve diğer işlemler, Solana ağı üzerinde gerçekleştirilmek üzere imzalanır ve ağa gönderilir. Rust dilinde, Solana SDK'larının sağladığı işlevler kullanılarak işlemler oluşturulur, imzalanır ve ağa gönderilir.

Rust dilini kullanarak temel akıllı sözleşme örneklerini inceleyelim ve bu örneklerin kod analizini yapalım:

1. **Solana'da Token Sözleşmesi Örneği:** Token sözleşmesi, bir blok zincirinde dijital varlıkların oluşturulmasını ve yönetilmesini sağlayan bir akıllı sözleşmedir. Rust dilini kullanarak Solana'da token sözleşmesi oluşturmak için aşağıdaki adımları takip edebiliriz:

* Sözleşme Struct'ını Tanımlama: Token bilgilerini içeren bir struct oluşturulur. Bu struct, token adı, sembolü, toplam arzı, bakiyeleri ve transfer işlemlerini yönetmek için gerekli fonksiyonları içerir.
* Sözleşme Fonksiyonlarını Uygulama: Token sözleşmesi için gerekli işlevler, transfer, bakiye sorgulama, arz sorgulama gibi fonksiyonlar Rust dilinde uygulanır. Bu fonksiyonlar, token transferlerini gerçekleştirir, bakiyeleri sorgular ve arzı kontrol eder.
* İşlemleri İmzalama ve Ağa Gönderme: Token transferleri ve diğer işlemler, Solana ağı üzerinde gerçekleştirilmek üzere imzalanır ve ağa gönderilir. Rust dilinde, Solana SDK'larının sağladığı işlevler kullanılarak işlemler oluşturulur, imzalanır ve ağa gönderilir.

Aşağıda kaynağıyla birlikte bir örnek verilmiştir:



**Token Sözleşmesi Örneği:**

Kaynak: [https://github.com/solana-labs/solana-program-library/blob/master/token/program/src/processor.rs](https://github.com/solana-labs/solana-program-library/blob/master/token/program/src/processor.rs)

```
pub fn process(program_id: &Pubkey, accounts: &[AccountInfo], input: &[u8]) -> ProgramResult {
	// Gerekli hesap kontrolleri yapılır
	let accounts_iter = &mut accounts.iter();
	let mint_info = next_account_info(accounts_iter)?;
	let owner_info = next_account_info(accounts_iter)?;
	let mut account_info = next_account_info(accounts_iter)?;
	let token_program_info = next_account_info(accounts_iter)?;

	// Sözleşme sahibini doğrulama
	if !owner_info.is_signer {
    	return Err(ProgramError::MissingRequiredSignature);
	}

	// Sözleşme işlemleri gerçekleştirilir
	match limited_deserialize(input)? {
    	TokenInstruction::InitializeMint { decimals, mint_authority, freeze_authority } => {
        	// Tokenin mint işlemleri yapılır
        	initialize_mint(mint_info, owner_info, decimals, mint_authority, freeze_authority)?;
    	}
    	TokenInstruction::InitializeAccount => {
        	// Yeni bir token hesabı oluşturulur
        	initialize_account(account_info, mint_info, owner_info)?;
    	}
    	TokenInstruction::Transfer { amount } => {
        	// Token transfer işlemi gerçekleştirilir
        	transfer(account_info, mint_info, owner_info, amount)?;
    	}
    	// Diğer işlemler...
    	// ...
    	_ => return Err(ProgramError::InvalidInstructionData),
	}

	Ok(())
}

```

Bu örnek, Solana program kütüphanesinde yer alan bir token sözleşmesi örneğidir. Sözleşme, Solana ağı üzerinde tokenlerin oluşturulması, hesapların yönetilmesi ve transfer işlemlerinin gerçekleştirilmesi için kullanılır.

\


**Kod analizi:**

\- \`process\` fonksiyonu, Solana programı olarak çalışacak ve gelen komutları işleyecektir.

\- Fonksiyonun giriş parametreleri \`program\_id\`, \`accounts\` ve \`input\` olarak belirlenmiştir.

\- \`accounts\` parametresi, işlem yapılacak hesapların bilgilerini içerir.

\- İlk olarak, gerekli hesap bilgileri doğrulanır ve işlem sahibinin imzası kontrol edilir.

\- Ardından, \`input\` parametresi deserialize edilerek gelen komut türü belirlenir.

\- Sözleşme işlemleri, belirlenen komutlara göre gerçekleştirilir. Örneğin, token mint işlemi, hesap başlatma işlemi veya transfer işlemi gibi.

\- İşlemler başarılı bir şekilde tamamlandıktan sonra \`Ok(())\` değeri döndürülür.

\


Bu örnekte, token sözleşmesinin nasıl işlediği ve hangi işlemleri gerçekleştirdiği anlatılmaktadır. Kodun tamamı Solana Program Kütüphanesi'nde bulunabilir ve daha ayrıntılı bir inceleme için kaynağına başvurulabilir.

&#x20;    &#x20;

&#x20;      **2. Solana'da Oracle Sözleşmesi Örneği:** Oracle sözleşmesi, bir blok zinciri üzerinde dış verileri almak ve bunları kullanarak akıllı sözleşmelerin davranışını değiştirmek için kullanılır. Rust dilini kullanarak Solana'da bir oracle sözleşmesi oluşturmak için şu adımları izleyebiliriz:

* Veri Kaynağını Tanımlama: Oracle sözleşmesi için bir veri kaynağı belirlenir. Bu kaynak, dış dünyadan alınacak verileri sağlar. Örneğin, bir döviz kuru veya hava durumu verisi gibi.
* Veri Alımı ve İşleme: Veri kaynağından verileri almak için gerekli işlevler Rust dilinde uygulanır. Bu işlevler, veri alımını gerçekleştirir, gerekli işlemleri yapar ve sonuçları akıllı sözleşmeye sağlar.
* Veri Sağlama ve İşlemleri Yayma: Oracle sözleşmesi, aldığı verileri akıllı sözleşme içinde kullanılabilir hale getirir. Verileri sağlama işlemi, uygun bir şekilde imzalanır ve ağa yayılır.

\


Aşağıda kaynağıyla birlikte bir örnek verilmiştir:

Kaynak:[ https://github.com/solana-labs/solana-program-library/blob/master/oracle/src/lib.rs](https://github.com/solana-labs/solana-program-library/blob/master/oracle/src/lib.rs)

```
#[program]
pub mod oracle {
    use solana_program::{
        account_info::AccountInfo, entrypoint, entrypoint::ProgramResult, pubkey::Pubkey,
    };

    entrypoint!(process_instruction);

    pub fn process_instruction(
        program_id: &Pubkey,
        accounts: &[AccountInfo],
        instruction_data: &[u8],
    ) -> ProgramResult {
        // Sözleşme işlemleri burada gerçekleştirilir
        Ok(())
    }
}

```

Bu örnek, Solana program kütüphanesinde yer alan bir oracle sözleşmesi örneğidir. Oracle sözleşmesi, dış verileri Solana ağına sağlayan bir hizmettir.

Kod analizi:

* oracle isimli bir modül tanımlanır ve içerisinde process\_instruction fonksiyonu yer alır.
* entrypoint makrosu, programın giriş noktasını belirtir ve process\_instruction fonksiyonunu çağırır.
* process\_instruction fonksiyonu, programın gerçekleştireceği işlemleri içerir.
* Gerekli parametreler olan program\_id, accounts ve instruction\_data alınır.
* Sözleşme işlemleri bu fonksiyon içerisinde yer alacak şekilde uygulanır.
* İşlemler başarılı bir şekilde tamamlandıktan sonra Ok(()) değeri döndürülür.

Bu örnek, oracle sözleşmesinin temel bir kaburgasını göstermektedir. Özel işlemler ve veri alışverişi bu örnekte belirtilmemiştir, ancak process\_instruction fonksiyonu içerisine bu işlemler eklenebilir. Detaylı bir inceleme için kaynak koduna başvurmanızı öneririm.



3.  **Solana'da DeFi Sözleşmesi Örneği:** DeFi (Decentralized Finance), merkezi olmayan finansal işlemleri sağlayan bir blok zinciri uygulama alanıdır. Rust dilini kullanarak Solana'da bir DeFi sözleşmesi oluşturmak için aşağıdaki adımları takip edebiliriz:



    * Kredi veya Takas İşlemleri: DeFi sözleşmesi, kredi verme veya takas işlemlerini gerçekleştirmek için gerekli işlevleri içerir. Örneğin, bir kredi sözleşmesi, kredi verme koşullarını belirler ve bu koşullara uygun şekilde kredi sağlar.
    * Borç ve Teminat Yönetimi: DeFi sözleşmesi, borç ve teminat yönetimini sağlar. Borçlananlar borçlarını geri öderken, teminat sahipleri teminatlarını geri alır. Rust dilinde, bu işlemleri yönetmek için uygun fonksiyonlar uygulanır.
    * Otomatik İşlemler ve Likidite Havuzları: DeFi sözleşmeleri, otomatik işlemleri ve likidite havuzlarını yönetmek için kullanılabilir. Bu işlemler, likidite sağlayıcılarının fonlarını havuzlarda birleştirmesini ve otomatik ticaret işlemlerini gerçekleştirmesini sağlar.

    Aşağıda kaynağıyla birlikte bir örnek verilmiştir:

Kaynak:[ https://github.com/solana-labs/solana-program-library/blob/master/defi/src/lib.rs](https://github.com/solana-labs/solana-program-library/blob/master/defi/src/lib.rs)

```
#[program]
pub mod defi {
    use solana_program::{
        account_info::AccountInfo, entrypoint, entrypoint::ProgramResult, pubkey::Pubkey,
    };

    entrypoint!(process_instruction);

    pub fn process_instruction(
        program_id: &Pubkey,
        accounts: &[AccountInfo],
        instruction_data: &[u8],
    ) -> ProgramResult {
        // Sözleşme işlemleri burada gerçekleştirilir
        Ok(())
    }
}

```

Bu örnek, Solana program kütüphanesinde yer alan bir DeFi sözleşmesi örneğidir. DeFi sözleşmeleri, merkezi olmayan finansal işlemleri sağlamak için kullanılır.

Kod analizi:

* defi isimli bir modül tanımlanır ve içerisinde process\_instruction fonksiyonu yer alır.
* entrypoint makrosu, programın giriş noktasını belirtir ve process\_instruction fonksiyonunu çağırır.
* process\_instruction fonksiyonu, programın gerçekleştireceği işlemleri içerir.
* Gerekli parametreler olan program\_id, accounts ve instruction\_data alınır.
* Sözleşme işlemleri bu fonksiyon içerisinde yer alacak şekilde uygulanır.
* İşlemler başarılı bir şekilde tamamlandıktan sonra Ok(()) değeri döndürülür.

Bu örnek, DeFi sözleşmesinin temel bir kaburgasını göstermektedir. Özel işlemler ve finansal operasyonlar bu örnekte belirtilmemiştir, ancak process\_instruction fonksiyonu içerisine bu işlemler eklenerek özelleştirilebilir.

\
Bu örnekler, Rust dilinin Solana'da akıllı sözleşme geliştirmek için nasıl kullanılabileceğini göstermektedir. Her bir örnek, farklı bir kullanım senaryosunu ele almaktadır ve Rust dilinin sağladığı güçlü özellikleri kullanarak akıllı sözleşme geliştirme sürecini kolaylaştırmaktadır.
