# Bai-Tap
BÀI TẬP VIẾT CODE
1. so sanh hai so a,b
#include<stdio.h>
#include<conio.h>
main()
{
    float a,b;
    printf ("\nNhap vao so a :");
    scanf("%f", &a);
    printf ("\nNhap vao so b :");
    scanf("%f", &b);
    if (a==b)
        printf ("\na bang b");
    else 
        printf ("\na khong bang b");
}
2.kiem tra tinh chan le
#include<stdio.h>
#include<conio.h>
#include<math.h>
main()
{
    int a;
    printf("\nNhap vao so a :");
    scanf("%d", &a);
    if(a % 2 == 0)
        printf("\na la so chan", a);
    else
        printf("\na la so le", a);
    getch();
}
3.kiem tra nam nhuan
#include<stdio.h>
#include<conio.h>
#include<math.h>
main()
{
    int a;
    printf("\nNhap vao so nam :");
    scanf("&d", &a);
    if (a % 4 == 0)
        printf("\nNam nhuan", a);
    else 
        printf("\nNam khong nhuan", a);
    getch();
}
4.kiem tra chieu cao
#include<conio.h>
#include<stdio.h>
main()
{
    float a;
    printf("\nNhap vao chieu cao : cm");
    scanf("%f", &a);
    if (a > 170)
        printf("Cao");
    else if (a>160 && a<170)
        printf("Trung binh");
    else if (a<160)
        printf("Thap");
    getch();
}
5. dua ra so lon nhat trong 3 so bat ky
#include<conio.h>
#include<stdio.h>
main()
{
    float a,b,c;
    printf("\nNhap cao so a :");
    scanf("%f", &a);
    printf("\nNhap vao so b :");
    scanf("%f", &b);
    printf("\nNhap vao so c :");
    scanf("%f", &c);
    float max = a;
    if(max < b) 
        max == c;
    if(max < b)
        max == c;
    printf("\nSo lon nhat la %4.2f", max );
    getch();
}
6.kiem tra tinh chat tam giac
#include<conio.h>
#include<stdio.h>
#include<math.h>
main()
{
    float a,b,c;
    printf("\nNhap vao canh a :");
    scanf("%f", &a);
    printf("\nNhap vao canh b :");
    scanf("%f", &b);
    printf("\nNhap vao canh c :");
    scanf("%f", &c);
    if((a==b)||(a==c)||(b==c))
        printf("\nTam giac co 3 canh %0.2f %0.2f %0.2f la tam giac can", a,b,c);
    else if((a*a+b*b==c*c)||(a*a+c*c==b*b)||(b*b+c*c==a*a))
        printf ("\nTam giac co 3 canh %0.2f %0.2f %0.2f la tam giac vuong", a,b,c);
    else if(a==b==c)
        printf("\nTam giac co 3 canh %0.2f %0.2f %0.2f la tam giac can", a,b,c);
    else
        printf("\nTam giac binh thuong");
    getch();
}
7.giai phuong trinh bac 2
#include<conio.h>
#include<stdio.h>
#include<math.h>
main()
{
    float a,b,c,d, x1, x2;
    printf("\nNhap vao a,b,c :");
    scanf("%f%f%f", &a, &b, &c);
    d = b*b-4*a*c;
    if(d<0.0)
        printf("\nPhuong trinh vo nghiem");
    else if(d==0.0)
        printf("\nPhuong trinh co nghiem kep = %0.2f", -b/(2*a));
    else if (d>0)
        printf("\nPhuong trinh co 2 nghiem : x1=%0.2f x2=%0.2f",(-b-sqrt(d))/(2*a), (-b+sqrt(d))/(2*a));
    getch();
}
12. chuong trinh
#include<conio.h>
#include<stdio.h>
#include<math.h>
main()
{
    int MS;
    printf("\n1. Tinh dien tich hinh chu nhat");
    printf("\n2. Tinh dien tich hinh vuong");
    printf("\n3. Tinh dien tich hinh tron");
    printf("\n4. Tinh dien tich hinh tam giac");
    printf("\nMoi nhap vao tuy chon : ");
    scanf("%d", &MS);
    if(MS==1)
    {   float cd,cr;
        printf("\nNhap vao chieu dai:");
        scanf("%f", &cd);
        printf("\nNhap vao chieu rong: ");
        scanf("%f", &cr);
        printf("\nDien tich hinh chu nhat da cho la: %0.2f", cd*cr);
    }
    else if(MS==2)
    {   float v;
        printf("\nNhap vao canh hinh vuong :");
        scanf("%f", &v);
        printf("\nDien tich hinh vuong la : %0.2f", v*v);
    }
    else if(MS==3)
    {   float r;
        printf("\nNhap vao ban kinh hinh tron :");
        scanf("%f", &r);
        printf("\nDien tich hinh chu nhat da cho la : %0.2f", M_PI*r*r);
    }
    else if(MS==4)
    {   float a,b,c,p;
        printf("\nNhap vao 3 canh tam giac :");
        scanf("%f%f%f", &a, &b, &c);
        printf("\nDien tich ta, giac da cho la : %0.2f",sqrt(p*(p-a)*(p-b)*(p-c)));
    }
}
11. hien thi so ngay trong thang
#include<conio.h>
#include<stdio.h>
main()
{
    int thang;
    printf("\nNhap vao thang :");
    scanf("%d", &thang);
    if(thang ==1 || thang==3|| thang==5||thang==7||thang==8||thang==10||thang==12)
        printf("\nthang %d co 31 ngay", thang);
    else if(thang==4||thang==6||thang==9||thang==11)
        printf("\nthang %d co 30 ngay", thang);
    else if(thang==2)
        printf("\nthang %d co 28 ngay", thang);
    else
        printf("\nGia tri thang khong ton tai");
    getch();
}
10.hoa don tien dien
#include<conio.h>
#include<stdio.h>
main()
{
    float a;
    double b;
    printf("\nNhap vao So dien: ");
    scanf("%f", &a);
    if(a<=199){
        b=2000*a;
        printf("\nSo tien dien phai tra la : %4.2f VND", b);
    }
    else if (a> 200 && a< 399){
        b=2000*199+(a-199)*3000;
        printf("\nSo tien dien phai tra la : %4.2f VND", b);
    }
    else if (a> 400 && a< 599){
        b=2000*199+3000*399+4000*(a-399);
        printf("\nSo tien dien phai tra la : %4.2f VND", b);
    }
    else if (a>600){
        b= 2000*199+3000*399+4000+599+(a-599)*6000;
        printf("\nSo tien dien phai tra la : %4.2f VND", b);
    }
    getch();
}
Bai 3:
in ra 100 so dau tien
#include<conio.h>
#include<stdio.h>
main()
{
    int i,S;
    for (i==0;i<101;i++){
        S=0;
        S=S+i;
        printf("\nDay so la: %d ",S);
    }

2.




