# laravel9_auth_with_livewire_jetstream
## 1. Install Laravel 9
```Dockerfile
composer create-project laravel/laravel laravel9_auth_with_livewire_jetstream
```
- Install Jetstream:
```Dockerfile
composer require laravel/jetstream
```
- Create Auth with Livewire:
```Dockerfile
php artisan jetstream:install livewire
OR
php artisan jetstream:install livewire --teams
```
- Dùng node js package (Cài Node.js) 
```Dockerfile
npm install
```
- run package
```Dockerfile
npm run dev
```
- run create database table
```Dockerfile
php artisan migrate
```

# Laravel 9 Jetstream Features
Laravel 9 Jetstream cung cấp tất cả các tính năng mới đều có thể cấu hình được. bạn có thể thấy có tệp cấu hình fortify.php và tệp jetstream.php nơi bạn có thể bật và tắt tùy chọn cho tính năng đó:
-  Vào config / fortify.php
```Dockerfile
....
  
'features' => [
        Features::registration(),
        Features::resetPasswords(),
        Features::emailVerification(),
        Features::updateProfileInformation(),
        Features::updatePasswords(),
        Features::twoFactorAuthentication(),
    ],
...
```
-  Vào config/jetstream.php
```Dockerfile
....
  
'features' => [
        Features::profilePhotos(),
        Features::api(),
        Features::teams(),
    ],
...
```
# Run Laravel App:
```Dockerfile
php artisan serve
```
- Vào 
http://localhost:8000/

![Container](a.png)
![Container](a1.png)
![Container](a2.png)
![Container](a3.png)
![Container](a4.png)
![Container](a5.png)
![Container](a6.png)
