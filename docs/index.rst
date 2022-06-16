Solidity
========

Solidity  akıllı kontratlar geliştirmek için kullanılan, nesneye dayalı, yüksek seviye bir
programlama dilidir. Akıllı kontratlar, Ethereum hesaplarının davranışlarını yöneten programlardır.

Solidity, Ethereum Sanal Makinesi (EVM) için tasarlanmış, `süslü parantez kullanan programlama dilidir <https://en.wikipedia.org/wiki/List_of_programming_languages_by_type#Curly-bracket_languages>`_.
C++, Python ve JavaScript programlama dillerinden etkilenmiştir. Solidity diline ilham veren programlama dilleri hakkında daha fazla bilgiye :doc:`dil etkileri <language-influences>` bölümünde ulaşılaiblir.

Solidity statik bir dildir; desteklediği birçok özellikle birlikte, nesnel programlamanın kalıtım özelliğini,
kütüphaneleri ve kullanıcılar tarafından tanımlanabilen karmaşık veri tiplerini destekler.

Solidity ile oylama, kitlesel fonlama, kapalı müzayede ve çok kilitli cüzdanlarda kullanılmak üzere
kontratlar oluşturulabilir.

Kontratları yayımlarken, Solidity'nin son sürümü kullanılmalıdır. İstisnai bazı durumlar hariç
`güvenlik güncellemelerini <https://github.com/ethereum/solidity/security/policy#supported-versions>`_
yalnızca son sürüm almaktadır. Ayrıca, önceki sürümlerle uyumsuzluk oluşturabilecek değişiklikler,
yeni özellikler sıklıkla duyurulmaktadır. Mevcut durumda, `hızlı güncelleme temposunu gösterebilmek için <https://semver.org/#spec-item-4>`_ 
0.y.z sürüm numaraları kullanılmaktadır.

.. warning::

  Solidity'nin son yayınlanan 0.8.x sürümü önceki sürümlerle uyumsuzluk içeren
  birçok değişiklik barındırmaktadır. Bu değişikliklerin :doc:`tüm listesini <080-breaking-changes>`
  okuyunuz.

Solidity'nin veya bu dokümantasyonun gelişmesini sağlayacak her fikire açığız,
daha fazla bilgi için :doc:`katkı sağlama rehberini <contributing>` inceleyiniz.

.. Hint::

  Bu dokümantasyonu PDF, HTML veya Epub formatında indirmek için sol alt köşede yer alan
  sürüm menüsünden istenen format seçilebilir.

Başlangıç
---------

**1. Akıllı Kontrat Temellerini Anlama**

Akıllı kontrat konseptine yeni olanlar için "Akıllı Kontratlara Giriş" bölümünden başlanabilir,
bu bölüm aşağıdakileri içerir:

* Solidity ile yazılmış :ref:`basit bir akıllı kontrat <simple-smart-contract>`.
* :ref:`Blockzinciri Temelleri <blockchain-basics>`.
* :ref:`Ethereum Sanal Makinesi <the-ethereum-virtual-machine>`.

**2. Solidty'i Tanımak**

Temellere alışıldıktan sonra, programlama dilinin temel konseptlerini anlamak için
:doc:`"Örnekle Solidity" <solidity-by-example>` ve "Dil Tanımı" bölümlerinin okunması tavsiye edilir.

**3. Solidity Derleyicisini Yükleme**

Solidty derleyicisini yüklemek için çeşitli yollar vardır,
tercih ettiğiniz yolu seçin ve :ref:`yükleme sayfasındaki <installing-solidity>`
adımları takip edin.

.. hint::
  Kod örnekleri internet tarayıcınızdan `Remix IDE <https://remix.ethereum.org>`_
  kullanarak denenebilir. Remix internet tarayıcısından erişilebilen bir kod düzenleyicisidir,
  bu düzenleyici ile Solidity'i bilgisayrınıza yüklemeden, Solidity
  akıllı kontratları yazılabilir, dağıtılabilir ve yönetilebilir.

