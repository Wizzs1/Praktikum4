Nama : Wisnu Ikhwansyah saputra

Nim : 312210305

Kelas : TI 22.A3

# Praktikum 4
## Latihan 1

Masukan input sebagai berikut : 

    Character = ['Kratos','Atreus','Faye','Freya','Baldur']

    print(Character[2])
    print(Character[1:4])
    print(Character[4])


    Character[3] = 'Thrud'


    Character[3:4] = 'Sif','Odin'

    Character1 = [Character[0],Character[1]]
    print(Character1)

    Character1.append('Thor')
    print(Character1)

    Character1.extend(['Brok','Sindri','Tyr'])
    print (Character)

    Character3 = Character1 + Character

    print(Character3)
    
Maka outputnya akan jadi Seperti berikut :

<img width="713" alt="p1" src="https://user-images.githubusercontent.com/110619093/202981324-71391d24-e7d7-4676-acb7-d8374eec127b.png">

# Tugas Praktikum 3.0

Masukan input seperti di bawah ini : 

    data = []
    stop = False

    while(not stop):
        nama = input("Nama : ")
        nim = input("NIM : ")
        tugas = int(input("Nilai Tugas : "))
        uts = int(input("Nilai UTS : "))
        uas = int(input("Nilai UAS : "))
        akhir = (tugas * 30/100) + (uts * 35/100) + (uas * 35/100)
        data.append([nama,nim,tugas,uts,uas,int(akhir)])

        tanya = input('Tambahkan Data (y/t) ? ')
        if (tanya == 't'):
            stop = True

    print("==================================================================")
    print("| No |    Nama      |  NIM  | Tugas |  UTS  |  UAS  |  Akhir |")
    print("==================================================================")

    i = 0

    for nilai in data:
        i += 1
        print("| {no}  | {nama:12s} | {nim:5s} | {tugas:5d} | {uts:5d} | {uas:5d} | {akhir:6.2f} |".format(no=i, nama=nilai[0], nim=nilai[1],         tugas=nilai[2],uts=nilai[3],uas=nilai[4],akhir=nilai[5]))

    print("==================================================================")

Maka outputnya akan terlihat seperti ini : 

<img width="717" alt="p2" src="https://user-images.githubusercontent.com/110619093/202982223-bc4e5ac1-b1c4-4bd4-acdc-af7ce685ec5d.png">
