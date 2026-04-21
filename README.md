## Commit 1 Reflection Notes

Pada percobaan ini, saya mempelajari bagaimana browser mengirim HTTP request ke server.

Ketika saya mengakses http://127.0.0.1:7878, browser mengirim request seperti:
- Method (GET)
- Path (/)
- Header seperti Host dan User-Agent

Fungsi handle_connection digunakan untuk membaca request dari browser menggunakan BufReader.
Request dibaca per baris sampai menemukan baris kosong, lalu disimpan dalam vector dan dicetak.

Dari sini saya memahami bahwa komunikasi antara browser dan server menggunakan format HTTP request.