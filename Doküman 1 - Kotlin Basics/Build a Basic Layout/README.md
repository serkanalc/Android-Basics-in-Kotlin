# Kotlin Basics

- [Kotlin'deki İlk Programınızı Çalıştırın](#1)
- [Programı Değiştirin](#2)
- [Programı Genişletin](#3)

- [Çözüm Kodu](https://github.com/serkanalc/Android-Basics-in-Kotlin/blob/main/Dok%C3%BCman%201%20-%20Kotlin%20Basics/Build%20a%20Basic%20Layout/%C3%87%C3%B6z%C3%BCm%20Kodu/Hello%20World.kt)

## <a name="1"></a>Kotlin'deki İlk Programınızı Çalıştırın

Bu aşamada, hemen Kotlin dilinde programlamaya başlamak için bir web sitesinde bir düzenleyici kullanacaksınız.

### Etkileşimli Bir Kod Düzenleyici Kullanın

Bilgisayarınıza yazılım yüklemek yerine, ilk programınızı oluşturmak için web tabanlı bir araç kullanabilirsiniz.

1. Tarayıcınızda [bu linkten](https://developer.android.com/training/kotlinplayground) açın . Bu, tarayıcı tabanlı bir programlama aracı açar.
2. Ortada bir kod düzenleyici ile aşağıdaki ekran görüntüsüne benzer bir sayfa görmelisiniz.

![image](https://user-images.githubusercontent.com/70329389/145654875-8ca52bda-96e7-4167-9d0d-49c9dde665bd.png)

Bu, editördeki program kodudur:

```
fun main() {
    println("Hello, world!")
}
```

### Program Kodunu Çalıştırın

Oluşturduğunuz bir programı çalıştırmak, bilgisayarınızda kelime işlemci gibi bir programı çalıştırmaktan çok farklı değildir. Aradaki fark, bir görevi gerçekleştirmek için bir programı çalıştırdığınızda veya bir oyun oynadığınızda, öncelikle programın sizin için neler yapabileceğini önemsersiniz ve onu çalıştıran kodla ilgilenmezsiniz. Programlarken, sihrin gerçekleşmesini sağlayan gerçek kodu görebilir ve onunla çalışabilirsiniz.

Bakalım bu program ne yapacak!

1. Düzenleyicide, sağ üst köşedeki beyaz veya yeşil üçgeni bulun ve programı çalıştırmak için tıklayın.
2. Alttaki bölmeye bakın.

```
Hello, world!
```

Dikkat `Hello World!` yukarıdaki resimdeki gibi ekrana basılmıştır. Artık bu programın ne yaptığını biliyorsunuz: Bir hello world mesajı yazdırıyor veya çıktı veriyor.

*Derleme , Kotlin program kodunu sistemin çalıştırabileceği bir forma çeviren bir işlemdir. Derleme başarıyla tamamlanırsa, programda çalışmasını engelleyecek hiçbir hata yoktur. Sorunlar varsa, bunlar alttaki bölmede görünecektir.*

## <a name="2"></a>Programı Değiştirin

### "Hello World" Kodunu değiştirin

Programı biraz farklı bir şey yapacak şekilde değiştirelim.

1. "Hello World" metnini "Doğum Günün Kutlu olsun!" metni ile değiştirin
2. Sağ üstteki mavi veya yeşil çalıştır düğmesine tıklayarak programınızı çalıştırın.
3. Altta `Doğum Günün Kutlu Olsun!`aşağıda gösterildiği gibi yazdırıldığını görmelisiniz.

```
Doğum Günün Kutlu Olsun!
```
### Nasıl Çalışır?

Bu nasıl yapılır? Bu sadece bir şey yazdırmak için çok fazla kod gibi görünüyor!

Bir arkadaşınızın belirli bir kağıt parçasına "Hello World!" yazmasını istiyorsanız. Bunu yapması için birçok aşama var. Ona sadece "Hello World!" yaz derseniz bu kağıt parçası üzerinde, belirtmediğiniz bilgiler hakkında varsayımlarda bulunacaklar. Örneğin, bir kalem kullanmaları gerektiğini ve sizin onu harflerle yazmalarını istediğinizi varsayacaklardır! Bilgisayar bu varsayımları yapmaz, bu nedenle her adımı içeren kesin talimatlar vermeniz gerekir.

Tıpkı İngilizcenin bir yapısı olduğu gibi, bir programlama dili de öyle. Başka bir dil öğrendiyseniz, dilbilgisini, imlayı, belki de yeni bir sembol alfabesini ve kelimeleri öğrenmenin zorluğunu bilirsiniz. Programlamayı öğrenmenin benzer zorlukları vardır, ancak neyse ki, örneğin İngilizce gibi öğrenmekten daha az karmaşık ve çok daha mantıklıdır.

### Programın Bölümlerini Anlayın

Şimdi koda bir göz atın. Bu programın her parçası belirli bir amaca hizmet eder ve programı çalıştırabilmek için tüm parçalara ihtiyacınız vardır. İlk kelimeyle başlayalım.

- `fun` Kotlin programlama dilinde bir kelimedir. `fun` function anlamına gelir. function, belirli bir görevi gerçekleştiren programın bir bölümüdür

> Not: Kotlin'in çok özel anlamları olan birçok özel kelimesi vardır. Kotlin dilinde programlamayı öğrendikçe bu kelimeleri de öğreneceksiniz. Bunlara genellikle keywords veya reserved words denir.

- `main` bu function'un adıdır. Fonksiyonların isimleri vardır, bu yüzden birbirlerinden ayırt edilebilirler. Bu function, `main` programı çalıştırdığınızda çağrılan ilk veya ana işlev olduğu için çağrılır. Her Kotlin programının main fonksiyonuna ihtiyacı vardır.

- İşlev adının ardından her zaman `()` iki parantez gelir.
- Parantezlerin içine, fonksiyonun kullanması için bilgi girebilirsiniz. Fonksiyona yapılan bu girdiye "arguments" veya kısaca `args` denir . Argümanlar hakkında daha sonra daha fazlasını öğreneceksiniz.
- Parantezlerden sonraki `{}` küme parantezlerine  dikkat edin . Bir foksiyonun içinde bir görevi yerine getiren kod bulunur. Bu küme parantezleri bu kod satırlarını çevreler.

Küme parantezler arasındaki kod satırına bakın:

```
println("Doğum Günün Kutlu Olsun!")
```
Bu kod satırı Doğum Günün Kutlu Olsun! metni yazdırır.

- `println` sisteme bir metin satırı yazdırmasını söyler.
- Parantezlerin içine, yazdırılacak metni koyarsınız.
- Yazdırılacak metnin tırnak içine alındığına dikkat edin. Bu, sisteme tırnak işaretleri içindeki her şeyin tam olarak verildiği gibi yazdırılması gerektiğini söyler.

Metni gerçekten yazdırmak için, tüm bu `println` talimatın `main` fonksiyonunun içinde olması gerekir.

İşte burada. En temel Kotlin programı.

```
fun main() {
    println("Happy Birthday!")
}
```

## <a name="3"></a>Programı Genişletin

### Birden Fazla Mesaj Yazdır

`println()` fonksiyonunu kullanarak bir satır metin yazdırdınız. Bununla birlikte, bir fonksiyonun içine istediğiniz veya bir görevi tamamlamak için ihtiyaç duyduğunuz kadar talimat satırı koyabilirsiniz.

1. println("Happy Birthday!") satırını kopyalayın ve altına iki kez daha yapıştırın. Yapıştırdığınız satırların main foksiyonunun küme parantezleri içinde olduğundan emin olun.
2. Birinin adına yazdırılacak bir metn ile değiştirin, "Serkan" deyin.
3. Yazdırılacak diğer metni "23 yaşına bastın!" olarak değiştirin.

Kodunuz aşağıdaki kod gibi görünmelidir.

```
fun main() {
    println("Doğum Günün Kutlu Olsun!")
    println("Serkan")
    println("23 yaşına bastın!")
}
```
Bu kodun çalıştığında ne yapmasını beklersiniz?

4. Ne yaptığını görmek için programınızı çalıştırın.
5. Çıktı bölmesine gidin ve aşağıda gösterildiği gibi konsol penceresinde yazdırılan 3 satır görmelisiniz.

```
Doğum Günün Kutlu Olsun!
Serkan
23 yaşına bastın!
```

### Hatalarla Başa Çıkmak

Programlama sırasında hata yapmak normaldir ve çoğu araç, hataları düzeltmenize yardımcı olmak için size geri bildirimde bulunur. Bu adımda, ne olduğunu görmek için bir hata oluşturun.

1. Programınızda, metnin etrafındaki tırnak işaretlerini kaldırın `Serkan`, böylece satır aşağıda gösterildiği gibi görünecektir.

```
println(Serkan)
```
2. Programınızı çalıştırın. Nerede bir hata olduğunu göstermek için değiştirdiğiniz `Jhansi` kod satırının yanında kırmızı ile yazdırılmış ve bir ünlem işareti görmelisiniz .

![image](https://user-images.githubusercontent.com/70329389/145657137-ae22f652-1611-46d1-bddc-7da846a843e3.png)

3. Çıkış bölmesine bakın. Aynı ünlem işareti simgesine ve kelimesine sahip bir `Error` mesaj gösterir. Aşağıda, kodunuzdaki hatanın açıklaması yer almaktadır.

![image](https://user-images.githubusercontent.com/70329389/145657175-f0fa37a9-a315-4ac4-996e-b5005b7fd6ba.png)

4. Bu mesaj, `Unresolved reference: Serkan`, size sistemin koddaki hatanın ne olduğunu düşündüğünü söyler. Hata mesajının ne anlama geldiğini bilmeseniz bile, neyin yanlış olduğunu anlayabilirsiniz. Bu durumda `println()` komutunun metin yazdırdığını bilirsiniz. Metnin tırnak işaretleri arasında olması gerektiğini daha önce öğrenmiştiniz. Metin alıntı değilse, bu bir hatadır.

5. Devam edin ve tırnak işaretlerini tekrar ekleyin.
6. Tekrar çalıştığından emin olmak için programınızı çalıştırın.

*Tebrikler, ilk Kotlin programınızı çalıştırdınız ve değiştirdiniz!*






