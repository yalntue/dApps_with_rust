# III. Solana ve Akıllı Sözleşme Geliştirme Ortamının Kurulumu

## A. Geliştirme Ortamı Hazırlığı Akıllı sözleşme geliştirme sürecine başlamadan önce, geliştirme ortamınızı doğru şekilde hazırlamanız gerekmektedir. Aşağıdaki adımları izleyerek geliştirme ortamınızı kurabilirsiniz:

1.  IDE (Integrated Development Environment) Seçimi:



    * Bir IDE seçin ve kurun.&#x20;
    * IDE'nizi Solana'ya ve akıllı sözleşme geliştirmeye uygun bir şekilde yapılandırın.
    * Gerekli eklentileri ve araçları yükleyin.


2. Rust Derleyicisi:

*   **Windows için Rust Kurulumu:**



    1. Rust programlama dilini Windows işletim sisteminde kullanabilmek için öncelikle Rust'un resmi web sitesine ([https://www.rust-lang.org](https://www.rust-lang.org)) gidin.
    2. Sayfanın sağ üst köşesindeki "Install" düğmesine tıklayın ve indirme sayfasına yönlendirileceksiniz.
    3. İndirme sayfasında "rustup" adlı bir aracı indirme seçeneğiniz olacak. Bu araç, Rust dilini yönetmenize ve güncellemeleri almanıza olanak tanır.
    4. "rustup-init.exe" dosyasını indirin ve çalıştırın.
    5. Yükleme işlemi başladığında, size Rust kurulumunun lisansını ve kullanım koşullarını kabul etme seçeneği sunulacak. Kabul edin ve devam edin.
    6. Kurulum sırasında size varsayılan yapılandırma seçenekleri sunulacak. Genellikle önerilen seçenekleri kabul edebilirsiniz.
    7. Kurulum tamamlandığında, komut istemini yeniden başlatın ve Rust dilini kullanmaya başlayabilirsiniz.



*   **Linux için Rust Kurulumu:**



    * Linux işletim sisteminizde Rust dilini kullanabilmek için terminali açın.
    * Rust'un resmi web sitesine gidin ([https://www.rust-lang.org](https://www.rust-lang.org)) ve sayfanın sağ üst köşesindeki "Install" düğmesine tıklayın.
    * İndirme sayfasına yönlendirileceksiniz. Burada "rustup" adlı Rust yönetim aracını indirme seçeneğiniz olacak.
    * Terminalde aşağıdaki komutu girerek "rustup" aracını indirin ve kurun:\
      \


    `curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh`\


    * Kurulum işlemi başladığında size Rust kurulumunun lisansını ve kullanım koşullarını kabul etme seçeneği sunulacak. Kabul edin ve devam edin.
    * Kurulum sırasında size varsayılan yapılandırma seçenekleri sunulacak. Genellikle önerilen seçenekleri kabul edebilirsiniz.
    * Kurulum tamamlandığında, terminali yeniden başlatın ve Rust dilini kullanmaya başlayabilirsiniz.



*   **macOS için Rust Kurulumu:**



    * macOS işletim sisteminde Rust dilini kullanabilmek için öncelikle terminali açın.
    * Rust'un resmi web sitesine gidin ([https://www.rust-lang.org](https://www.rust-lang.org)) ve sayfanın sağ üst köşesindeki "Install" düğmesine tıklayın.
    * İndirme sayfasına yönlendirileceksiniz. Burada "rustup" adlı Rust yönetim aracını indirme seçeneğiniz olacak.
    * Terminalde aşağıdaki komutu girerek "rustup" aracını indirin ve kurun:

    \


    `curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh`

    \


    * Kurulum işlemi başladığında size Rust kurulumunun lisansını ve kullanım koşullarını kabul etme seçeneği sunulacak. Kabul edin ve devam edin.
    * Kurulum sırasında size varsayılan yapılandırma seçenekleri sunulacak. Genellikle önerilen seçenekleri kabul edebilirsiniz.
    * Kurulum tamamlandığında, terminali yeniden başlatın ve Rust dilini kullanmaya başlayabilirsiniz.

## B. Solana Ağlarına Bağlantı ve Testnet Ortamı Solana ağlarına bağlanarak geliştirme ve test işlemlerinizi gerçekleştirebilirsiniz. Aşağıdaki adımları izleyerek Solana ağlarına bağlanabilirsiniz:

1.  Solana Ağı Seçimi: İlk adım, hangi Solana ağına bağlanmak istediğinizi belirlemektir. Solana, Mainnet (ana ağ) ve test ağları (testnet) olmak üzere farklı ağlarda hizmet vermektedir. Geliştirme ve test amacıyla genellikle test ağları tercih edilir çünkü burada gerçek değerli varlıkların yerine test tokenleri kullanılır ve işlemler ücretsizdir. Bu şekilde, dApp'lerinizi ve akıllı sözleşmelerinizi risk almadan geliştirebilir ve test edebilirsiniz.


