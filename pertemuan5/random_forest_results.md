# Hasil Klasifikasi Sentimen dengan Random Forest

## Metrik Utama
| Metrik | Nilai |
| :--- | :--- |
| Akurasi | 93.20% |
| F1-Score (Macro Avg) | 0.933 |
| AUC (Macro Avg) | 0.992 |

## Classification Report
|              |   precision |   recall |   f1-score |   support |
|:-------------|------------:|---------:|-----------:|----------:|
| Irrelevant   |    0.957576 | 0.918605 |   0.937685 |   172     |
| Negative     |    0.923077 | 0.947368 |   0.935065 |   266     |
| Neutral      |    0.946043 | 0.922807 |   0.934281 |   285     |
| Positive     |    0.911972 | 0.935018 |   0.923351 |   277     |
| accuracy     |    0.932    | 0.932    |   0.932    |     0.932 |
| macro avg    |    0.934667 | 0.93095  |   0.932596 |  1000     |
| weighted avg |    0.93248  | 0.932    |   0.932047 |  1000     |

## Catatan Implementasi
Model Random Forest dilatih menggunakan data dari `twitter_training.csv` dan dievaluasi pada `twitter_validation.csv`.
Fitur diekstrak menggunakan **TfidfVectorizer** dengan `max_features=1700` dan `ngram_range=(1,2)`.
Preprocessing teks mencakup *lowercase*, penghapusan karakter khusus, *stopword removal*, dan *lemmatization*.
