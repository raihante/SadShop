﻿# SadShop
> Muhammad Reihan Triatha 19.11.2816/IF04

## Description
Program SadShop ini bertujuan menambahkan item ke sebuah keranjang digital
## Scope of Functions
Berikut beberapa fungsi dari projek ini

- Menambahkan barang dengan teknik mvc
- Penambahan fungsi voucher
- Penambahan messagebox pada saat menghapus

## Cara Kerja
logika perhitungan untuk melakukan kalkulasi terdapat pad class Payment.cs

``` csharp
class Payment
    {
        OnPaymentChangedListener paymentListener;
        public Payment(OnPaymentChangedListener paymentListener)
        {

            this.paymentListener = paymentListener;
        }

        public void updateTotal(double subTotal, double promo)
        {

            double total = subTotal - promo;
            this.paymentListener.onPriceUpdated(subTotal, total, promo);

        }
    }
```
    
## Screenshot
 <p align="center" width="100%">
 - Tampilan Awal / MainWindow
 </p>
 <br>
  <p align="center" width="100%">
  <img alt="⚡ - Tampilan Awal / MainWindow" src="https://raw.githubusercontent.com/raihante/SadShop/master/SadShop/Screenshot/ss1.png" style="display:block;float:none;margin-left:auto;margin-right:auto;width:100%"/>
</p>



 <p align="center" width="100%">
- Menu item
 </p>
 <br>
  <p align="center" width="100%">
  <img alt="⚡ - Menu item" src="https://raw.githubusercontent.com/raihante/SadShop/master/SadShop/Screenshot/ss2.png" style="display:block;float:none;margin-left:auto;margin-right:auto;width:100%"/>
</p>


 <p align="center" width="100%">
- Menu voucher
 </p>
 <br>
  <p align="center" width="100%">
  <img alt="⚡ - Menu voucher" src="https://raw.githubusercontent.com/raihante/SadShop/master/SadShop/Screenshot/ss3.png" style="display:block;float:none;margin-left:auto;margin-right:auto;width:100%"/>
</p>


 <p align="center" width="100%">
- Hasil jika item dan voucher telah ditambahkan
 </p>
 <br>
  <p align="center" width="100%">
  <img alt="⚡ - Hasil jika item dan voucher telah ditambahkan" src="https://raw.githubusercontent.com/raihante/SadShop/master/SadShop/Screenshot/ss4.png" style="display:block;float:none;margin-left:auto;margin-right:auto;width:100%"/>
</p>

> Muhammad Reihan Triatha 19.11.2816/IF04
