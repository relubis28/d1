# Sonuçları metin dosyasına yazdır
with open('karlilik_sonuclari.txt', 'w') as f:
    for sonuc in hesaplanan_sonuclar:
        f.write(f"{sonuc['Ürün Adı']} - Karlılık Oranı: {sonuc['Karlılık Oranı (%)']:.2f}%, "
                f"Satış Oranı: {sonuc['Satış Oranı']:.2f}, Verimlilik: {sonuc['Verimlilik']:.2f}\n")

print("Sonuçlar 'karlilik_sonuclari.txt' dosyasına başarıyla kaydedildi.")
