## DİNAMİK SAYFALAR OLUŞTURMAK
Öncelikle örnek olarak ürün modelimizi oluşturalım <br>
<img src="img/urunModelNew.PNG"> <br> <br>

Ardından sayfa yönlendirmeleri ile views.py fonskiyoruları oluşturalım <br>
<img src="img/viewsNew.PNG"> <br> <br>

urls.py içerisinde ise sayfa yönlendirmelerini id'ye göre ayarlayalım <br>
<img src="img/urlsPyNew.PNG"> <br> <br>

Son olarakta urun sayfasını ve detay sayfasını oluşturalım <br>
<img src="img/urun.PNG"> <br> <br>
<img src="img/urunDetay.PNG"> <br> <br>

## CKEDITOR KULLANIMI
pip install django-ckeditor komutu ile ckeditoru yüklüyoruz <br> <br>

setting.py içerisinde installed_app içerisine ckeditoru ekliyoruz <br>
<img src="img/ckeditor.PNG"> <br> <br>

Model içerisinde **from ckeditor.fields import RichTextField** komutu ile içeriye aktarıyoruz ve son olarak açıklama yaptırmak istediğimiz alanda **RichTextField()** Kullanıyoruz. <br>
<img src="img/ckModels.PNG"> <br> <br>

Ckeditor çıktısını DOM'a yansıtmak için **autoescape** Kullanılır. <br>
Dikkat edilmesi gereken ise otomatik autospace tamamlamasında kapanışında **end** içeriği atılmaz. <br>
Burada biz kedmiz autospace'in kapanış başına **end** ifadesini ekleyeceğiz
<img src="img/autospace.PNG"> <br> <br>




