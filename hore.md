
Imperative programming adalah paradigma programming yang mendeskripsikan komputasi dalam terminologi pernayataan yang merubah program state (keadaan). 
Dengan kata lain imperative mood dalam bahasa biasa mengekspresikan perintah untuk melakukan aksi, imperative programs mendefinisikan urutan dari perintah untuk komputer agar bisa dieksekusi.
Ciri-ciri pemrograman imperatif yaitu 
- Adanya instruksi/command/perintah/kalimat-kalimat perintah 
- Adanya status yang berubah contoh 
contoh 
```python
sample_characters = ['p','y','t','h','o','n']
sample_string = ''
sample_string
for c in sample_characters:
    sample_string = sample_string + c
    print(sample_string)

p
py
pyt
pyth
pytho
python
```	
Prosedural programming adalah imperative programming dalam program yang dibangun dari satu atau lebih procedure (juga dikenal sebagai subroutines atau functions).
Procedural programming dapat dipertimbangkan sebagai langkah ke arah declarative programming. 
Programmer sering menyebutkan, sederhana dari melihat nama, arguments dan pengembalian tipe dari procedure (dan related comments), 
keterangan procedure mengharuskan untuk melakukan tanpa perlu melihat detail dari bagaimana procedure untuk mencapai hasil tersebut. 
Dalam waktu yang sama, program lengkap masih imperative karena ia mengatur pernyataan untuk dieksekusi dan memerintah eksekusi untuk lebih luas lagi.
contoh 
```python
new_lst = [1, 2, 3, 4,6]
def sum_list(lst):
	result = 0
	for value in lst:
		result += value
	return result
print(sum_list(new_lst))

16
```

OOP (Object Oriented Programming) adalah suatu metode pemrograman yang berorientasi kepada objek. 
Tujuan dari OOP diciptakan adalah untuk mempermudah pengembangan program dengan cara mengikuti model yang telah ada di kehidupan sehari-hari. 
Jadi setiap bagian dari suatu permasalahan adalah objek, nah objek itu sendiri merupakan gabungan dari beberapa objek yang lebih kecil lagi. 
 contoh 
```python
class Computer:
    
    def __init__(self):
        self.__maxprice = 1000000

    def sell(self):
        print('Harga Jual Laptop: {}'.format(self.__maxprice))

    def setMaxPrice(self, price):
        self.__maxprice = price

laptop = Computer()
laptop.sell()

laptop.__maxprice = 900000
laptop.sell()

laptop.setMaxPrice(9000000)
laptop.sell()


Harga Jual Laptop: 1000000
Harga Jual Laptop: 1000000
Harga Jual Laptop: 9000000
>>> 
```
