class _tinggi:
    def __init__(self, nama, tmpt_lahir, tgl_lahir, gender, tinggi_badan,):
        self.nama = nama
        self.tmpt_lahir = tmpt_lahir
        self.tgl_lahir = tgl_lahir
        self.gender = gender
        self.tinggi_badan = tinggi_badan
        
    def _set (self, nama, tmpt_lahir, tgl_lahir, gender, tinggi_badan,):
        self.nama = nama
        self.tmpt_lahir = tmpt_lahir
        self.tgl_lahir = tgl_lahir
        self.gender = gender
        self.tinggi_badan = tinggi_badan

    def _get (self):
        print('Nama lengkap   : ' + self.nama)
        print('TTL      : ' + self.tmpt_lahir + ', ' +  self.tgl_lahir)
        if self.gender in ['L', 'l']:
            gender = 'Laki-Laki'
        else:
            gender = 'Perempuan'
        print('Gender      :' + gender)

        if self.tinggi_badan >139:
            print('tinggi badan tidak normal')
        else:
            if self.tinggi_badan >136:
                print('tinggi badan normal')
            else:
                if self.tinggi_badan <136:
                    print('tinggi badan dingin')

print('=====================================')
print('     PROGRAM CEK TINGGI BADAN      ')
print('=====================================')

nama      = input('Nama lengkap        :')
tmpt_lahir = input('Tempat lahir        :')
tgl_lahir  = input('Tanggal lahir       :')
gender     = input('Gender L/P          :')
tinggi_badan = float(input('Masukkan tinggi badan :'))

print('======================================')

proses = _tinggi(nama,tmpt_lahir,tgl_lahir,gender,tinggi_badan)
print (proses._get())
