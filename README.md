# 144_RESPONSI-UTS-ALPRO_Kamis-12.15-Iqbal_C

// kode soal c
#include <iostream>
#include <fstream>
#include <string>
#include <vector>
using namespace std;

struct Barang {
	string namaBarang;
	int harga;
	int jumlah;
	string kode, alamat;
	int total = 0; 
};

class Toko {
private:
	string nama = "Delicia" ;
	string nim  = "144"     ;
	int saldo = 0;
	vector<Barang> brg;
	bool protek = false;
	bool vou = false;
	bool gra = false;
	
public:
	void login() {
		while (true) {
			string user, pass;
			cout << "username     : ";
			cin >> user;
			cout << "password     : ";
			cin >> pass;
			
			if (user == nama && pass == nim) {
				cout << "Selamat kamu berhasil login.n\n";
				break;
			} else {
				cout << "username dan password salah\n\n";
			}
		}
	}	
	
	void cekSaldo() {
		cout << "\nSaldo anda Rp " << saldo;
	}
	
	void tambahSaldo() {
		int tambahSaldo;
		cout << "\nMasukkan jumlah saldo yang ingin kamu tambakan : Rp" ;
		cin >> tambahSaldo;
		
		Saldo += tambahSaldo;
		cout << "\nSaldo kamu Rp: " << saldo << endl; 
	} 
	
	void tambahBarang() {
		Barang b;
		
		char lagi;
		do {
		cout << "Masukkan kode barang:        ";
		cin >>b.kode;
		cout << "Masukkan nama barang:        ";
		cin >>b.namabarang;
		cout << "Masukkan harga barang:        ";
		cin >>b.hargabarang;
		cout << "Masukkan jumlah barang:        ";
		cin >>b.jumlah;
		
		int ttlHarga = b.harga * b.jumlah; 
		b.total +=  ttlHarga;
		
		brg.puuh_back(b);
		cout << b.namabarang << " Berhasil ditambahkan ke keranjang\n";	
		
	} while lagi (lagi == 'Y' || lagi == 'y');
	
	void hapusBarang() {
		Barang.b;
		keranjang();
		string kodeps;
		cout << "\nMasukkan kode barang yang ingin dihapus : ";
		cin >> kodeps;
		
	}
	
	void alamat() {
		Barang b;
		cout << "Masukkan Alamat Penerima : ";
		cin >> b.alamat;
		
		brg.puuh_back(b);
		cout << brg[i].kode << "  " << brg[i].namaBarang << "  " << brg[i].harga << "  " << brg[i].jumlah << endl;
	}
	
	void Menu() {
		int pilih;
		do {
            cout << "\n==========================================\n";
			cout << "             Menu Marketplace\n";
			cout << "\n==========================================\n";		
			cout << "1. Cek Saldo\n";
			cout << "2. Tambah Saldo\n";
			cout << "3. Tambah Barang\n";
			cout << "4. Hapus Barang\n";
			cout << "5. Lihat Keranjang\n";
			cout << "6. Tambah Alamat\n";
			cout << "7. Voucher / Diskon\n";
			cout << "8. Proteksi\n";
			cout << "9. Ekspedisi\n";
			cout << "10. Gratis Ongkir\n";
			cout << "11. Invoice\n";
			cout << "12. Keluar\n";
			
			cout << " Pilihan Anda: ";
			cin >> pilih;
			
			if (pilih == 1) {
				cekSaldo();
			} else if (pilih == 2) {
				tambahSaldo();
			} else if (pilih == 3) {
				tambahBarang();
			} else if (pilih == 4) {
				hapusBarang();
			} else if (pilih == 5) {
				lihatKeranjang();
			} else if (pilih == 6) {
				tambahAlamat();
			} else if (pilih == 7) {
				voucher/diskon();
			} else if (pilih == 8) {
				proteksi();
			} else if (pilih == 9) {
				ekspedisi();
			} else if (pilih == 10) {
				gratisongkir();
			} else if (pilih == 11) {
				invoice();
			} else if (pilih == 12) {
				keluar();
			}
		} while (pilih != 0);
		
	};
	
int main() {
	Toko t;
	
	//t.login();
	t.menu;
	
	return 0;
}	





