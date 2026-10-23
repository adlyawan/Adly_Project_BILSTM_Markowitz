#  Dashboard Saham BUMN

Dashboard saham 20 perusahaan BUMN (BUMN20) dengan analisis teknikal, prediksi harga
BiLSTM, dan optimasi portofolio Markowitz. Backend Flask + frontend HTML/CSS/JS murni
(tanpa build step), siap dijalankan dan diedit langsung di VSCode.

## Struktur Folder

```
Dashboard/
├── backend/
│   ├── app.py            # Flask API (yfinance, indikator, LSTM, Markowitz)
│   └── requirements.txt
└── frontend/
    ├── index.html
    ├── css/style.css
    └── js/
        ├── config.js     # alamat API backend
        ├── constants.js  # daftar 20 ticker BUMN
        ├── utils.js       # formatting, helper Chart.js
        ├── theme.js       # toggle dark/light
        ├── api.js         # pembungkus fetch ke backend
        ├── overview.js    # tab Ringkasan
        ├── technical.js   # tab Analisis Teknikal
        ├── lstm.js        # tab Prediksi LSTM
        ├── portfolio.js   # tab Optimasi Portofolio
        └── app.js         # init, tab switching, sidebar
```

