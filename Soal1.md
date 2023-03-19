impor  jawa . menggunakan . Pemindai ;

 tugas1 kelas  umum {
  public  static  void  main ( String [] args ){
     Inputan pemindai = Pemindai baru  ( System.in ) ; _
    Sistem . keluar . println ();
    Sistem . keluar . print ( "Masukan jumlah data: " );
    int  n = inputan . nextInt ();

    String [] namaMahasiswa = String baru  [ n ];
    int [] nilaiMahasiswa = new  int [ n ];

    untuk ( int  i = 1 ; i < n + 1 ; i ++){
      Sistem . keluar . println ( "\n-----------------------" );
      Sistem . keluar . println ( "Mahasiswa ke " + i );
      Sistem . keluar . print ( "Nama: " );
      namaMahasiswa [ i - 1 ] = inputan . berikutnya ();
      Sistem . keluar . print ( "Nila: " );
      nilaiMahasiswa [ i - 1 ] = inputan . nextInt ();
    }

    Sistem . keluar . println ( "\nDAFTAR NILAI MAHASIWA" );
    Sistem . keluar . println ( "=========================" );
    Sistem . keluar . println ( "No\tNama\tNilai\tStatus" );
    for ( int  i = 1 ; i < namaMahasiswa .panjang + 1 ; i ++) {
      String  nama = namaMahasiswa [ i - 1 ];
      int  nilai = nilaiMahasiswa [ i - 1 ];
       Status string = nilai >= 70 ? "Lulus" : "Tidak lulus" ;
      Sistem . keluar . println ( i + "\t" + nama + "\t" + nilai + "\t" + status );
    }
    Sistem . keluar . println ( "=========================" );
    float  jumlah = 0 ;
    for ( int  i = 0 ; i < nilaiMahasiswa .length ; i ++) {
      jumlah += nilaiMahasiswa [ i ];
    }
    float  rataRata = jumlah / nilaiMahasiswa . panjang ;
    Sistem . keluar . println ( "Jumlah: " + jumlah );
    Sistem . keluar . println ( "Nilai Rata-rata: " + rataRata );

    masukan . tutup ();
  }
}