2.  Solana Cüzdanı Oluşturma: Solana ağına bağlanabilmek için bir Solana cüzdanına ihtiyacınız olacak. Solana cüzdanı, hesaplarınızı yönetmenize ve işlemlerinizi gerçekleştirmenize olanak sağlar. Solana cüzdanınızı oluşturmak için resmi Solana cüzdan uygulamasını (Sollet, Phantom vb.) veya Solana destekli bir cüzdan sağlayıcısını kullanabilirsiniz. Cüzdan oluşturma sürecinde size bir cüzdan adresi ve özel anahtar sağlanır. Bu özel anahtar, hesabınıza erişim sağlamak için kullanılmalıdır, bu nedenle güvenli bir şekilde saklamanız önemlidir.


3.  Solana Ağına Bağlanma: Solana ağına bağlanmak için Solana cüzdanınızı kullanmanız gerekmektedir. Solana destekli bir cüzdan uygulaması indirip kurduysanız, cüzdan uygulamasını açın ve cüzdanınıza giriş yapın. Ardından, cüzdanınızla Solana ağına bağlanmak için sağlanan seçenekleri kullanın. Genellikle cüzdan uygulamasında bir "Bağlan" veya "Connect" düğmesi bulunur. Bu düğmeye tıklayarak Solana ağına bağlanabilirsiniz.


4. Testnet Ortamına Bağlanma: Test ağlarına bağlanmak için Solana cüzdanınızı testnet modunda çalışacak şekilde yapılandırmanız gerekmektedir. Çoğu Solana cüzdan uygulamasında, ağ seçenekleri arasında "Mainnet" ve "Testnet" gibi seçenekler bulunur. Testnet seçeneğini seçerek Solana test ağına bağlanabilirsiniz. Bu şekilde, Solana testnetinde dApp'lerinizi ve akıllı sözleşmelerinizi geliştirmek ve test etmek için bir ortam elde edersiniz.



Solana ağlarına bağlanmak, geliştirme ve test sürecinizde önemli bir adımdır. Test ağlarını kullanarak işlemlerinizin güvenliğini ve doğruluğunu test edebilir, dApp'lerinizi gerçek dünyada kullanılabilir hale getirmeden önce çeşitli senaryolarda deneyimleyebilirsiniz.

## C. SDK'ların ve Araçların Kurulumu ve Kullanımı Solana geliştirme sürecini desteklemek için çeşitli SDK'lar ve araçlar mevcuttur. Aşağıdaki adımları izleyerek SDK'ları ve araçları kurabilir ve kullanabilirsiniz:

Anchor, Solana üzerinde dApp'lerin geliştirilmesi için kullanılan bir geliştirme platformudur. Anchor, Solana SDK'larına ek olarak daha yüksek seviye bir arayüz sağlar ve geliştiricilere akıllı sözleşme geliştirme sürecini kolaylaştırır.

* Windows için Anchor kurulumu:

Komut istemcisini (Command Prompt) açın.

Aşağıdaki komutu girerek Anchor CLI'ı yükleyin

`cargo install --git https://github.com/project-serum/anchor anchor-cli --locked`

* Kurulumu Doğrulama:



Komut istemcisini yeniden başlatın.

Aşağıdaki komutu girerek Anchor'ın doğru bir şekilde yüklendiğini doğrulayın:

```css
anchor --version
```

* Linux için Anchor kurulumu:

Komut istemcisini açın ve aşağıdaki komutu girin

* <pre class="language-arduino"><code class="lang-arduino"><strong><a data-footnote-ref href="#user-content-fn-1">cargo install --git https://github.com/project-serum/anchor anchor-cli --locked</a>
  </strong></code></pre>
* Kurulumu Doğrulama:



Yeni bir terminal açın.

Aşağıdaki komutu girerek Anchor'ın doğru bir şekilde yüklendiğini doğrulayın:

```css
anchor --version
```

* macOS için Anchor kurulumu:

Terminalde aşağıdaki komutu girin:



* ```arduino
  cargo install --git https://github.com/project-serum/anchor anchor-cli --locked
  ```
*   Kurulumu Doğrulama:



Yeni bir terminal açın.

Aşağıdaki komutu girerek Anchor'ın doğru bir şekilde yüklendiğini doğrulayın:

```css
anchor --version
```



#### Solana CLI(Solana Command Line Interface - Solana CLI), Solana ile etkileşimde bulunmak ve geliştirme işlemlerini yönetmek için kullanılan bir araçtır. Aşağıdaki adımları izleyerek Solana CLI'ı kurabilir ve kullanabilirsiniz:

Windows için Solana CLI Kurulumu:

1. Solana CLI'ı indirmek için[ https://docs.solana.com/cli/install-solana-cli-links](https://docs.solana.com/cli/install-solana-cli-links) adresine gidin.
2. "Windows Installer" seçeneğini tıklayarak indirme işlemini başlatın.
3. İndirilen Solana CLI yükleyiciyi çalıştırın ve kurulum sihirbazını takip edin.
4. Kurulum tamamlandığında, Solana CLI'ı kullanmaya hazır olacaksınız. Komut istemini açın ve `solana --version` komutunu çalıştırarak doğru şekilde yüklendiğini doğrulayabilirsiniz.

