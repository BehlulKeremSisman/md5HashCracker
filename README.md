MD5 HASH CRACKER

Kullanılabilecek örnek komutlar ve açıklamalar aşağıdadır.

----------------------------------------------------------------------------------------------------------------------------

1)	./md5HashCracker.ps1 -help h

Kullanıcı programın çalışması ile ilgili bilgi almak için –help h parametresini kullanabilir. 
Bu komuta yanıt olarak diğer parametreler ile ilgili bilgiler ve kullanım örnekleri hakkında 
bilgi verilir. 

----------------------------------------------------------------------------------------------------------------------------

Burada kullanıcıya kullanım tarzına göre 2 seçenek sunuldu. Eğer kullanıcı tek 1 hash değerini 
cracklemek istiyorsa –crackType için ‘single’ parametresini kullanır. Eğer okuyacağı hash değeri
1 den fazla ise bu değerleri bir text dosyasına yazar, bu dosyanın pathini programa verir ve 
karşılığında dosyadaki tüm hashler için birer yanıt alır. Bunun için –crackType parametresine 
‘plural’ vermeli. Raporun devamında bu kullanım örneklerini ve detaylı açıklamaları bulacaksınız.

a) ./md5HashCracker.ps1 -crackType single -Wordlist <wordlistpath>

Cracklenmek istenen hash 1 tane ise –crackType parametresi için ‘single’ kullanılabilir. 

Cracklenmek istenen hash değeri input olarak girilir. Girilen md5 hash değeri 32 karakterli olacağı 
için, 32 karakter olarak girilmeyen bir input değeri için “ERROR ! Hash değeri yanlış girdiniz. Lutfen 
32 karakterli hash değeri girin.” şeklinde bir hata mesajı verilir.

–Wordlist parametresine pathi verilen sözlük dosyasındaki her satırdaki elemanın hash alınarak, inputa 
verilen hash ile kıyaslanır. İnputtaki hash değerine karşılık gelen bir hash değeri bulunursa o elemanı 
cevap olarak ekrana verir. Eğer karşılık gelen hashi bulamazsa “Hash olarak girilen ‘<hash>’ için md5 
crack yapılamadı” şeklinde bir bilgi mesajı verilir. 

----------------------------------------------------------------------------------------------------------------------------

b) ./md5HashCracker.ps1 -crackType plural -Wordlist <wordlistpath>

Cracklenmek istenen hash sayısı 1’den fazla ise –crackType parametresi için ‘plural’ kullanılabilir. 

Cracklenmek istenen hash değerleri bir text dosyasına aktarılır. Kullanıcı bu text dosyasının pathini 
programı çalıştırdıktan sonra girer. Girilen dosyadan tüm hashler sırasıyla alınır.Her bir hash değeri 
32 karakterli olacağı için, 32 karakter olmayan bir hash değeri için “ERROR ! Hash değeri yanlış girdiniz. 
Lutfen 32 karakterli hash değeri girin.” şeklinde bir hata mesajı verilir.

Hash listesinde sırayla okunan hashler –Wordlist parametresine pathi verilen sözlük dosyasındaki her satırdaki 
elemanın sırayla hashi alınarak, her bir hash ile kıyaslanır. İnputtaki hash değerine karşılık gelen bir hash 
değeri bulunursa o elemanı cevap olarak ekrana verir. Eğer karşılık gelen hashi bulamazsa “Hash olarak girilen 
‘<hash>’ için md5 crack yapılamadı” şeklinde bir bilgi mesajı verilir. 

Örnek bir kullanım ve ekran çıktıları aşağıda verilmiştir.

 
