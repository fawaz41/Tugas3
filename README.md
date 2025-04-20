# Tugas3
https://studio.firebase.google.com/tugas3-05866732

#Membuat library
fawaz_library/
__init__.py
#module1.py
def sapa(fawaz):
  return f"Halo, {fawaz}!"

def kali_dua(angka):
  return angka * 2

#module2.py
class Kalkulator:
  def tambah(self, a, b):
    return a + b

  def kurang(self, a, b):
    return a - b

#__init__.py
from .module1 import sapa, kali_dua
from .module2 import Kalkulator

#Menggunakan Library
import fawaz_library

## Menggunakan fungsi dari module1.py
hasil_sapa = fawaz_library.module1.sapa("fawaz")
print(hasil_sapa)  # Output: Halo, fawaz!

hasil_kali = fawaz_library.module1.kali_dua(5)
print(hasil_kali)  # Output: 10

## Menggunakan kelas dari module2.py
kalkulator = fawaz_library.module2.Kalkulator()
hasil_tambah = kalkulator.tambah(3, 7)
print(hasil_tambah)  # Output: 10

hasil_kurang = kalkulator.kurang(10, 4)
print(hasil_kurang)  # Output: 6


from nama_library import sapa, kali_dua, Kalkulator

hasil_sapa = sapa("Andi")
print(hasil_sapa)

hasil_kali = kali_dua(10)
print(hasil_kali)

kalkulator = Kalkulator()
hasil_tambah = kalkulator.tambah(2, 8)
print(hasil_tambah)
