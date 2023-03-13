# BELAJAR TAILWIND CSS DAY 7 ------------------
- day 1 : instalasi
    1. INSTALASI DENGAN CDN :tinggal copas script cdn tailwind dan taruh diatas
    2. INSTALASI NPM : 
    -inisialisasi folder dengan : npm init -y
    -instal tailwind dengan : npm i tailwindcss atau npm install tailwindcss
    -inisialisasi tailwind : npx tailwindcss init
    -configuasi templates pada file tailwind.config.js di bagian conten : [./src/**/*.{hmtl,js}]
        ./src adalah nama folder
        /** adalah semua folder yang ada
        /*{html,js} adalah semua file yang ada yang berjenis html dan js
    -buat file tailwind.css yang  isinya 3 directif atau tri layers of tailwind diantaranya tailwind base,components,utilitis:
    -build tailwindcss : npx  tailwindcss -i ./src/input.css -o ./output.css --watch
    -sambung file output.css dengan file html dengan link
    -YOK BEKERJA DENGAN CLASSNYA TAILWINDCSS DI HTML

- day 2 : utilitis
    -menambah nilai custom/arbitrari value dengan: namaClass-[nilai], cth: bg-[#ffghb]
    -preflight
    -spacing & sizing
    -typography
    -color

    -backgound & border
    -rounding & shadow
    -effect & filter
        shadwo-xl shadow-indigo
        opacity-5
        blure-sm
        backdop-blure-lg bg-white/50 : berpasangan, /50 adalah nilai  opacity

    -pseudo class
        meghover dengan 2 aksi pada parent dan childern
        grup, taruh di parent
        grup-hover : text-white, taruh di chiledrn

    -transition,transformation & animation
        transform:
        scale       : untuk menmperbesar atau memperkecil objek
        rotate      : untuk memutarobjek
        translate   : untuk mengeser objek
        skew        : untuk memiringkan objek

        transitions:
        
    -layout & positioning 
    -flexbox & grid
    -responsive design