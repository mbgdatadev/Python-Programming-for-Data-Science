# Python-Programming-for-Data-Science
## İçindekiler
- [Python Nedir?](#python-nedir)
- [Virtual Environment Nedir?](#virtual-environment-nedir)
- [Package Management Nedir?](#package-management-nedir)
- [Python Veri Tipleri ve Veri Yapıları](#python-veri-tipleri-ve-veri-yapilari)


## Python Nedir?

Python, kullanımı kolay ve güçlü bir programlama dilidir. Genellikle okunabilir ve anlaşılabilir sözdizimiyle bilinir. Çeşitli alanlarda kullanılan, geniş bir kütüphane ve araç yelpazesi sunan yüksek seviyeli bir dil olarak öne çıkar.Python, bir betik dilidir ve kodu yürütmek için yorumlayıcı kullanır. Dolayısıyla, kodun çalıştırılması sırasında herhangi bir derleme aşaması yoktur; kod satır satır yorumlanır ve anında çalıştırılır.Python'da satır sonlarına ihtiyaç duyulmaz. Normalde, kodun her yeni mantıksal yapısını belirtmek için girintilere dayalı bir yapı kullanılır. 

### Özellikleri

- **Kolay Okunabilirlik:** Basit ve temiz bir sözdizimine sahiptir, bu da kodların anlaşılmasını kolaylaştırır.
- **Geniş Kütüphane Desteği:** Zengin standart kütüphaneleri ve üçüncü taraf modülleriyle işleri hızlandırır.
- **Taşınabilirlik:** Farklı platformlarda (Windows, macOS, Linux) çalışabilir.
- **Çeşitli Kullanım Alanları:** Web geliştirme, veri analizi, yapay zeka, bilimsel hesaplama ve daha birçok alanda kullanılır.

### Örnek Kod

```python
# Merhaba Dünya
print("Merhaba, Dünya!")
```

## Virtual Environment Nedir?
Sanal ortam (Virtual Environment), bir Python projesinin bağımlılıklarını izole etmek ve yönetmek için kullanılan bir araçtır. Projenizin farklı versiyonları için farklı kütüphane versiyonları veya modüller gerekebilir. Sanal ortamlar, bu durumda projenizi belirli bir Python sürümü ve kütüphane seti ile sınırlamanıza yardımcı olur. Yaygın olarak kullanılan sanal ortamlar `venv` `virtualenv` `pipenv` `conda`

### Neden Sanal Ortam Kullanılır ?

- **Bağımlılıkları İzole Eder:** Her proje kendi sanal ortamını oluşturabilir ve bağımlılıkları izole edebilir. Bu, farklı projelerde farklı kütüphane versiyonlarını kullanmanızı sağlar.
- **Temiz ve Kontrollü Çalışma Alanı:** Sanal ortamlar, proje bağımlılıklarının kurulumunu, güncellemesini ve kaldırılmasını izole bir şekilde yapmanızı sağlar.
- **Taşınabilirlik:** Sanal ortam, projeyle birlikte taşınabilir olduğundan farklı sistemlerde aynı bağımlılıkları kullanabilirsiniz. 

### Sanal Ortam Nasıl Oluşturulur ?

Sanal ortam oluşturmak için terminale şu komutu kullanabilirsiniz:

```bash
# Python 3 ile sanal ortam oluşturma
python3 -m venv myenv
```
`myenv` yerine kullanmak istediğiniz ismi verebilirsiniz. Daha sonra oluşturulan sanal ortamı etkinleştirmek için:

#### Windows
```
myenv\Scripts\activate
```

#### Unix veya MacOS:
```
source myenv/bin/activate
```

## Package Management Nedir?

Paket yönetimi (Package Management), bir programlama dilinde veya bir sistemde kullanılan paketlerin (kütüphaneler, modüller veya yazılım bileşenleri) yönetimini ve dağıtımını içeren süreçtir. Bu paketler genellikle kodun farklı parçalarını veya belirli işlevleri gerçekleştiren hazır yazılım bileşenleridir.

### Paket Yönetiminin Önemi

- **Bağımlılıkları Yönetme:** Projeler genellikle birden çok pakete veya kütüphaneye ihtiyaç duyar. Paket yöneticileri, bu bağımlılıkları kolayca yönetmenizi sağlar.
- **Sürüm Kontrolü:** Belirli sürümlere veya paket versiyonlarına ihtiyaç duyulabilir. Paket yönetimi, belirli sürümleri belirtme ve yönetme konusunda yardımcı olur.
- **Güncelleme ve Yükleme Kolaylığı:** Paket yöneticileri, paketleri kolayca güncelleme, kaldırma veya yükleme imkanı sunar.
- **Proje İzolasyonu:** Sanal ortamlar gibi araçlarla projelerin bağımlılıkları izole edilebilir, böylece her proje kendi bağımlılıklarını yönetir.

### Paket Yöneticileri

Pek çok programlama dilinin kendi paket yöneticileri bulunur:
- Python için **pip**, **pipenv**, **conda**
- C# için **Nuget**
- JavaScript için **npm** (Node Package Manager),
- Ruby için **gem**,
- Java için **Maven** veya **Gradle**,
- ve daha birçok dillerin kendi paket yöneticileri vardır.

Paket yöneticileri, genellikle depolardan (repository) paketleri arar, indirir, yükler, günceller ve kaldırır. Bu şekilde, geliştirme sürecinde ihtiyaç duyulan paketleri kolayca elde edebilirsiniz.

Paket yönetimi, yazılım geliştirme sürecinde önemli bir rol oynar ve projelerde kullanılan paketlerin etkin bir şekilde yönetilmesini sağlar.

## Python Veri Tipleri ve Veri Yapıları

### Sayılar (Numbers)

- **int:** Tam sayıları temsil eder. Örneğin: `5`, `-10`.
- **float:** Ondalık sayıları temsil eder. Örneğin: `3.14`, `2.71828`.
- **complex:** Karmaşık sayıları temsil eder. Örneğin: `3+4j` (gerçek ve sanal kısım).

### Karakter Dizileri (Strings)

- **str:** Metin veya karakter dizilerini temsil eder. Örneğin: `'Merhaba'`, `"Python"`.

### Boolean (TRUE-FALSE)

- **bool:** Mantıksal değerleri temsil eder. `True` veya `False` olarak ifade edilir.

### Liste (List)

- **Liste:** Sıralı ve değiştirilebilir öğelerin bir koleksiyonunu temsil eder. Örneğin: `[1, 2, 3, 'a', 'b']`.

### Sözlük (Dictionary)

- **Sözlük:** Anahtar-değer çiftlerinin koleksiyonunu temsil eder. Örneğin: `{'anahtar1': 'değer1', 'anahtar2': 'değer2'}`.

### Demet (Tuple)

- **Demet:** Değiştirilemeyen öğelerin bir koleksiyonunu temsil eder. Örneğin: `(1, 2, 'a', 'b')`.

### Set

- **Küme:** Benzersiz öğelerin bir koleksiyonunu temsil eder. Örneğin: `{1, 2, 3, 4}`.





