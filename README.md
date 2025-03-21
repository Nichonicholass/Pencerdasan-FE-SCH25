# Pencerdasan-FE-Schematics-2025

## Daftar Isi

- [Pencerdasan-ITDEV-Schematics-2024](#pencerdasan-itdev-schematics-2024)
  - [Daftar Isi](#daftar-isi)
  - [Workflow](#workflows)
  - [Tech Stack](#tech-stack)
    - [Next JS](#next-js)
      - [Data Fetching](#data-fetching)
      - [SSR dan CSR](#ssr-dan-csr)
    - [TypeScript](#typescript)
      - [Perbedaan TypeScript dan JavaScript](#perbedaan-typescript-dan-javascript)
    - [React Hook Form](#react-hook-form)
      - [Kelebihan React Hook Form](#kelebihan-react-hook-form)
    - [Zustand](#zustand)
    - [React Query](#react-query)
  - [Express](#express)
    - [Routing](#routing)
    - [Middleware](#middleware)
    - [Controller](#controller)
    - [Service](#service)
    - [Repository](#repository)
  - [Prisma](#prisma)
  - [PostgreSQL (Supabase)](#postgresql-supabase)
  - [Layouting](#layouting)
  - [Design System](#design-system)
  - [Clean Code](#clean-code)
  - [Git \& Github](#git--github)
    - [Git](#git)
    - [GitHub](#github)
  - [Issues dan Project](#issues-dan-project)
  - [Git Branch](#git-branch)
  - [Git Commit dan Push:](#git-commit-dan-push)
  - [Pull Request](#pull-request)


## Tech Stack

### TypeScript

TypeScript adalah bahasa pemrograman open-source yang dikembangkan oleh Microsoft. TypeScript adalah `superset` dari JavaScript, yang berarti semua sintaksis dan fitur JavaScript juga tersedia di TypeScript, tetapi dengan penambahan kemampuan `tipe` (type) yang lebih kuat.

Kelebihan TypeScript antara lain:

1. Kemampuan tipe yang lebih kuat, sehingga kode menjadi lebih terstruktur dan mudah dipahami, serta memungkinkan untuk mendeteksi kesalahan pada saat kompilasi.
2. Meningkatkan produktivitas pengembang dengan memungkinkan otomatisasi refaktorisasi kode, dukungan untuk refactor yang lebih aman, dan fitur editor IntelliSense yang canggih.
3. TypeScript menawarkan fitur-fitur modern seperti async/await, dekorator, dan banyak lagi.
4. Lebih mudah untuk melakukan debugging kode TypeScript.

Kekurangan TypeScript antara lain:

1. Tidak semua pengembang atau tim pengembangan mengerti TypeScript, sehingga membutuhkan waktu belajar yang lebih lama.
2. Kode TypeScript memerlukan waktu kompilasi lebih lama daripada kode JavaScript biasa, karena memerlukan tahap kompilasi tambahan.
3. Kurangnya dukungan untuk beberapa pustaka JavaScript, terutama pustaka yang belum ditingkatkan ke TypeScript atau pustaka yang kurang populer.

#### Perbedaan TypeScript dan JavaScript

TypeScript dan JavaScript adalah dua bahasa pemrograman yang saling terkait, namun memiliki perbedaan-perbedaan berikut ini:

1. Tipe Data</br>
   JavaScript merupakan bahasa pemrograman yang bersifat dinamis, sehingga tipe data variabel bisa berubah-ubah sepanjang program berjalan. Sementara itu, TypeScript merupakan bahasa pemrograman yang statis, sehingga tipe data variabel harus didefinisikan pada saat penulisan kode.
2. Kompilasi </br>
   JavaScript dieksekusi secara langsung oleh browser atau runtime environment lainnya, sedangkan TypeScript harus dikompilasi terlebih dahulu menjadi JavaScript sebelum bisa dijalankan.
3. Fitur Baru </br>
   TypeScript memiliki fitur-fitur baru yang belum tersedia pada JavaScript, seperti interface, generic, union type, dan lain-lain.

Untuk memahami lebih detail tentang TypeScript, silahkan kunjungi [https://www.typescriptlang.org/docs/](https://www.typescriptlang.org/docs/) untuk melihat dokumentasi lengkapnya.
Atau bisa juga kunjungi
https://youtube.com/playlist?list=PLNqp92_EXZBJ4CBroxVBJEpAXoz1g-naZ untuk melihat video tutorial lengkapnya.


### Next js
Next.js adalah kerangka kerja JavaScript sumber terbuka (open source) yang digunakan untuk membuat aplikasi web dengan cepat dan mudah menggunakan React. Next.js dirancang untuk mempercepat proses pengembangan aplikasi web dengan menyediakan fitur-fitur seperti server-side rendering (SSR), pre-rendering, dan optimasi performa.

Next js Documentation : https://nextjs.org/docs


### TailwindCSS
TailwindCSS adalah framework untuk CSS yang mempermudah dalam melakukan styling CSS dengan lebih cepat dan efisien. Selain itu, TailwindCSS juga bisa membuat custom class untuk setiap component, Tailwind menyediakan kelas utility yang dapat langsung digunakan di HTML. Kelas-kelas ini mencakup margin, padding, ukuran, warna, hingga tata letak responsif, sehingga memudahkan styling tanpa harus membuat stylesheet terpisah.

Kelebihan dari TailwindCSS:

Kecepatan dan Efisiensi: sehingga mempercepat pengembangan karena tidak perlu beralih ke file CSS.
Konsistensi Desain: Utility classes memastikan tampilan yang konsisten di seluruh halaman, mengurangi risiko inkonsistensi antar komponen.
Customizable: Tailwind bisa dikustomisasi melalui konfigurasi, sehingga sesuai dengan kebutuhan desain spesifik proyek tanpa harus menulis ulang banyak kode.
Responsive Design: Tailwind menyediakan kelas bawaan untuk desain responsif, sehingga memudahkan penyesuaian tampilan di berbagai ukuran layar.

https://tailwindcss.com/

### React Query
Library yang mempermudah pengelolaan data asinkron dalam aplikasi React, terutama saat berurusan dengan API seperti mengatur state, loading, error, dan caching secara manual, React Query menangani semua itu secara otomatis dan menjadi lebih efisien.

Kelebihan:

React Query secara otomatis mengurus data fetching, error handling, dan state loading, sehingga kode jadi lebih bersih dan lebih sedikit boilerplate dibanding pengelolaan manual.
React Query bisa otomatis me-refresh data ketika dianggap usang atau ada perubahan, memastikan aplikasi selalu menampilkan data terbaru.
React Query juga mendukung mutations, yang memudahkan pengiriman data ke server (seperti menambah, mengubah, atau menghapus data). Setelah mutation berhasil, cache otomatis diperbarui, jadi UI selalu sinkron dengan data terbaru.

### React Hook Forms
React Hook Form adalah library untuk menangani form dalam aplikasi React. Library ini memanfaatkan fitur React Hooks sehingga memungkinkan pengelolaan form state, validasi, dan pengiriman data dengan lebih efisien. React Hook Form fokus pada kinerja, sehingga cocok digunakan dalam form yang kompleks dan dengan banyak input.

Kelebihan:

React Hook Form bekerja tanpa perlu re-render berlebihan setiap kali ada perubahan input. Ini menjaga performa aplikasi tetap cepat, terutama untuk form yang besar atau kompleks.
React Hook Form mendukung integrasi validasi yang mudah, baik menggunakan fitur built-in atau melalui library validasi seperti Zod.
React Hook Form mendukung penggunaan controlled components di form, memberikan fleksibilitas untuk berbagai kebutuhan.
Dengan React Hook Form, proses pengiriman data (submit) lebih sederhana, karena semuanya dikelola melalui satu fungsi handleSubmit yang menangani validasi dan pengiriman data secara otomatis.

## Git & Github

### Git

Git adalah version control system yang bertugas untuk mencatat setiap perubahan pada file. Git memiliki fungsi untuk mengelola versi source code. Git sangat penting digunakan pada sebuah projek yang dikerjakan oleh banyak orang karena git dapat membuat salinan kode yang dapat dimodifikasi tanpa mengubah dan mengganggu versi utama dari kode tersebut. Karena itu, tim yang bekerja untuk mengembangkan sebuah fitur, atau memperbaiki dapat bekerja secara pisah dan menggabungkannya kembali kepada kode utama

Git commands dasar yang biasa digunakan contohnya adalah add, commit, pull, dan push.

### GitHub

GitHub adalah tempat yang digunakan untuk menyimpan dan mengelola kode suatu project. GitHub dan git saling berhubungan, karena git menyimpan data hanya di local komputer kita saja, sedangkan github bisa menyimpan kode kita yang dapat diakses oleh banyak orang.

## Issues dan Project

Pada issues kalian dapat melihat tugas yang diberikan ke kalian, dan branch yang akan kalian gunakan untuk mengerjakan tugas tersebut. Kalian dapat melihat deadline tugas pada bagian Project. Jangan lupa keep track progress kalian di project seperti mengubah status todo menjadi in progress, dll.

## Git Branch

Kalian akan mengerjakan tugas yang diberikan pada branch yang seusai dengan Issue yang diberikan pada kalian. Untuk berpindah branch kalian dapat menggunakan perintah `git checkout -b` untuk beralih ke cabang lain:

```
git checkout -b nama_branch
```

## Git Commit dan Push:

Setelah melakukan perubahan, kalian harus melakukan commit untuk menyimpan perubahan tersebut secara lokal, dan kemudian push perubahan ke repo. Gunakan perintah berikut:

```
git add .
git commit -m "Pesan commit Anda di sini"
git push
```

Link contoh conventional commit:
https://gist.github.com/qoomon/5dfcdf8eec66a051ecd85625518cfd13

## Pull Request

Setelah task yang kalian kerjakan selesai dan sudah di push ke repo, langkah selanjutnya adalah melakukan pull request. Dan meminta review kepada staff ahli.

Ketika pada review tersebut revisi, maka lakukanlah revisi sesusai dengan apa yang diminta.
Jika kalian sudah selesai mengerjakan revisi tersebut, ulangi langkah Commit dan push.
Dan kalian dapat menuggu kembali apakah revisi kalian di acc.

## Workflows

Workflow Schematics 2024 menggunakan sistem agile project management yang terdiri dari sprint dan scrum.

1. Cek Backlog and convert to isse
![image](https://github.com/user-attachments/assets/366cfe32-4aee-4c03-ad00-272f90109ac1)

Contoh yang sudah di convert : 
![image](https://github.com/user-attachments/assets/96ccf4e3-5b0c-4b6e-9242-f6732a6524e9)

2. Buka issue dan create branch
![image](https://github.com/user-attachments/assets/3f17fbe1-2b9a-44c3-a3f6-55ce37731a5c)

biasanya akan dikasih template git fetch dan checkout branch, di copy aja.

3. Fetch dan Pindah Branch

Contoh
```   
git fetch origin
git checkout 23-slicing-diterima-dan-ditolak
```

4. Slicing dan integrasi

Slicing ->
Integrasi

5. Buat PR
kalau kalian sudah selesai

```
git add .
git commit -m "Pesan commit Anda di sini"
git push
```

contoh commit yang paling sering dipake 
```
feat: add slicing dashboard admin
fix; fix layout login
```

buka Github
Create new pull request.
![image](https://github.com/user-attachments/assets/5d4575d9-bf67-428b-8ed9-5eacf6bbdd7c)

sebelum push
pastiin branch kalian sudah rebased branch main.
```
git pull --rebase origin main
```

ada banyak cara buat cek apakah branch kalian sudah rebased, salah satunya
![image](https://github.com/user-attachments/assets/61955f86-497a-4c6c-9065-c4e207ce0323)

lalu, nunggu kalian diriview sama staffli kalian. Kalau ada revisi, boleh langsung di perbaiki.



