#include <stdio.h>
#include <stdlib.h>
void nhapmang(int a[],int n){
	for(int i=0; i<n;i++){
		printf("a[%d]",i);
		scanf("%d,&a[i]");
	}
}

void xuatmang(int a[],int n){
	for(int i=0; i<n; i++){
		printf("a[%d]=",i);
		scanf("%d,&a[i]");
	}
}

void trungbinhtong(int a[],int n){
	int luutong=0, dem=0;
	for(int i=0; i<n; i++){
		if(a[i]%3==0)
		luutong=luutong+a[i];
		dem++;
	}
	float ketqua=luutong/dem;
	printf("toang so chia het cho 3 la:%.f");
}

int main(){
	int a[50],n;
	printf("nhap vao so phan tu cua mang");
	scanf("%d",&n);
	xuatmang(a,n);
	nhapmang(a,n);
	trungbinhtong(a,n);
}

