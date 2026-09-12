# MaçRadar

Türkçe futbol sonuçları, haftalık fikstür, puan durumu ve takım istatistikleri.

## İçerik
- Türkiye Süper Lig: TFF'nin herkese açık fikstür ve puan cetveli.
- Bundesliga, Bundesliga 2 ve 3. Liga: OpenLigaDB.
- Mobil uyumlu arayüz; görünür sayfada 60 saniyede bir yenileme.
- API anahtarı veya ücretli veri aboneliği gerekmez. Kaynak gecikmesi ve hizmet sınırları geçerlidir; anlık veri garantisi yoktur.

`worker.js` çalışan sitenin arayüzü ve sunucu kodunu içeren tek dosyalık Cloudflare Worker sürümüdür. `wrangler.jsonc` ile kullanılabilir. `macradar-source.zip` düzenlenebilir kaynak dosyalarını içerir.

Node.js ile `npm run dev` yerel önizlemeyi açar. `npm run deploy` yalnızca kendi Cloudflare hesabınıza giriş yaptıktan sonra isteğe bağlı yayındır. Bu depo mevcut OranRadar sitesini veya ayarlarını değiştirmez.

Kaynaklar: https://www.tff.org/default.aspx?pageID=198 ve https://www.openligadb.de/

TFF sonuçları sunucuda 60 saniyeye kadar önbelleğe alınır. Kaynak hatasında eski veri en fazla 30 dakika boyunca açık bir uyarıyla gösterilebilir. TFF sayfa yapısı değişirse veri ayrıştırıcısının güncellenmesi gerekir.

Yayındaki site: https://macradar-spor-enes.mereb379.chatgpt.site
