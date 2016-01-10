#include <iostream.h>
#include <conio.h>


void main ()
{
int pilih,ukonsum;
long discount1=0,discount2=0,discount3=0,discount4=0, total,all;
long harga1=0,harga2=0,harga3=0,harga4=0,more,jml_order;
cout<<"           APLIKASI KASIR BY LEARNIT             "<<endl;
cout<<"                 153112706450017                 "<<endl;
cout<<"*************************************************"<<endl;
cout<<"SALE SOUVENIR mascot FIFA WORLD CUP  2014 “Fuleco”"<<endl;
cout<<"*************************************************"<<endl;
cout<<"++-----------------------------------------------++\n";
cout<<"||Nama Barang              || Harga              ||\n";
cout<<"++-----------------------------------------------++\n";
cout<<"||[1] Cramic Cup Coffee    || Rp 18.000          ||\n";
cout<<"||[2] USB Flash Drive      || Rp 145.000         ||\n";
cout<<"||[3] USB Pen Drive        || Rp 170.000         ||\n";
cout<<"||[4] Watch                || Rp 425.000         ||\n";
cout<<"++-----------------------------------------------++\n";
awal :
cout<<"Masukan No Barang : ";cin>>pilih;

switch(pilih)
{
    case 1 :
           cout<<"\n";
           cout<<"******SALE Logo ceramic cup Coffee Mug ******"<<endl;
         cout<<"Masukan Jumlah Order : ";cin>>jml_order;
         if(jml_order>=10 && jml_order<=19)
             { cout<<"Discount 4% \n";
            discount1=18000*14/100;
            }else if(jml_order>=20 && jml_order<=49)
            { cout<<"Discount 8% \n";
            discount1=18000*8/100;
            }else if(jml_order>=50)
            { cout<<"Discount 10% \n";
            discount1=18000*10/100;
            }
         harga1=jml_order*18000-discount1;

      break;
   case 2 :
       cout<<"\n";
       cout<<"******SALE 2014 Brasil world cup USB flash drive ******"<<endl;
         cout<<"Masukan Jumlah Order : ";cin>>jml_order;
         if(jml_order>=10 && jml_order<=19)
             {
            cout<<"Discount 5%\n";
            discount2=145000*5/100;
            }else if(jml_order>=20 && jml_order<=49)
            {
            cout<<"Discount 8%\n";
            discount2=145000*8/100;
            }else if(jml_order>=50)
            {
            cout<<"Discount 15%\n";
            discount2=14500015/100;
            }
         harga2=jml_order*145000-discount2;
      break;
      case 3 :
      cout<<"\n";
       cout<<"******SALE 2014 Brazil World Cup mascot USB pen drive ******"<<endl;
         cout<<"Masukan Jumlah Order : ";cin>>jml_order;
         if(jml_order>=10 && jml_order<=19)
             {
            cout<<"Discount 4%\n";
            discount3=170000*4/100;
            }else if(jml_order>=20 && jml_order<=49)
            {
            cout<<"Discount 8%\n";
            discount3=170000*8/100;
            }else if(jml_order>=50)
            {
            cout<<"Discount 17%\n";
            discount3=170000*17/100;
            }
         harga3=jml_order*170000-discount3;
      break;
      case 4 :
      cout<<"\n";
       cout<<"******SALE World Cup 2014 Promotional Watch Products ******"<<endl;
         cout<<"Masukan Jumlah Order : ";cin>>jml_order;
         if(jml_order>=10 && jml_order<=19)
             {
            cout<<"Discount 5%\n";
            discount4=425000*5/100;
            }else if(jml_order>=20 && jml_order<=49)
            {
            cout<<"Discount 8%\n";
            discount4=425000*5/100;
            }else if(jml_order>=50)
            {
            cout<<"Discount 15%\n";
            discount4=425000*15/100;
            }
         harga4=jml_order*425000-discount4;
      break;
}
cout<<"\n";
cout<<"tekan 1 jika ada yang di tambah tekan no sembarang untuk exit ";cin>>more;
if(more == 1)
{
goto awal;}
else{
cout<<"\n";
cout<<"++----MENU TOTAL HARGA SOUVENIR mascot FIFA WORLD CUP  2014----++"<<endl;
cout<<" Sub Total Harga Order Coffee Mug          : Rp."<<harga1<<endl;
cout<<" Sub Total Harga Order USB flash drive     : Rp."<<harga2<<endl;
cout<<" Sub Total Harga Order USB PAN drive       : Rp."<<harga3<<endl;
cout<<" Sub Total Harga Order Watch               : Rp."<<harga4<<endl;
cout<<"++-------------------------------------------------------------++"<<endl;
total=harga1+harga2+harga3+harga4;
cout<<"Total Pembayaran                           : Rp."<<total<<endl;
cout<<"-----------------------------------------------------------------\n";
cout<<"Jumlah Uang Konsumen                       : Rp.";cin>>ukonsum;
cout<<"-----------------------------------------------------------------\n";
all=ukonsum-total;
cout<<"Kembalian                                  : Rp."<<all<<endl;
}
getch();
} 
