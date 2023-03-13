# ================ BELAJAR TAILWIND CSS ================

## INSTALASI -------------------------------------------
1. menggunakan CLI
    -npm init -y
        untuk membuat package .json
    -npm install tailwindcss atau npm i tailwindcss
        untuk install tailwaind
    -npx tailwindcss init
        untuk file configurasi
2. menggunakan CDN
    -buat file index.html
    -masukan link cdn nya
    -buat file tailwind.config.js
    
configurasi --------------------------------------------
-package.json
    "scripts":{ 
        "dev":"tailwindcss -i ./tailwind.css -o ./style.css --wathc"
    },

## QUICK START -----------------------------------------

-menggunakan css sendiri :tinggal tambahkan type="text/tailwindcss" pada tag pembuka cssnya, contoh :
<style type="text/tailwindcss">
        *{
            border: 1px solid orange;
        }
</style>

-menggunakan custom sendiri : 
<script>
        module.exports = {
        theme: {
          extend: {
            spacing: { //custom spasi
              '13': '3.25rem',              
            },
            fontFamily: { //custom font family
                'inter':['Inter']
            },
          }
        }
      }
</script>

-SPACING
    MARGIN & PADDING
    -margin         : m-3   /   p-3 (paddding tidak memiliki nilai mines)
    -margin left    : ml-3
    -margin right   : ms-3
    -margin top     : mt-3
    -margin bottom  : mb-3
    -untuk margin mines, tambahkan tanda mines di depannya : -ms-3

    WIDTH & HEIGHT
    -width          : w-3
    -width left     : wl-3 
    -width right    : wr-1/2
    -width  top     : wt-3
    -width  bottom  : wb-3

-FONT
    -Font Family    : font-serif
    -Font Size      : text-4xl
    -Font Style     : italic
    -Warna Gradient : bg-gradient-to-r from-indigo-500 to-cyan-300 text-transparent bg-clip-text
         bg-gradient-to-r               : arah gradient
         from-indigo-500 to-cyan-300    : dari warna A ke warna B
         text-transparent bg-clip-text  : ubah ke warna transfaran kemudian masukan warna gradient
         untuk menggunakan 3 warna tinggal sisipkan diantara wana A degan B via-namaWarna, contoh:
         bg-gradient-to-r from-indigo-500 via-red-200 to-cyan-300 text-transparent bg-clip-text
