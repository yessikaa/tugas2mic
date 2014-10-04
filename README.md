tugas2mic
=========
#include<stdio.h>
#include<conio.h>
main()
{
	int pilih;
	float r, t, vol, luas, sisi;
	ulang;
   	printf("\n========================================\n");
   	printf("PILIH MENU DI BAWAH INI : \n");
  	printf("1. Menghitung Volume Kubus\n");
   	printf("2. Menghitung Luas Lingkaran\n");
   	printf("3. Menghitung Volume Silinder\n\n");
   	printf("Pilihan : ");
   	scanf("%d", &pilih);
      		if(pilih>3)
      		printf("MAAF KODE YANG ANDA MASUKKAN SALAH\n");
   		switch(pilih)
   	{
   	case 1:
   	printf("~~~~MENGHITUNG VOLUME KUBUS~~~~\n");
   	printf("Masukkan sisi kubus : ");
   	scanf("%f", &sisi);
   	vol=sisi*sisi*sisi;
   	printf("hasilnya = %.0f", vol);
   	break;
      	case 2:
      	printf("~~~~MENGHITUNG LUAS LINGKARAN~~~~\n");
      	printf("Masukkan jari-jari lingkaran : ");
      	scanf("%f", &r);
      	luas=3.14*r*r;
      	printf("hasilnya = %.2f", luas);
      	break;
        case 3:
        printf("~~~~MENGHITUNG VOLUME SILINDER~~~~\n");
        printf("Masukkan jari-jari silinder : ");
        printf("%f", &r);
        printf("Masukkan tinggi silinder : ");
        printf("%f", &t);
        vol=3.14*r*r*t;
        printf("hasilnya = %.2f", vol);
        break;
   	}
   	goto ulang;
}
