KRISTIAN SENTOSA(173210001)
DENI HERDIANA (173210002)
MARFIANA AYUIRAWATI (173210004)
RISA KURNIAWATI (173210008)

```python
def dist2D( p ):
    return (p[0]**2 + p[1]**2)**0.5

pts = [ (4.5, 3), (2.1,-1), (6.8,-3), (1.4, 2.9) ]
print(max( map(dist2D,pts) ))
7.432361670424818
```
Contoh di atas melewati fungsi len sebagai argumen,untuk menemukan nilai maksimum dari daftar poin dari asal.
```python
def dist2D( p ):
    return list(map( lambda x: x**2, [ 1, 2, 3, 4 ] ))

pts = [ (4.5, 3), (2.1,-1), (6.8,-3), (1.4, 2.9) ]
print(max( map(dist2D,pts) ))
```
Contoh di atas melewati fungsi len sebagai argumen,untuk menemukan nilai maksimum dari daftar poin dari asal.

```python
list(map( lambda x: x**2, [ 1, 2, 3, 4 ] ))
[ 1, 4, 9, 16 ]
```
 fungsi terpisah di sini dengan menulis fungsi anonim yang disebut fungsi lambda.
   Contoh diatas pertama kami hanya mengkuadratkan nilai daftar
```python
n = 100
sum( map( lambda x: x**2, range(1,n+1)))
```
menjumlahkan kuadrat dari 1 ke n

```python
def dist2D( p ):
    return max( map( lambda p: (p[0]**2 + p[1]**2)**0.5, pts) )

pts = [ (4.5, 3), (2.1,-1), (6.8,-3), (1.4, 2.9) ]
print(max( map(dist2D,pts) ))
```
teruskan sebagai argumen untuk dipetakan () adalah lokasi kode fungsi.
 menemukan nilai selisih maksimum dari daftar poin dari asal.
```python
def dist2D( p ):
    return max( map( lambda p: (p[0]**2 + p[1]**2)**0.5, pts) )

pts = [ (6,-1), (8,4), (7.5,-3), (4.4,12), (7,2) ]
print(max( map(dist2D,pts) ))
```
teruskan sebagai argumen untuk dipetakan () adalah lokasi kode fungsi.
 menemukan nilai selisih maksimum dari daftar poin dari asal.
```python
def dist2D( p ):
    return list(filter( lambda x: x>0, v))
v = [ 1, 9, -4, -8, 10, -3 ]
pts = [ (6,-1), (8,4), (7.5,-3), (4.4,12), (7,2) ]
print(max( map(dist2D,pts) ))
```
menghilangkan nilai angka kurang dari nol dengan menggunakan filter
```python
def dist2D( p ):
    return sum(filter( lambda x: x>0, v))
v = [ 1, 9, -4, -8, 10, -3 ]
20
```
menjumlahkan nilai dari hasil diatas yang menggunakan filter
```python
pts = [ (6,-1), (8,4), (7.5,-3), (4.4,12), (7,2) ]
print(max( map(dist2D,pts) ))
```
pengurutan daftar poin (x, y) berdasarkan nilai y mereka terlebih dahulu dan nilai x untuk nilai terikat y, keduanya dalam urutan menurun. 
```python
def dist2D( p ):
    return sum(filter( lambda x: x>0, v))
v = [ 1, 9, -4, -8, 10, -3 ]
pts = [(8, 12), (14, 10), (12, 10), (6, 5), (2, 5), (12, 3), \
     (5, 3), (12, 1)]
print(max( map(dist2D,pts) ))
```
pengurutan daftar poin (x, y) berdasarkan nilai y mereka terlebih dahulu dan nilai x untuk nilai terikat y, keduanya dalam urutan menurun.
```python
def dist2D( p ):
    return sorted( pts, reverse=True )
v = [ 1, 9, -4, -8, 10, -3 ]
pts = [(8, 12), (14, 10), (12, 10), (6, 5), (2, 5), (12, 3), \
     (5, 3), (12, 1)]
print(max( map(dist2D,pts) ))
```
pengurutan daftar poin (x, y) berdasarkan nilai y mereka terlebih dahulu dan nilai x untuk nilai terikat y, keduanya dalam urutan menurun.

```python
n = 8
[ i*i for i in range(1,n+1) ]
 
 [1, 4, 9, 16, 25, 36, 49, 64]


v = [ 1, 9, -4, -8, 10, -3 ]
[ x for x in v if x>0 ]
 [1, 9, 10]

v = [ 1, 9, -4, -8, 10, -3 ]
[ x*x for x in v if x>0 ]
[1, 81, 100]


[ (i,j) for i in range(1,5) for j in range(1,5) if i != j ]
[(1, 2), (1, 3), (1, 4), (2, 1), (2, 3), (2, 4), (3, 1), (3, 2),
    (3, 4), (4, 1), (4, 2), (4, 3)]
```
exercise :
 ```python
 v=[1,2,3,4,5,6,7,8,9,10]
 [x for x in v if x%2==1]
[1, 3, 5, 7, 9]
```
menampilkan nilai ganjil kurang dari 10 dengan nilai pertama lebih rendah dari nilai kedua