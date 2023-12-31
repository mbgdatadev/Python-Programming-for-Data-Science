# Python-Programming-for-Data-Science
## İçindekiler
- [Python Nedir?](#python-nedir)
- [Virtual Environment Nedir?](#virtual-environment-nedir)
- [Package Management Nedir?](#package-management-nedir)
- [Python Data Structures](#python-data-structures) 
- [Python Function Nedir?](#python-function-nedir) 
- [Python Conditions Nedir?](#python-conditions-nedir)
- [Python Loops Nedir?](#python-loops-nedir) 
- [Python Comprehension Nedir?](#python-comprehension-nedir)
- [Numpy Nedir?](#numpy-nedir)
- [Pandas Nedir?](#pandas-nedir)
 
 


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

## Python Data Structures

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


## Python Function Nedir?
Python'da bir fonksiyon, belirli bir görevi yerine getiren ve kodunuzu tekrar kullanılabilir hale getiren bir bloktur. Genellikle belirli bir adı vardır ve parametreler alabilir, bir işlem gerçekleştirir ve isteğe bağlı olarak bir değer döndürebilir.

### Function Ne Zaman Yazılır?
- Belirli bir işlemi tekrar tekrar gerçekleştirmeniz gerektiğinde.
- Kodunuzu parçalara ayırmak ve daha okunabilir hale getirmek istediğinizde.
- Aynı işlemi farklı verilerle uygulamanız gerektiğinde.

### Function Nasıl Yazılır?

```python
def greet(name):
    return f"Merhaba, {name}!"
```

### Function Parametreleri Nedir?
Parametreler: Fonksiyonların aldığı değerlerdir. Yukarıdaki örnekte name, fonksiyonun aldığı tek bir parametredir. Fonksiyonlar birden fazla parametre alabilir.

### Return Nedir?
Return: Fonksiyonun işlemi sonucunda döndürdüğü değerdir. Örneğin, yukarıdaki fonksiyon "Merhaba, {name}!" dizesini döndürür.

### Docstring Nedir?
Docstring: Python'da fonksiyonların veya modüllerin başında yer alan açıklamalardır. Genellikle fonksiyonun ne yaptığını, parametreleri ve dönüş değerini anlatır. Bu açıklamalar kodun daha okunabilir olmasını sağlar.

Örnek Docstring:
```python
def greet(name):
    """Belirtilen isme göre selam döndürür."""
    return f"Merhaba, {name}!"

```

## Python Conditions Nedir?
### Condition Nedir?
Python'da koşullar, programın belirli bir duruma göre farklı işlemler yapmasını sağlar. if, elif, else gibi ifadelerle belirli koşulları kontrol edebiliriz.
```python
# 1. Koşul: if
x = 10
if x > 5:
    print("x, 5'ten büyük")

# 2. Koşul: if-else
y = 3
if y > 5:
    print("y, 5'ten büyük")
else:
    print("y, 5'ten küçük veya eşit")

# 3. Koşul: if-elif-else
z = 7
if z > 10:
    print("z, 10'dan büyük")
elif z == 10:
    print("z, 10'a eşit ")
else:
    print("z, 10'dam küçük ")

```


## Python Loops Nedir?

Python'da döngüler, belirli bir bloğun belirli bir koşul sağlandığı sürece tekrarlanmasını sağlar. Bu, program içinde belirli işlemlerin yinelemeli olarak gerçekleştirilmesini sağlar.

### For Loop
```python
numbers = [1, 2, 3, 4, 5]
for num in numbers:
    print(num)

```

Yukarıdaki örnek, `numbers` adlı bir liste oluşturur. `for` döngüsü bu liste üzerinde her eleman için `num` adlı geçici bir değişken oluşturur ve listenin her elemanını bu değişkene atar. Daha sonra her eleman için belirtilen işlemi gerçekleştirir, burada `print(num)` komutu ile her bir sayıyı ekrana yazdırır.

### While Loop
`while` döngüsü, belirli bir koşul sağlandığı sürece belirtilen işlemi tekrarlar. Koşul doğru olduğu sürece döngü çalışmaya devam eder. Koşul yanlış olduğunda döngü sona erer.

```python
count = 0
while count < 5:
    print(count)
    count += 1
```
Yukarıdaki örnekte `count` adlı bir değişken tanımlanır ve `while` döngüsü bu değişkenin değeri 5'ten küçük olduğu sürece çalışır. Her döngü adımında `count` değeri bir artırılarak ekrana yazdırılır. `count` değeri 5 olduğunda koşul sağlanmaz ve döngü sona erer.

### Python `enumerate` Fonksiyonu

`enumerate`, bir dizi veya başka bir yinelenebilir nesne üzerinde döngü oluştururken hem elemanların değerlerine hem de indislerine erişmemizi sağlayan bir Python işlevidir.

Örneğin:

```python
liste = ['a', 'b', 'c', 'd']

for index, value in enumerate(liste):
    print(f"Index: {index}, Value: {value}")
```

### Python'da `continue` ve `break`

- **`continue`**: Bir döngü içinde kullanıldığında, döngü herhangi bir sebepten dolayı beklenmedik bir şekilde sonlanmadığı sürece, döngünün o anda bulunduğu adımı atlar ve döngüyü devam ettirir. Yani, `continue` ifadesi çalıştığında döngü bloğundaki geri kalan kısmı görmezden gelir ve bir sonraki döngü adımına geçer.

Örnek:

```python
for i in range(5):
    if i == 2:
        continue
    print(i)

output:
0
1
3
4

```

- **`break`**  Bir döngü içinde kullanıldığında, belirli bir koşul gerçekleştiğinde döngüyü tamamen sonlandırır. Yani, `break` ifadesi çalıştığında döngü derhal sona erer ve döngü bloğunun dışındaki kod satırlarına geçilir.

```python
for i in range(5):
    if i == 3:
        break
    print(i)


output:
0
1
2

```
### Python'da Kullanılan Bazı Fonksiyonlar ve İfadeler

#### `zip()`
- `zip()`, birden fazla iterable'ı (liste, tuple vb.) eşleştirerek birleştiren ve her bir iterable'dan sırayla elemanları alarak tuple'lar oluşturan bir Python işlevidir.
- Örneğin:

```python
liste1 = [1, 2, 3]
liste2 = ['a', 'b', 'c']

for eleman in zip(liste1, liste2):
    print(eleman)

outpu:
(1, 'a')
(2, 'b')
(3, 'c')
```

`lambda`, anonim (isimsiz) bir fonksiyon oluşturmak için kullanılan bir ifadedir. Genellikle tek satırda basit fonksiyonlar tanımlamak için kullanılır.

```python
carpma = lambda x, y: x * y
print(carpma(5, 3))  # Bu kod 15 çıktısını verecektir.

```

`map()`, bir fonksiyonu belirli bir iterable'ın her elemanına uygulayarak yeni bir iterable döndüren bir Python işlevidir.

```python
liste = [1, 2, 3, 4]
kareler = map(lambda x: x ** 2, liste)
print(list(kareler))  # Bu kod [1, 4, 9, 16] çıktısını verecektir.

```

`filter()`, bir fonksiyonu belirli bir iterable'ın her elemanına uygulayarak, fonksiyonun doğruladığı elemanlardan oluşan bir iterable döndüren bir Python işlevidir

```python
liste = [1, 2, 3, 4, 5, 6]
cift_sayilar = filter(lambda x: x % 2 == 0, liste)
print(list(cift_sayilar))  # Bu kod [2, 4, 6] çıktısını verecektir.
```

`reduce()`, bir fonksiyonu belirli bir iterable'ın elemanlarına sırayla uygulayarak tek bir sonuç üreten bir Python işlevidir. Python 3'ten itibaren functools modülünde bulunur.

```python
from functools import reduce

liste = [1, 2, 3, 4]
toplam = reduce(lambda x, y: x + y, liste)
print(toplam)  # Bu kod 10 çıktısını verecektir.
```


## Python Comprehension Nedir?
Python programlama dilinde daha kısa, daha okunaklı ve daha hızlı kod yazmayı sağlayan bir yapıdır. List Comprehension, Dictionary Comprehension, Set Comprehension ve Generator Comprehension gibi çeşitleri bulunur.

### List Comprehension (Liste Oluşturma): 
Bir liste üzerinde döngü oluşturarak yeni bir liste oluşturma yöntemidir. Özellikle mevcut bir liste veya başka bir iterable'dan yeni bir liste oluşturmak için kullanılır.

```python
liste = [1, 2, 3, 4, 5]
kareler = [x ** 2 for x in liste]
# kareler şimdi [1, 4, 9, 16, 25] değerlerine sahip bir liste olmuştur
```

### Dictionary Comprehension (Sözlük Oluşturma): 
Bir sözlük üzerinde döngü oluşturarak yeni bir sözlük oluşturma yöntemidir. Sözlükteki her bir anahtar ve değer için belirli bir koşula göre yeni bir sözlük oluşturmak için kullanılır.

```python
sozluk = {'a': 1, 'b': 2, 'c': 3}
yeni_sozluk = {anahtar: deger * 2 for anahtar, deger in sozluk.items()}
# yeni_sozluk şimdi {'a': 2, 'b': 4, 'c': 6} değerlerine sahip bir sözlük olmuştur

```
### Set Comprehension (Küme Oluşturma): 
Bir küme üzerinde döngü oluşturarak yeni bir küme oluşturma yöntemidir. Benzer şekilde mevcut bir küme veya başka bir iterable'dan yeni bir küme oluşturmak için kullanılır.

```python
kume = {1, 2, 3, 4, 5}
tekler = {x for x in kume if x % 2 != 0}
# tekler şimdi {1, 3, 5} değerlerine sahip bir küme olmuştur
```
### Generator Comprehension (Generator Oluşturma): 
Bir generator (üreteç) oluşturmak için kullanılan yapıdır. Liste veya sözlük gibi veri yapısını tam olarak bellekte oluşturmadan, ihtiyaç duyulduğunda elemanları üreten bir yapıdır.

```python
generator = (x ** 2 for x in range(5))
# Bu, bir generator nesnesi oluşturur ve elemanları gerektiğinde üretir
```
## NumPy Nedir?

NumPy, Python programlama dilinin bilimsel hesaplamalar, veri manipülasyonu ve analizi için kullanılan temel bir kütüphanesidir. "Numerical Python" ifadesinden türetilmiştir.

#### Temel Özellikler:

1. **Nesne Dizileri (ndarray)**: NumPy'nin temel veri yapısı olan ndarray (N-dimensional Array), aynı türden verileri depolamak için optimize edilmiş çok boyutlu dizilerdir. Bu çok boyutlu diziler, 1D, 2D, 3D ve daha fazla boyutta veri depolamak için kullanılabilir.

2. **Hızlı Matematiksel İşlemler**: Vektörel ve matris işlemleri gibi matematiksel işlemler hızlı bir şekilde gerçekleştirilir. NumPy, altında C dilinde yazılmış optimize edilmiş altyapıları kullanır, bu da işlemlerin Python listelerine göre daha hızlı olmasını sağlar.

3. **Broadcasting**: NumPy, farklı şekillerdeki diziler üzerinde matematiksel işlemler yaparken otomatik olarak yayma (broadcasting) özelliği sunar. Bu, farklı boyutlardaki dizileri birbirleriyle işlem yapılabilir hale getirir.

4. **Rastgele Sayı Üretimi**: NumPy, rastgele sayılar üretmek için fonksiyonlar içerir. Bu, simülasyonlar, istatistiksel analizler ve diğer birçok algoritma için önemlidir.

NumPy, bilimsel hesaplamalar, veri analizi, makine öğrenimi gibi birçok alanda yaygın olarak kullanılan bir kütüphanedir. Ayrıca, diğer Python kütüphaneleriyle (örneğin, Pandas, Matplotlib, SciPy) uyumlu olarak çalışarak veri analizi ve bilimsel hesaplamalar için temel bir bileşen olarak kullanılır.

### Reshaping (Yeniden Şekillendirme)
NumPy'de `reshape()` fonksiyonu, mevcut bir ndarray'in şeklini değiştirmek için kullanılır. Bu işlem, veriyi aynı veri miktarında fakat farklı bir şekilde düzenlemek için kullanılır. Yani, verinin boyutları değiştirilebilir ancak içerdiği toplam veri miktarı değişmez.

```python
import numpy as np

# 1'den 9'a kadar olan sayıları içeren bir ndarray oluşturma
array = np.arange(1, 10)

# Yeniden şekillendirme işlemi ile 3x3'lük bir matris oluşturma
reshaped_array = array.reshape(3, 3)
```

### Index İşlemleri
NumPy'de dizilerdeki belirli elemanlara erişmek için indeksler kullanılır. Bu indeksler, tek bir elemana erişmek veya bir dilim (slice) almak için kullanılabilir.

```python
import numpy as np

array = np.array([1, 2, 3, 4, 5])

# İndeks kullanarak belirli bir elemana erişme
print(array[2])  # Bu kod, 3 çıktısını verecektir

# Dilimleme (slicing) kullanarak belirli bir aralığı alma
print(array[1:4])  # Bu kod, [2, 3, 4] çıktısını verecektir
```


### Fancy Index
Fancy Indexing, NumPy'de daha karmaşık indeksleme yöntemlerini ifade eder. Bu yöntem, normal bir indeks dizisi kullanarak veya bir koşul ifadesiyle belirli elemanlara erişmek için kullanılır.

```python
import numpy as np

array = np.array([1, 2, 3, 4, 5])

# Fancy Indexing kullanarak belirli elemanlara erişme
indices = [0, 2, 4]
print(array[indices])  # Bu kod, [1, 3, 5] çıktısını verecektir

# Koşul ifadesiyle belirli elemanlara erişme
print(array[array > 2])  # Bu kod, [3, 4, 5] çıktısını verecektir
```

## Pandas Nedir?

Pandas, Python programlama dilinde veri manipülasyonu ve veri analizi için kullanılan güçlü bir kütüphanedir. Yüksek performanslı, kolay kullanımlı veri yapıları ve veri analizi araçları sunar.

#### Temel Özellikler:

1. **DataFrame ve Series**: Pandas'ın temel veri yapıları, DataFrame ve Series'dir. DataFrame, satır ve sütunlardan oluşan tablo benzeri bir veri yapısıdır. Series ise tek boyutlu etiketlenmiş bir dizidir.

2. **Veri Okuma ve Yazma**: Pandas, çeşitli dosya formatlarındaki verileri okuma (csv, excel, json, sql, vb.) ve yazma işlemleri için işlevler sunar.

3. **Veri Manipülasyonu**: Veri içinde filtreleme, birleştirme, gruplama, eksik verilerle çalışma, veri dönüştürme gibi işlemler kolaylıkla yapılabilir.

4. **Zaman Serileri Analizi**: Pandas, zaman serileri verileri üzerinde analiz yapmak için özel araçlar içerir.

5. **Hızlı ve Verimli**: Veri yapıları, altında Numpy'ın hızlı matematiksel işlemlerini kullandığı için büyük veri kümeleri üzerinde etkili çalışma sağlar.

Pandas, veri temizleme, veri hazırlama, veri görselleştirme ve veri analizi gibi birçok alanda yaygın olarak kullanılmaktadır. Özellikle, veri bilimi ve makine öğrenimi gibi alanlarda veri işleme süreçlerinin önemli bir parçasıdır.

### Pandas Series
Pandas Series, tek boyutlu etiketli bir dizidir. Her bir eleman, belirli bir indeksle tanımlanır. Series'ler, farklı veri tiplerinde verileri içinde barındırabilirler.

### Pandas Seçim İşlemleri, loc, iloc
Pandas'da veri seçimi yapmak için `loc` ve `iloc` indeksleme yöntemleri kullanılır. `loc` indeksleme, etiket bazlı indeksleme yaparken `iloc`, konum bazlı (sıra numarası) indeksleme yapar.

### Toplulaştırma (Aggregation) ve Gruplama (Grouping)
Pandas, veri toplulaştırma ve gruplama işlemlerini yapmak için kullanılır. Veri toplulaştırma, bir veri kümesini özetleyerek istatistiksel bilgiler elde etmeyi sağlar. Gruplama ise belirli bir kritere göre veriyi gruplayarak işlem yapmayı kolaylaştırır.

### Pivot Table
Pivot table, verileri bir DataFrame'de çapraz tablo şeklinde düzenlemek ve özetlemek için kullanılan bir işlevdir. Bu, verileri bir veya daha fazla anahtarla gruplayarak çok boyutlu bir şekilde analiz etmeyi sağlar.

### Apply & Lambda
Pandas'ta apply() fonksiyonu, DataFrame veya Series üzerinde belirli bir işlevi veya lambda fonksiyonunu her bir elemana uygulamak için kullanılır. lambda ise Python'da anonim (isimsiz) fonksiyonlar oluşturmayı sağlar.


















