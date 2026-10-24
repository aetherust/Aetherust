# Aetherust

Aetherust, **The Binding of Isaac: Repentance+** için steampunk/dişli temalı özel bir karakter modudur. Özel karakter görselleri, dişli temalı gözyaşı efektleri, özel tüketilebilir eşya/anlatıcı sesleri ve **Aetherust'ın WD-40'ı** adlı eşyayı içerir.

## Gereksinimler

- The Binding of Isaac: Repentance+ (Steam'deki güncel sürüm önerilir)
- [REPENTOGON](https://repentogon.com/) — modun kullandığı bazı callback ve API'ler için gereklidir.

## Kurulum

1. `Aetherust` klasörünü Isaac'in `mods` klasörüne çıkarın.
2. Klasörde `metadata.xml`, `main.lua`, `content/`, `resources/` ve `resources-dlc3/` bulunduğunu kontrol edin.
3. REPENTOGON etkin durumdayken oyunu başlatın ve Modlar menüsünden Aetherust'u etkinleştirin.
4. Mevcut kurulumu güncelliyorsanız geçmiş sürümlerden dosyaları parça parça birleştirmek yerine eski `Aetherust` klasörünü bu eksiksiz klasörle değiştirin.
5. Özel Music/SFX dostaları vardır; Oyun içi deneyiminiz için SFX ses ayarını en az 3 çubuk, Music ses ayarını ise 1 çubukta tutunuz. Kulalık kullanmanızı tavsiye ederim.

## Modun özellikleri

- Aetherust ve Tainted Aetherust karakter sürümleri.
- Özel dişli/testere tarzı gözyaşı davranışı ve buna bağlı görsel efektler.
- Özel saç, gövde ve kostüm katmanları ile karakter menüsü çizimleri.
- Hap, kart/rün/ruh taşı ve boss anlatıcısı için özel sesler.
- Özel hap/kart/anlatıcı/karakter giriş sesleri çalarken müziğin geçici olarak kısılması. Ses klibi bitince müzik geri yükselir; gözyaşı ve gözyaşından türetilen ses efektleri bu sisteme dahil değildir.
- Etkileri modun Lua kodu ve eşya XML dosyasında tanımlanmış Aetherust'ın WD-40'ı eşyası.

## Ses sistemi

Müziği geçici olarak kısma sistemi, REPENTOGON'un `MusicManager:PlayJingle` özelliğini sessiz bir döngü parçasıyla birlikte kullanır. Süre, modda bulunan hap/kart/anlatıcı/giriş WAV seslerinin uzunluğuna ve eklenen kısa bir güvenlik payına göre ayarlanır. Bu sistem oyuncunun genel müzik sesi ayarını değiştirmez. Dişli gözyaşları, gözyaşı çarpma sesleri, lazer efektleri, anahtar sesleri, hasar sesleri ve hedeflenmeyen diğer efektler müziği kısma işlemini tetiklemez.

## Sorun giderme

- REPENTOGON'un kurulu ve etkin olduğundan emin olun; bu mod REPENTOGON olmadan çalışmak üzere tasarlanmamıştır.
- Özel sesler veya müzik başlatılmazsa oyunun `log.txt` dosyasındaki Aetherust uyarılarını kontrol edin. Ayrıca `content/sounds.xml` ve `content/music.xml` yollarının `resources/` içindeki dosyalarla eşleştiğinden emin olun.
- Kurulum veya güncellemeden sonra, özellikle ses dengesi ve karakter görselleri için oyunun içinde test yapılması önerilir.

## Katkıda bulunanlar ve krediler

Mod ve üçüncü taraf proje kredileri için [`credit.txt`](credit.txt) dosyasına bakın.
