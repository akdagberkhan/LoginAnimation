
Lottie ile Login Animasyonu

# Proje Amacı

Giriş ekranında daha hoş ve kullanıcı için daha çekici bir görüntü oluşturmak için animasyon kullanmak.

## Kullanılan Kütüphaneler

 `implementation "com.airbnb.android:lottie:3.4.0"`  

## Kullandığım Teknolojiler

Lottie(https://lottiefiles.com) sitesinden indirmiş olduğum json formatında ki animasyonumu kullanmak için yuakrıda belirttiğim kütüphaneyi kullandım.

Text ve Animasyon nesnelerimin X ve Y eksenlerinde Hareketini sağlamak için aşağıdaki kod dizilimini kullandım;
 `lottieAnimationView.animate().translationY(-4000).setDuration(4500).setStartDelay(2300);`
 
 Daha sonra onCreate methodu başladıktan sonra 4 Saniye bekleyip ikinci aktivite mi başlatmak için aşağıda ki kodlarımmı kullandım;
 `new Handler().postDelayed(new Runnable() {
            @Override
            public void run() {
                Intent intent = new Intent(getApplicationContext(),SecondActivity.class);
                startActivity(intent);
            }
        }, 4000);`

## Bazı Görüntüler 
![start](https://i.hizliresim.com/ngfj48l.png)
-
![login](https://i.hizliresim.com/q9xa672.png)


