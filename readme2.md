# LaraNuxt

# repo: https://github.com/fumeapp/laranuxt
# clone: git clone --depth=1 https://github.com/fumeapp/laranuxt.git

# cara instal
# 1 install dependency laravel
# command ini akan mendownload semua depcendency laravel, disimpan di folder vendor
# mendownload berdasarkan compose.json 
composer install 

# 2 install dependency nuxt 
# command ini akan mendownload semua depcendency Nuxt, disimpan di folder node_modules 
# berdasarkan package.json 
npm install 
# atau kalau error, coba: 
npm install --legacy-peer-deps

# 3 jalankan laravel
php artisan serve 

# 4 jalankan nuxt 
npm run dev 

# copy .env.example menjadi .env 
cp .env.example .env 

# settingan laravel ada di .env 
# settingan nuxt ada di nuxt.config.ts 


# Notes tambahan untuk Laravel 
# 1 bikin database dulu, supaya programnya jalan 
# 2 lalu setup konfigurasi database di .env 
DB_CONNECTION=pgsql
DB_HOST=127.0.0.1
DB_PORT=5432
DB_DATABASE=belajar_laranuxt
DB_USERNAME=odoo
DB_PASSWORD=odoo

# 3 migrasi database laravel 
php artisan migrate --seed 

# 4 jalankan kembali laravel 
php artisan serve 
