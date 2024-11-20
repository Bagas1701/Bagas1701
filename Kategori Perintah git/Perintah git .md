# Panduan Perintah Git

## Memulai Area Kerja (Start a Working Area)
1. **`git clone <repository-url>`**  
   - **Fungsi**: Mengunduh salinan dari repository Git yang ada ke komputer lokal Anda.  
   - **Contoh**:
     ```bash
     git clone https://github.com/user/repo.git
     ```

2. **`git init`**  
   - **Fungsi**: Menginisialisasi repository Git baru di direktori lokal Anda.  
   - **Contoh**:
     ```bash
     git init
     ```

---

## Bekerja pada Perubahan Saat Ini (Work on the Current Change)
1. **`git add <file>`**  
   - **Fungsi**: Menambahkan perubahan file ke *staging area*.  
   - **Contoh**:
     ```bash
     git add file.txt
     git add .
     ```

2. **`git mv <old-path> <new-path>`**  
   - **Fungsi**: Memindahkan atau mengganti nama file atau direktori.  
   - **Contoh**:
     ```bash
     git mv oldname.txt newname.txt
     ```

3. **`git restore <file>`**  
   - **Fungsi**: Mengembalikan file dari *staging area* atau commit sebelumnya.  
   - **Contoh**:
     ```bash
     git restore file.txt
     ```

4. **`git rm <file>`**  
   - **Fungsi**: Menghapus file dari *working directory* dan *index*.  
   - **Contoh**:
     ```bash
     git rm file.txt
     ```

---

## Memeriksa Sejarah dan Status (Examine the History and State)
1. **`git bisect`**  
   - **Fungsi**: Mencari commit tertentu yang menyebabkan bug menggunakan *binary search*.  
   - **Contoh**:
     ```bash
     git bisect start
     git bisect bad HEAD
     git bisect good <commit-hash>
     ```

2. **`git diff`**  
   - **Fungsi**: Menampilkan perbedaan antara dua commit atau antara commit dan *working directory*.  
   - **Contoh**:
     ```bash
     git diff
     ```

3. **`git grep <pattern>`**  
   - **Fungsi**: Mencari pola teks dalam file di repository.  
   - **Contoh**:
     ```bash
     git grep "function main"
     ```

4. **`git log`**  
   - **Fungsi**: Menampilkan riwayat commit.  
   - **Contoh**:
     ```bash
     git log --oneline
     ```

5. **`git show <commit-hash>`**  
   - **Fungsi**: Menampilkan detail commit tertentu.  
   - **Contoh**:
     ```bash
     git show 123abc
     ```

6. **`git status`**  
   - **Fungsi**: Menampilkan status file di repository.  
   - **Contoh**:
     ```bash
     git status
     ```

---

## Mengelola dan Mengubah Sejarah (Grow, Mark, and Tweak Your History)
1. **`git branch`**  
   - **Fungsi**: Membuat, menghapus, atau menampilkan daftar cabang.  
   - **Contoh**:
     ```bash
     git branch
     git branch new-feature
     ```

2. **`git commit`**  
   - **Fungsi**: Menyimpan perubahan dari *staging area* ke repository.  
   - **Contoh**:
     ```bash
     git commit -m "Initial commit"
     ```

3. **`git merge <branch>`**  
   - **Fungsi**: Menggabungkan cabang lain ke cabang saat ini.  
   - **Contoh**:
     ```bash
     git merge feature-branch
     ```

4. **`git rebase`**  
   - **Fungsi**: Memindahkan commit dari cabang saat ini ke ujung cabang target.  
   - **Contoh**:
     ```bash
     git rebase main
     ```

5. **`git reset`**  
   - **Fungsi**: Mengatur ulang HEAD ke commit tertentu.  
   - **Contoh**:
     ```bash
     git reset --hard HEAD~1
     ```

6. **`git switch`**  
   - **Fungsi**: Beralih ke cabang lain.  
   - **Contoh**:
     ```bash
     git switch feature-branch
     ```

7. **`git tag`**  
   - **Fungsi**: Membuat label pada commit tertentu.  
   - **Contoh**:
     ```bash
     git tag v1.0.0
     ```

---

## Kolaborasi (Collaborate)
1. **`git fetch`**  
   - **Fungsi**: Mengunduh perubahan dari repository remote tanpa menggabungkannya.  
   - **Contoh**:
     ```bash
     git fetch origin
     ```

2. **`git pull`**  
   - **Fungsi**: Mengunduh dan menggabungkan perubahan dari repository remote ke cabang lokal.  
   - **Contoh**:
     ```bash
     git pull origin main
     ```

3. **`git push`**  
   - **Fungsi**: Mengunggah commit dari cabang lokal ke repository remote.  
   - **Contoh**:
     ```bash
     git push origin main
     ```
