# epik-s-per-m-per-harika-tesi-hesap-makinesi-hem-de-tasar-ml-
hesaplıyor 

# Epik Süper Müper Harika Ötesi Hesap Makinesi Hem de Tasarımlı

Bu proje, sıradan bir hesap makinesi deneyimini bambaşka bir boyuta taşıyarak kullanıcılarına yepyeni, akıllara durgunluk veren ve görsel açıdan da özenle tasarlanmış bir arayüz sunmayı amaçlamaktadır. Projemiz, her detayıyla “epik”, “süper”, “müper”, “harika” ve “ötesi” niteliklerini bünyesinde barındırırken; kullanıcı deneyimini en üst seviyeye çıkarmak, kullanım kolaylığı sağlamak ve modern web teknolojileriyle desteklenen dinamik işlevselliği sunmak üzere geliştirildi.

---

## İçerik ve Genel Bakış

Bu projede, HTML, CSS ve JavaScript kullanılarak geliştirilmiş olan hesap makinesi, temel aritmetik işlemleri (toplama, çıkarma, çarpma, bölme) gerçekleştirmek üzere tasarlanmıştır. Kullanıcılar, iki adet sayısal giriş alanına değer girip, üzerlerine tıklayarak ilgili matematiksel işlemi gerçekleştirebilirler. Her işlem sonucu, sayfa içerisinde anlık olarak güncellenen ve göz alıcı şekilde sunulan bir sonuç kutusunda görüntülenir. Proje sadece fonksiyonelliği ile değil, aynı zamanda modern, temiz ve akıllıca düzenlenmiş arayüz tasarımı ile de öne çıkmaktadır.

---

## Kullanılan Teknolojiler

- **HTML5:** Sayfanın temel yapısını oluşturmak, içerikleri semantik bir şekilde düzenlemek ve erişilebilirlik açısından avantaj sağlamak için kullanılmıştır.
- **CSS:** Sayfanın stil ve tasarımını yönetmek, modern ve çekici bir kullanıcı arayüzü sunmak amacıyla dış bir stil dosyası (`css.css`) aracılığıyla uygulanmıştır.
- **JavaScript:** Dinamik işlemleri gerçekleştirmek ve kullanıcı etkileşimlerine anında yanıt vermek için temel hesaplama fonksiyonları (topla, cıkar, carp, bol) ile birlikte kodun işlevselliğini artırmaktadır.

---

## Proje Yapısı ve Kod İncelemesi

### HTML & Temel Yapı

Proje, modern web standartlarına uygun olarak hazırlanmıştır. Aşağıdaki HTML kodu, hesap makinesinin temel yapısını ortaya koymaktadır:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Panne bir şeyler denemekte</title>
    <link rel="stylesheet" href="css.css">
</head>
<body>
<div class="container">
    <div class="inputs">
        <input type="number" id="input1">
        <input type="number" id="input2">
    </div>
    <div class="buttons">
        <button onclick="topla()">Topla</button>
        <button onclick="cıkar()">Çıkar</button>
        <button onclick="carp()">Çarp</button>
        <button onclick="bol()">Böl</button>
        <div class="cevap">
            <div id="sonuc"></div>
        </div>
    </div>
</div>

<div class="reklam">
    <p>hello world</p>
    <a href="https://www.rightwho.com">allah site</a> <br>
    <a href="https://www.whus.xyz">Allah siteyi yapanlar</a>
</div>

<script>
function topla() {
    var input1 = document.getElementById("input1").value;
    var input2 = document.getElementById("input2").value;
    var sum = Number(input1) + Number(input2);
    document.getElementById("sonuc").innerHTML = `Toplama işlemi sonucu : ${sum}`;
}

function cıkar() {
    var input1 = document.getElementById("input1").value;
    var input2 = document.getElementById("input2").value;
    var sum = Number(input1) - Number(input2);
    document.getElementById("sonuc").innerHTML = `Çıkarma işlemi sonucu : ${sum}`;
}

function carp() {
    var input1 = document.getElementById("input1").value;
    var input2 = document.getElementById("input2").value;
    var sum = Number(input1) * Number(input2);
    document.getElementById("sonuc").innerHTML = `Çarpma işlemi sonucu : ${sum}`;
}

function bol() {
    var input1 = document.getElementById("input1").value;
    var input2 = document.getElementById("input2").value;
    var sum = Number(input1) / Number(input2);
    document.getElementById("sonuc").innerHTML = `Bölme işlemi sonucu : ${sum}`;
}
</script>
</body>
</html>
