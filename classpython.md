>>> class coba:
	x=5
//membuat class dengan nama coba dengan properti x
	
>>> p1=coba()
>>> print(p1.x)
5
//membuat objek dengan nama p1 daan mencetak nilai x


>>> class person:
	def __init__(self,name,age):
		self.name=name
		self.age=age
//Buat kelas bernama Person, gunakan fungsi __init __ () untuk menetapkan nilai untuk nama dan usia:
		
>>> p1=person("denol",20)
>>> print(p1.name)
denol
>>> print(p1.age)
20
//membuat objek dengan nama p1 dan mencetak nilai nama dan nilai usia

>>> class person:
	def __init__(self,name,age):
		self.name=name
		self.age=age

		
>>> def myfunc(self):
	print("hello my name is " + self.name)

	
>>> p1=person("denol",20)
>>> p1.myfunc()
//Masukkan fungsi yang mencetak ucapan, dan jalankan pada objek p1


class Person:
  def __init__(mysillyobject, name, age):
    mysillyobject.name = name
    mysillyobject.age = age
//Gunakan kata-kata mysillyobject dan abc sebagai ganti self:

  def myfunc(abc):
    print("Hello my name is " + abc.name)

p1 = Person("denol",20)
p1.myfunc()
//Parameter sendiri adalah referensi ke instance kelas saat ini, 
dan digunakan untuk mengakses variabel yang termasuk dalam kelas.

