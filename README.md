# Python-Programming-for-Data-Science
## İçindekiler
- [Python Nedir?](#python-nedir)
- [Virtual Environment Nedir?](#virtual-environment-nedir)
- [Package Management Nedir?](#package-management-nedir)
- [Python Data Structures](#python-data-structures) 
- [Python Function Nedir?](#python-function-nedir) 
- [Python Conditions Nedir?](#python-conditions-nedir)
- [Python Loops Nedir?](#python-loops-nedir) 
- [Python enumerate Fonksiyonu](#python-enumerate-fonksiyonu)
 


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

## Python enumerate Fonksiyonu

`enumerate`, bir dizi veya başka bir yinelenebilir nesne üzerinde döngü oluştururken hem elemanların değerlerine hem de indislerine erişmemizi sağlayan bir Python işlevidir.

Örneğin:

```python
liste = ['a', 'b', 'c', 'd']

for index, value in enumerate(liste):
    print(f"Index: {index}, Value: {value}")```








