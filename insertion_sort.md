# Veri Yapıları ve Algoritmalar- Proje 1
## Soru 1
**[22,27,16,2,18,6] -> Insertion Sort
Yukarı verilen dizinin sort türüne göre aşamalarını yazınız.**
*1. Adım*
Tüm dizideki en küçük eleman aranır, en başa yazılır. 2 ile 22 yer değiştirir.

|2|27|16|22|18|6|
|-|-|-|-|-|-|-|-|
*2. Adım*
2'den sonraki elemanlar içinde en küçük eleman aranır, 6 ile 27 yer değiştirir.

|2|6|16|22|18|27|
|-|-|-|-|-|-|-|-|
*3. Adım*
6'dan sonraki elemanlar içinde en küçük eleman aranır, 16 bu elemanlar içinde en küçük olduğundan yerinde kalır. 

|2|6|16|22|18|27|
|-|-|-|-|-|-|-|-|
*4. Adım*
16'dan sonraki elemanlar içinde en küçük eleman aranır, 18 ve 22 yer değiştirir.

|2|6|16|18|22|27|
|-|-|-|-|-|-|-|-|
*5. Adım*
18'den sonraki elemanlar içinde en küçük eleman aranır, 22 olduğundan dizi aynı kalır.

|2|6|16|18|22|27|
|-|-|-|-|-|-|-|-|

**Big-O gösterimini yazınız.**
Her adımda bir elemanı yerine yerleştirdiğimizden bir sonraki adımda dizinin kalan elemanlarını inceleriz. n elemanlı bir dizi için bir sonraki adımda inceleyeceğimiz eleman sayısı (n-1) olur, bu şekilde azalarak 1 eleman kalana kadar devam eder. 
n+(n-1)+(n-2)+...+2+1 işlem yapılır, n'e kadar olan sayıların toplamı [n(n+1)]/2 formülü ile hesaplanır, Big-O notasyonunda baskın elemanı kullanıyorduk, dolayısıyla insertation sort için O(n^2) olur. 

**Dizi sıralandıktan sonra 18 sayısı hangi case kapsamına girer?**

Dizinin ortasında bulunduğundan average case kapsamına girer.

---
## Soru 2
**[7,3,5,8,2,9,4,15,6] dizisinin Insertion Sort'a göre ilk 4 adımını yazınız.**
*1. Adım*
Tüm dizideki en küçük eleman aranır, en başa yazılır. 2 ile 7 yer değiştirir.

|2|3|5|8|7|9|4|15|6|
|-|-|-|-|-|-|-|-|-|-|
*2. Adım*
2'den sonraki elemanlar içinde en küçük eleman aranır, 3 olduğundan dizi aynı kalır.

|2|3|5|8|7|9|4|15|6|
|-|-|-|-|-|-|-|-|-|-|
*3. Adım*
3'ten sonraki elemanlar içinde en küçük eleman aranır, 5 ile 4 yer değiştirir. 

|2|3|4|8|7|9|5|15|6|
|-|-|-|-|-|-|-|-|-|-|
*4. Adım*
4'ten sonraki elemanlar içinde en küçük eleman aranır, 5 ve 8 yer değiştirir.

|2|3|4|5|7|9|8|15|6|
|-|-|-|-|-|-|-|-|-|-|
