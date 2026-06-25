1. Apa yang dimaksud dengan State, Action, dan Reward dalam Reinforcement Learning?
State merupakan kondisi lingkungan saat ini yang ditangkap oleh agen dan memberikan informasi posisi atau situasi agen di dalam lingkungan
Action merupakan keputusan yang dapat diambil oleh agen dari state saat ini (misalnya: bergerak ke atas, bawah, kiri, kanan, menjemput, atau menurunkan penumpang).
Reward merupakan Umpan balik (bisa bernilai positif/hadiah atau negatif/hukuman) yang diberikan oleh lingkungan setelah agen melakukan suatu action yang berfungsi sebagai pemandu agar agen tahu apakah tindakannya benar atau salah.

2. Apa fungsi dari Learning Rate (α)?
Learning Rate alpha menentukan seberapa besar informasi baru akan menggantikan informasi lama.
Jika alpha = 0, agen tidak belajar apa-apa dan hanya mengandalkan pengetahuan lama.
Jika alpha = 1, agen hanya mempertimbangkan informasi paling baru dan mengabaikan apa yang sudah dipelajari sebelumnya.

3. Apa fungsi dari Discount Factor (γ)?
Discount Factor gamma itu enentukan seberapa penting nilai reward di masa depan (future rewards) dibandingkan dengan reward yang langsung diterima saat ini (immediate reward).
Jika gamma mendekati 0, agen menjadi "rabun dekat" (myopic)—hanya peduli dengan hadiah instan.
Jika gamma mendekati 1, agen menjadi "visioner" (farsighted)—lebih menghargai keuntungan jangka panjang meskipun harus melewati proses yang panjang.

4. Mengapa digunakan metode Exploration dan Exploitation?
ini digunakan untuk mengatasi dilema utama dalam RL
Exploration (Eksplorasi) itu Agen mencoba tindakan-tindakan baru yang belum pernah dicoba sebelumnya untuk mengumpulkan informasi dan memetakan lingkungan lebih baik.
Exploitation (Eksploitasi)  itu Agen menggunakan informasi/jalur terbaik yang sudah diketahuinya saat ini untuk memaksimalkan total reward.
Mengapa keduanya dibutuhkan? Jika hanya melakukan eksploitasi, agen berisiko terjebak pada strategi lokal yang kurang optimal (tidak tahu ada jalan pintas yang lebih baik). Jika hanya melakukan eksplorasi, agen tidak akan pernah mengumpulkan reward secara maksimal karena terus-menerus mencoba hal acak.

5. Bagaimana perubahan nilai reward setelah training 2000 episode?
Setelah melewati 2000 episode, grafik reward rata-rata tidak akan lagi mengalami kenaikan yang tajam. Kurva pembelajaran akan berubah menjadi garis yang cenderung mendatar konstan (plateau).
Melanjutkan training sampai 5000 episode atau lebih  itu tidak akan meningkatkan performa agen secara signifikan. Agen sudah tau rute terpendek dan cara paling efisien untuk menjemput serta menurunkan penumpang, sehingga menambah episode hanya akan membuang waktu komputasi tanpa memberikan peningkatan skor reward

Tugas Lanjutan

Modifikasi program sehingga:

Menggunakan environment Taxi-v3 Menampilkan rata-rata reward setiap 100 episode Membandingkan hasil training 1000, 2000, dan 5000 episode

reward 1000
<img width="1600" height="792" alt="WhatsApp Image 2026-06-25 at 09 48 06" src="https://github.com/user-attachments/assets/cc83e50c-a644-48c6-a465-cfcce444342f" />
<img width="1297" height="636" alt="image" src="https://github.com/user-attachments/assets/fb92d90e-68a4-4d94-9d60-606cf7990afa" />

reward 2000
<img width="1600" height="790" alt="WhatsApp Image 2026-06-25 at 09 59 16" src="https://github.com/user-attachments/assets/4f7d03aa-4f77-45d5-8bc0-48ebab92583f" />
<img width="1281" height="632" alt="image" src="https://github.com/user-attachments/assets/52afb56f-c2ef-41ef-ba2a-0660b96c8d38" />


reward 5000
<img width="1600" height="786" alt="WhatsApp Image 2026-06-25 at 09 52 57" src="https://github.com/user-attachments/assets/3f1e3708-5313-4535-9d96-065445436f3e" />
<img width="1371" height="625" alt="image" src="https://github.com/user-attachments/assets/ba494cf4-2459-44fd-b203-344136f39a2c" />


