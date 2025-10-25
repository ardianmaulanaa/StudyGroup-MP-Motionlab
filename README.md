"Rangkuman Minggu 1 - Version Control (Git)" 

📅 **Tugas:**  
Study Group Mobile Programming - Motionlab  
📁 **Repository:** `StudyGroup-MP-Motionlab`  
👤 **Disusun oleh:** Ardian Maulana


## 🏁 1. Inisialisasi Repository
| Command | Fungsi |
|----------|--------|
| `git init` | Membuat repository Git baru di folder lokal |
| `git clone [url]` | Menyalin repository dari GitHub ke lokal |

---

## 🌿 2. Branch (Cabang Pengembangan)
| Command | Fungsi |
|----------|--------|
| `git branch` | Menampilkan daftar branch lokal |
| `git branch [nama-branch]` | Membuat branch baru |
| `git branch -d [nama-branch]` | Menghapus branch lokal |
| `git branch -m [nama-baru]` | Mengganti nama branch saat ini |
| `git checkout [nama-branch]` | Pindah ke branch lain |
| `git checkout -b [nama-branch]` | Membuat sekaligus pindah ke branch baru |
| `git merge [nama-branch]` | Menggabungkan branch lain ke branch aktif |
| `git branch -vv` | Menampilkan branch beserta tracking-nya |

---

## 💾 3. Stage dan Commit
| Command | Fungsi |
|----------|--------|
| `git status` | Melihat status file yang berubah |
| `git add [nama-file]` | Menambahkan file ke staging area |
| `git add .` | Menambahkan semua perubahan ke staging area |
| `git commit -m "pesan commit"` | Menyimpan snapshot perubahan dengan pesan |
| `git commit -am "pesan commit"` | Menambahkan dan commit langsung semua perubahan yang sudah dilacak |
| `git restore --staged [file]` | Membatalkan file yang sudah di-add |
| `git log` | Melihat riwayat commit |
| `git diff` | Melihat perbedaan antar versi file sebelum commit |

---

## 🌍 4. Remote Repository (GitHub, GitLab, Bitbucket)
| Command | Fungsi |
|----------|--------|
| `git remote -v` | Melihat remote yang terhubung |
| `git remote add origin [url]` | Menambahkan remote repository baru |
| `git remote remove origin` | Menghapus remote repository |
| `git push -u origin [nama-branch]` | Mengunggah branch ke remote dan set tracking |
| `git push origin [nama-branch]` | Mengunggah perubahan ke branch tertentu |
| `git pull origin [nama-branch]` | Mengambil dan menggabungkan perubahan dari remote |
| `git fetch` | Mengambil update dari remote tanpa merge otomatis |

---

## 🔁 5. Sinkronisasi dan Update
| Command | Fungsi |
|----------|--------|
| `git pull` | Menarik perubahan dari remote ke lokal |
| `git fetch` | Mengambil update remote tanpa menggabungkannya |
| `git merge origin/[branch]` | Menggabungkan update remote ke branch lokal |
| `git rebase [branch]` | Menyusun ulang commit agar lebih rapi |

---

## 🧹 6. Menghapus / Mengembalikan Perubahan
| Command | Fungsi |
|----------|--------|
| `git rm [nama-file]` | Menghapus file dari repo dan staging area |
| `git restore [nama-file]` | Mengembalikan file ke versi terakhir commit |
| `git revert [commit-id]` | Membatalkan perubahan commit tertentu dengan membuat commit baru |
| `git reset --soft HEAD~1` | Mengembalikan commit terakhir tapi simpan perubahan di staging |
| `git reset --hard HEAD~1` | Menghapus commit terakhir beserta perubahannya |

---

## 🧩 7. Tagging (Penandaan Versi)
| Command | Fungsi |
|----------|--------|
| `git tag` | Melihat daftar tag |
| `git tag [nama-tag]` | Membuat tag baru |
| `git tag -d [nama-tag]` | Menghapus tag lokal |
| `git push origin [nama-tag]` | Mengunggah tag ke remote |
| `git push origin --tags` | Mengunggah semua tag ke remote |

---

## 🔐 8. Konfigurasi Git
| Command | Fungsi |
|----------|--------|
| `git config --global user.name "Nama Kamu"` | Mengatur nama pengguna |
| `git config --global user.email "email@example.com"` | Mengatur email pengguna |
| `git config --list` | Melihat konfigurasi git saat ini |

---

## 🧰 9. Informasi & Bantuan
| Command | Fungsi |
|----------|--------|
| `git --version` | Menampilkan versi Git |
| `git help [command]` | Menampilkan bantuan untuk command tertentu |

---

## 💡 10. Command Ekstra 
| Command | Fungsi |
|----------|--------|
| `git stash` | Menyimpan perubahan sementara tanpa commit |
| `git stash pop` | Mengembalikan perubahan yang di-stash |
| `git shortlog` | Ringkasan commit per penulis |
| `git show [commit-id]` | Melihat detail commit tertentu |
| `git blame [file]` | Menunjukkan siapa yang terakhir mengubah setiap baris file |

---

## 🧠 11. Advanced 
| Command | Fungsi |
|----------|--------|
| `git cherry-pick [commit-id]` | Mengambil satu commit tertentu dari branch lain |
| `git reflog` | Menampilkan semua riwayat tindakan (termasuk commit yang sudah dihapus) |
| `git clean -f` | Menghapus file yang tidak dilacak (untracked) |
| `git bisect start` | Memulai proses mencari bug antara commit tertentu |
| `git bisect good [commit-id]` | Menandai commit yang baik |
| `git bisect bad [commit-id]` | Menandai commit yang rusak |
| `git bisect reset` | Mengakhiri pencarian bug |
| `git archive --format=zip -o [nama].zip HEAD` | Mengekspor repository jadi file ZIP |
| `git gc` | Membersihkan dan mengoptimalkan repository |
| `git fsck` | Mengecek integritas data repository |
| `git submodule add [url] [path]` | Menambahkan repository lain sebagai submodule |
| `git submodule update --init --recursive` | Mengupdate semua submodule |
| `git worktree add [path] [branch]` | Menambahkan direktori kerja baru untuk branch berbeda |

---

## ⚙️ 12. GitHub CLI (Command Line Interface)

| Command | Fungsi |
|----------|--------|
| `gh repo create [nama]` | Membuat repository baru langsung dari terminal |
| `gh repo clone [nama]` | Clone repo dari GitHub via CLI |
| `gh issue list` | Menampilkan daftar issue di repository |
| `gh pr create` | Membuat pull request dari command line |
| `gh pr view` | Melihat detail pull request |
| `gh pr merge` | Menggabungkan pull request dari CLI |

---

## 🧾 13. Alias & Shortcut
| Command | Fungsi |
|----------|--------|
| `git config --global alias.st status` | Membuat alias `git st` untuk `git status` |
| `git config --global alias.cm "commit -m"` | Membuat alias commit cepat |
| `git config --global alias.br branch` | Alias untuk `git branch` |
| `git config --global alias.co checkout` | Alias untuk `git checkout` |

---

## 🧩 14. Troubleshooting / Error Umum
| Error | Solusi |
|--------|--------|
| `fatal: not a git repository` | Jalankan `git init` di folder tersebut |
| `error: failed to push some refs` | Jalankan `git pull origin [branch] --rebase` lalu `git push` |
| `merge conflict` | Edit file konflik, lalu `git add` dan `git commit` |
| `Permission denied (publickey)` | Periksa SSH key dengan `ssh-keygen` dan tambahkan ke GitHub |
| `remote origin already exists` | Jalankan `git remote remove origin` sebelum menambahkan lagi |

---