.. warning::
    Yazılımlar insanlar tarafından yazılırlar, bu sebeple hatalar içerebilirler.
    Akıllı kontratlar yazılırken, genel kabul görmüş yazılım geliştirme yöntemleri
    takip edilmelidir. Kod incelemeleri, testler, denetimler ve doğruluk testleri
    buna dahildir. Akıllı kontrat kullanıcıları genelde yazarlarından çok koda
    güvenirler, ve blockzincirleri ve akıllı kontratlar dikkat edilmesi gereken
    kendilerine has problemlere sahiptir, ürün kodu üzerinde çalışmaya başlamadan önce,
    :ref:`security_considerations` bölümünü okuyunuz.

**4. Daha Fazla Bilgi**

Ethereum üzerinde dağıtık uygulama geliştirmeyle ilgili daha fazla bilgi almak için
`Ethereum Geliştirici Kaynakları <https://ethereum.org/en/developers/>`_ genel Ethereum dokümanlarıyla,
geniş eğitici kısımları ve geliştirme araçlarıyla yardımcı olacaktır.

Sorunuz olması durumunda, arama yapabilir, `Ethereum StackExchange <https://ethereum.stackexchange.com/>`_
üzerinde veya `Gitter kanalında <https://gitter.im/ethereum/solidity/>`_ soru sorabilirsiniz.

.. _translations:

Çeviriler
---------

Bu dokümantasyon topluluk katkılarıyla birçok dile çevrilmektedir.
Bunların güncellikleri ve bütünlükleri farklılık gösterebilir. İngilizce sürümü
referans sürüm olarak değerlendirilmelidir.

Sol alt köşedeki menü kullanılarak farklı diller arasında geçiş yapılabilir.

* `Fransızca <https://docs.soliditylang.org/fr/latest/>`_
* `Endonezya Dili <https://github.com/solidity-docs/id-indonesian>`_
* `Farsça <https://github.com/solidity-docs/fa-persian>`_
* `Japonca <https://github.com/solidity-docs/ja-japanese>`_
* `Korece <https://github.com/solidity-docs/ko-korean>`_
* `Çince <https://github.com/solidity-docs/zh-cn-chinese/>`_

.. note::

   Topluluğun çeviri eforunu yönlendirmek için yeni bir GitHub organizasyonu ve çeviri şeması
   oluşturulmuştur. Yeni bir dil için çeviri başlatmak için veya mevcut topluluk dillerine katkıda bulunmakta
   daha fazla bilgi almak için `çeviri rehberi <https://github.com/solidity-docs/translation-guide>`_ incelenebilir.

İçindekiler
===========

:ref:`Dizin <genindex>`, :ref:`Arama Sayfası <search>`

.. toctree::
   :maxdepth: 2
   :caption: Temeller

   introduction-to-smart-contracts.rst
   installing-solidity.rst
   solidity-by-example.rst

.. toctree::
   :maxdepth: 2
   :caption: Dil Tanımı

   layout-of-source-files.rst
   structure-of-a-contract.rst
   types.rst
   units-and-global-variables.rst
   control-structures.rst
   contracts.rst
   assembly.rst
   cheatsheet.rst
   grammar.rst

.. toctree::
   :maxdepth: 2
   :caption: Derleyici

   using-the-compiler.rst
   analysing-compilation-output.rst
   ir-breaking-changes.rst

.. toctree::
   :maxdepth: 2
   :caption: İç Kısımlar

   internals/layout_in_storage.rst
   internals/layout_in_memory.rst
   internals/layout_in_calldata.rst
   internals/variable_cleanup.rst
   internals/source_mappings.rst
   internals/optimizer.rst
   metadata.rst
   abi-spec.rst

.. toctree::
   :maxdepth: 2
   :caption: Ek Materyal

   050-breaking-changes.rst
   060-breaking-changes.rst
   070-breaking-changes.rst
   080-breaking-changes.rst
   natspec-format.rst
   security-considerations.rst
   smtchecker.rst
   resources.rst
   path-resolution.rst
   yul.rst
   style-guide.rst
   common-patterns.rst
   bugs.rst
   contributing.rst
   brand-guide.rst
   language-influences.rst
