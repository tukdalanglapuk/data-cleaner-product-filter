
console.log("CASE 1");

const data = " riyanda_azis, ARIFIAN_SAPUTRA , hasan_harahap ";

const nama = data.trim().split(",").map(n => n.trim().toLowerCase());

const hasil = nama.join(" | ");

console.log("Array nama:", nama);
console.log("Hasil:", hasil);


console.log("\nCASE 2");

const products = [
    { name: "Laptop", price: 1000, active: true },
    { name: "Mouse", price: 20, active: false },
    { name: "Keyboard", price: 50, active: true }
];

const produkAktif = products.filter(p => p.active);

const namaProduk = produkAktif.map(p => p.name.toUpperCase());

const totalHarga = produkAktif.reduce((total, p) => total + p.price, 0);

console.log("Produk aktif:", produkAktif);
console.log("Nama produk:", namaProduk);
console.log("Total harga:", totalHarga);
