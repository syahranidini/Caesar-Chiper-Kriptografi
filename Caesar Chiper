# Fungsi untuk mengenkripsi pesan menggunakan Caesar Cipher
def encrypt(text, shift):
    result = ""
    # Iterasi melalui setiap karakter dalam teks
    for i in range(len(text)):
        char = text[i]
        # Mengenkripsi huruf besar
        if char.isupper():
            result += chr((ord(char) + shift - 65) % 26 + 65)
        # Mengenkripsi huruf kecil
        elif char.islower():
            result += chr((ord(char) + shift - 97) % 26 + 97)
        else:
            result += char  # Jika bukan huruf, tidak diubah
    return result

# Fungsi untuk mendekripsi pesan menggunakan Caesar Cipher
def decrypt(text, shift):
    return encrypt(text, -shift)

# Program utama
if __name__ == "__main__":
    # Meminta pengguna untuk memasukkan teks dan shift
    text = input("Masukkan teks yang ingin dienkripsi: ")
    shift = int(input("Masukkan jumlah pergeseran (shift): "))
    
    encrypted_text = encrypt(text, shift)
    decrypted_text = decrypt(encrypted_text, shift)

    print(f"Teks asli: {text}")
    print(f"Teks terenkripsi: {encrypted_text}")
    print(f"Teks terdekripsi: {decrypted_text}")