Linux için Solana CLI Kurulumu:

1. Terminali açın ve aşağıdaki komutu çalıştırarak Solana CLI'yı yükleyin:

\


* `sh -c "$(curl -sSfL https://release.solana.com/v1.9.7/install)"`

\
İşlem tamamlandığında, Solana CLI'ı kullanmaya hazır olacaksınız. `solana --version` komutunu çalıştırarak doğru şekilde yüklendiğini doğrulayabilirsiniz.

macOS için Solana CLI Kurulumu:

1. Terminali açın ve aşağıdaki komutu çalıştırarak Solana CLI'yı yükleyin:

\


* `sh -c "$(curl -sSfL https://release.solana.com/v1.9.7/install)"`

\


2. İşlem tamamlandığında, Solana CLI'ı kullanmaya hazır olacaksınız. `solana --version` komutunu çalıştırarak doğru şekilde yüklendiğini doğrulayabilirsiniz.

Not: Yukarıdaki komutlar, Solana CLI'ın belirli bir sürümünü yükler. Güncel sürümü yüklemek için Solana belgelerini kontrol etmeniz önemlidir. Ayrıca, komutları çalıştırırken güvenlik açısından dikkatli olun ve yalnızca güvenilir kaynaklardan indirme yapın.

## Bağlantı Ayarları



Solana CLI'ı kullanmadan önce Solana ağına bağlanmanız gerekmektedir. Aşağıda, Solana CLI üzerinde gerekli bağlantı ayarlarını yapılandırmanız için adımları bulabilirsiniz:

**Test Ağı veya Mainnet Seçimi:**



* Solana'nın test ağına (testnet) veya ana ağına (mainnet) bağlanma seçeneğiniz vardır.
* Geliştirme ve test amacıyla genellikle test ağı tercih edilir. Bu ağda işlemler gerçek para kullanılmadan denenebilir.
* Ana ağ, gerçek varlıkların ve işlemlerin bulunduğu ağdır. Gerçek para ile işlem yapmadan önce dikkatli olmanız önemlidir.



**Bağlantı Yapılandırması:**

Solana CLI üzerindeki bağlantı ayarlarını yapılandırmak için aşağıdaki komutları kullanabilirsiniz:



* Test Ağı için:\
  \
  `solana config set --url https://api.testnet.solana.com`



* Mainnet için:\
  \
  `solana config set --url https://api.mainnet-beta.solana.com`

\
**Bağlantıyı Kontrol Etme:**

* Bağlantı ayarlarını yapılandırdıktan sonra, Solana ağına başarılı bir şekilde bağlandığınızı doğrulamak için aşağıdaki komutu çalıştırabilirsiniz:\
  \
  `solana config get`

Bu adımları izleyerek Solana CLI üzerinde bağlantı ayarlarını yapılandırabilir ve Solana ağına başarıyla bağlanabilirsiniz.

### Solana CLI komutlarına kısa bir bakış

Solana CLI, Solana ağıyla etkileşimde bulunmanızı sağlayan bir dizi komut sunar. Bu komutlar aracılığıyla cüzdan oluşturma, bakiye sorgulama, akıllı sözleşme dağıtma, işlem gönderme gibi işlemleri gerçekleştirebilirsiniz. Solana CLI'nın sağladığı bazı temel komutlar şunlardır:

* Cüzdan Oluşturma: Solana CLI ile yeni bir cüzdan oluşturabilirsiniz. Cüzdanınız, hesaplarınızı ve varlıklarınızı yönetmek için kullanacağınız bir kimlik bilgisidir. Cüzdan oluşturmak için aşağıdaki komutu kullanabilirsiniz:\
  \
  `solana-keygen new`



* Bakiye Sorgulama: Solana CLI ile cüzdanınızdaki bakiyeyi sorgulayabilirsiniz. Bakiyenizi kontrol etmek için aşağıdaki komutu kullanabilirsiniz:\
  \
  `solana balance`



* Akıllı Sözleşme Dağıtma: Solana ağına akıllı sözleşme dağıtmak için Solana CLI'yı kullanabilirsiniz. Akıllı sözleşmelerinizi Solana ağına yüklemek için gerekli komutları çalıştırabilirsiniz. Örneğin:\
  \
  `solana program deploy <sözleşme-dosyası>.so`



* İşlem Gönderme: Solana CLI, Solana ağı üzerinde işlem göndermek için kullanılabilir. Ödeme yapmak, token transferi gerçekleştirmek veya akıllı sözleşme işlevlerini çağırmak gibi işlemleri gerçekleştirebilirsiniz. İşlem göndermek için aşağıdaki komutu kullanabilirsiniz:\
  \
  `solana transfer <hedef-adres> <miktar>`

\
Solana CLI'nın belgelerini inceleyerek kullanabileceğiniz diğer komutları ve işlemleri keşfedebilirsiniz. Solana CLI, Solana ağına bağlanarak akıllı sözleşme geliştirme sürecinde size birçok fayda sağlar. Bu aracı kullanarak geliştirme ve test işlemlerinizi kolayca yönetebilirsiniz.

[^1]: 
