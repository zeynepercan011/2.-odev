# 2.-odev

//verilen say�n�n kombinasyonunu bulan kod

#include<stdio.h>
int fact(int);
int comb(int,int);
int main()
{
	int x,y;
	printf("iki sayi giriniz.");
	scanf("%d%d" , &x,&y);
	
	printf("kombinasyonu: %d" , comb(x,y));
	
	return 0;
}

int fact(int x)
{
	int sonuc=1;
	for(int i=1;i<=x;i++){
		sonuc*=i;
	}
	return sonuc;
}



int comb(int x, int y)
{
	int sonuc2;
	sonuc2=(fact(x))/(fact(y)*fact(x-y));
	
	return sonuc2;
}
