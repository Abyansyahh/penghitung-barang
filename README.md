# penghitung-barang
Buat ngitung barang

input_barang = input('Kamu mau beli apa hari ini?:')

barang = str(input_barang)

input_harga = input('Kamu ingin membeli ' + barang + ' seharga berapa satuannya?:')

harga = int(input_harga)

input_banyak = input('Kamu ingin membeli ' + barang + ' sebanyak?:' )

banyak = int(input_banyak)

total_harga = int (harga * banyak)

print ('Total harga yang kamu butuhkan sebanyak ' + str(total_harga) + ' untuk membeli ' + barang + ' sebanyak ' + str(banyak))

input_saldo = input('Saldo yang kamu miliki saat ini ada berapa?:')

saldo = int(input_saldo)

kembalian = int (saldo - total_harga)

print ('Saldo yang kamu miliki sebesar ' + str(saldo))

if saldo > total_harga:
    print('Kamu bisa membeli ' + barang + ' sebanyak ' + str(banyak) + ' dengan total harga sebesar ' + str(total_harga))
    print('Saldo kamu memiliki kembalian sebanyak ' + str(kembalian))

elif saldo == total_harga:
    print('Kamu bisa membeli ' + barang + ' sebanyak ' + str(banyak) + ' dengan total harga sebesar ' + str(total_harga))
    print('Saldo kamu habis')

else:
    print('Maaf kamu belum bisa membeli ' + barang)
