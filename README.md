JSON Dosyasını CSV Dosyasına Dönüştürme

Bu C programı, bir JSON dosyasındaki verileri bir CSV dosyasına dönüştürür. Program, bir JSON dosyasını girdi olarak alır,
ilgili bilgileri çıkarır ve verileri bir CSV dosyasına yazar. CSV dosyasına başlık satırı eklemek isteğe bağlıdır.

Kullanım
Genel kullanım:
./json_to_csv <JSON_dosya_adı> <CSV_dosya_adı> <header=ON|OFF>
<JSON_dosya_adı>: Girdi olarak kullanılacak JSON dosyasının adı.
<CSV_dosya_adı>: Çıktı olarak oluşturulacak CSV dosyasının adı.
<header=ON|OFF>: CSV dosyasında başlık satırını dahil etmek için "ON", dahil etmemek için "OFF" kullanılır.

Bu kod için terminalden şu komut girilerek çalıştırılabilir:
.\deneme test.json output.csv ON

Derleme
Programı derlemek için gcc gibi bir C derleyici kullanılmalıdır:
gcc json_to_csv.c -o json_to_csv

Program, belirli bir "id," "name," "midterm," "final," ve "course" gibi alanlara sahip bir JSON formatını varsayar. JSON yapınız farklı ise kodu buna göre ayarlayın.

İşlenen öğrenci sayısı maksimum olarak 50 olarak ayarlanmıştır. İhtiyaca göre Student dizisinin boyutunu değiştirebilirsiniz.

Programı çalıştırırken doğru sayıda komut satırı argümanını sağladığınızdan emin olun.


