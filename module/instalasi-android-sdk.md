# Instalasi Android SDK

Tutorial berikut bisa digunakan untuk pengguna **windows** ataupun **linux**  

Ikuti langkah - langkah berikut secara berurutan

### 1. Instalasi Android Studio
Karena android sdk sudah di bundle kedalam android studio, maka kita tidak bisa menginstall android sdk secara standalone,  maka dari itu kita perlu menginstall android studio terlebih dahulu

1. Silahkan [download android studio](https://developer.android.com/studio/index.html)

2. Pada saat instalasi, anda akan diberikan pilihan tipe instalasi, **silahkan pilih _Custom_**

3. Pastikan anda mencentang item berikut :
    - Android SDK
    - Android SDK Platform
    - Performance (Intel ® HAXM)
    - Android Virtual Device

4. Kemudian lanjutkan proses instalasi

5. Setelah instalasi selesai, anda akan disambut dengan welcome screen android studio
![welcome screen](https://raw.githubusercontent.com/wrideveloper/workshop-react-native/master/images/welcome-screen.png)

### 2. Instalasi Android SDK

1. Jalankan android studio hingga muncul welcome screen

2. Untuk membuka SDK manager, Klik _Configure_ yang terletak di kanan bawah, kemudian pilih _SDK Manager_

3. Window SDK Manager akan terbuka

4. Pilih tab SDK Platforms, kemudian centang checkbox _Show Package Details_

5. Pilih **Android 6.0 (Marshmallow)** kemudian centang item berikut :
    - Google APIs
    - Android SDK Platform 23
    - Intel x86 Atom_64 System Image
    - Google APIs Intel x86 Atom_64 System Image
![sdk platform tab](https://raw.githubusercontent.com/wrideveloper/workshop-react-native/master/images/sdk-platform-tab.png)

6. Kemudian pilih tab SDK Tools dan jangan lupa centang checkbox _Show Package Details_

7. Pilih **Android SDK Build-Tools** dan centang item **23.0.1**
![sdk tool tab](https://raw.githubusercontent.com/wrideveloper/workshop-react-native/master/images/sdk-tool-tab.png)
8. Klik _Apply_ untuk mendownload dan menginstall Android SDK
![install sdk](https://raw.githubusercontent.com/wrideveloper/workshop-react-native/master/images/sdk-install.png)

### 3. Mengatur Direktori ANDROID_HOME

#### Pada Windows :

1. Ketik _environment variables_ pada pencarian windows

2. Kemudian pilih _edit the system environment variables_

3. Window system properties akan muncul

4. Pada tab advance klik tombol _Environment Variables..._ yang terletak di pojok kanan bawah

5. Window Environment Variable akan muncul

6. Klik tombol New... pada System Variables

7. Isi variable name dengan _ANDROID_HOME_ dan Variable Value dengan direktori letak Android SDK anda berada  
    > Secara Default SDK Manager terinstall pada direktori berikut :  
c:\Users\YOUR_USERNAME\AppData\Local\Android\Sdk

![environment variable](https://raw.githubusercontent.com/wrideveloper/workshop-react-native/master/images/environtment-variable.png)

#### Pada Linux :

1. Edit file .bashrc yang terletak pada : _/home/YOUR_USERNAME/.bashrc_

2. Tambahkan perintah berikut pada akhir isi dari file .bashrc :
    > export ANDROID_HOME=$HOME/Android/Sdk
  export PATH=$PATH:$ANDROID_HOME/tools
  export PATH=$PATH:$ANDROID_HOME/platform-tools
3. Refresh konfigurasi dengan mengetikkan perintah berikut pada terminal : 
    > source ~/.bashrc