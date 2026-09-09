# Genç İşsizlik ve Eğitim Düzeyi Analizi (Türkiye)
Bu çalışma; Türkiye'de genç işsizliği ile eğitim seviyeleri arasındaki ilişkiyi, resmi istatistikler (TÜİK) ve akademik bir araştırma verisi üzerinden karşılaştırmalı olarak inceleyen bir veri analizi projesidir. Proje, aynı konuyu ele alan farklı iki veri kaynağının metodolojik ve oransal tutarsızlıklarını sorgulayarak eleştirel veri okuryazarlığını hedefler.

## Projenin Amacı ve Odak Soruları
* Eğitim düzeyi yükseldikçe genç işsizlik oranları sistematik olarak düşmekte midir?
* Resmi veriler (TÜİK) ile bağımsız akademik çalışma sonuçları birbiriyle ne ölçüde örtüşmektedir?
* İki kaynak arasındaki metodolojik veya örneklem kaynaklı farklılıklar analitik çıkarımları nasıl etkilemektedir?

## Kullanılan Araçlar
* Python (pandas, numpy, matplotlib, seaborn)
* Jupyter Notebook

## Veri Kaynakları ve Değişkenler
Analiz iki temel veri seti üzerinden yürütülmüştür:

1. **TÜİK Veri Seti (`genc_issizlik_egitim.csv`)**: Resmi istatistiklere dayalı genç işsizlik verileri
2. **Akademik Çalışma Veri Seti (`akademik_issizlik_verisi.csv`)**: Literatürden derlenen karşılaştırmalı araştırma verileri

### Temel Değişkenler
* `Yıl`: Verinin ait olduğu dönem
* `Eğitim Durumu`: Eğitim seviyesi kategorileri 
* `İşsizlik Oranı (%)`: İlgili gruptaki genç işsizlik yüzdesi

## Temel Bulgular ve Karşılaştırma
Analiz sürecinde iki kaynak arasında belirgin farklılıklar tespit edilmiştir:

| Eğitim Seviyesi | TÜİK Verisi (Yaklaşık İşsizlik Oranı) | Akademik Veri (İşsizlik Oranı) | Eğilim Farkı |
| :--- | :--- | :--- | :--- |
| **İlkokul Altı** | ~%25 | %14.5 | TÜİK'te en yüksek işsizlik bu gruptayken, akademik veride en düşüktür. |
| **Lise** | %18 – %19 | %17.0 | İki kaynakta birbirine en yakın oran bu grupta gözlenmiştir. |
| **Lisans** | %13 – %14 | %17.5 | Akademik çalışmada lisans mezunları en yüksek işsizlik oranına sahiptir. |

### Çıkarımlar
* **TÜİK Perspektifi:** Eğitim düzeyi arttıkça işsizlik oranı düzenli bir şekilde azalmakta; yükseköğretimin istihdama olumlu katkı sağladığı görülmektedir.
* **Akademik Veri Perspektifi:** Düşük eğitim düzeyindeki bireylerin iş gücü piyasasına daha erken ve kolay katılabildiği, üniversite mezunlarının ise daha yüksek işsizlik riski taşıdığı gözlemlenmiştir.
* **Veri Tutarlılığı:** Aynı dönem ve eğitim basamakları incelendiğinde ortaya çıkan bu sapmalar, veri toplama yöntemleri, örneklem tasarımı ve tanım farklılıklarının analizi doğrudan etkilediğini ortaya koymaktadır.

## Proje Yapısı
```text
├── data/
│   ├── akademik_issizlik_verisi.csv
│   └── genc_issizlik_egitim.csv
├── yorumlama_ve_analiz.pdf
├── genc_issizlik_ve_egitim_analizi.ipynb
└── README.md
```

## Geliştirici
Sıla Sarı -- Dokuz Eylül Üniversitesi, Ekonometri  
LinkedIn:www.linkedin.com/in/sıla-sarı

