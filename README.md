/// Program Penjualan Mobil
/// 
/// Nama: Muhamad Ubaydilah
/// NIM: 1124160011
/// Kelas: TI 24 SE SH
/// Matkul: Aplikasi Mobile

void main() {
  print("=== Penjualan Mobil ===");

  // Inisialisasi variabel dengan tipe data yang tepat
  String carName = "Toyota Fortuner";
  String previousOwner = "Budi";
  String newOwner = "Andi";
  int year = 2022;
  double price = 550.0;
  bool isSold = true;

  // Memperbarui nilai harga
  price = 575.5;

  // Menampilkan detail mobil
  print(
    'Mobil: $carName, Pemilik Lama: $previousOwner, Pemilik Baru: $newOwner',
  );

  print(
    'Tahun: $year, Harga Mobil: Rp${price.toStringAsFixed(1)} Jt, Terjual: $isSold',
  );

  // Bonus awal
  String? bonus = "Gratis kaca film dan service";

  // Nilai bonus diubah menjadi null sesuai logika program
  bonus = null;

  // Menggunakan operator ?? untuk menangani nilai null agar aman saat runtime
  // Issue: Perbaikan pada pemilihan variabel untuk menghindari ketidakpastian
  // Menggunakan variabel 'bonus' secara langsung untuk mendapatkan nilai yang benar
  String ketentuan = bonus ?? "Tidak ada Ketentuan Tambahan Tentang Bonus";

  // Menampilkan hasil setelah diubah ke format uppercase
  print('Ketentuan Bonus: ${ketentuan.toUpperCase()}');
}
