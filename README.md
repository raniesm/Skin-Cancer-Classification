# Skin-Cancer-Classification

## Objective
Tujuan dari program ini adalah untuk mengembangkan model computer vision menggunakan Arrtificial Neural Networks(ANN) untuk mengklasifikasikan gambar kanker kulit. Model ini diharapkan dapat membedakan berbagai jenis lesi kulit dengan akurasi yang baik. Proses melibatkan beberapa tahap penting, termasuk pemuatan dan pra-pemrosesan data, analisis data eksploratif, rekayasa fitur (seperti augmentasi data), serta pelatihan dan evaluasi model ANN 

## Dataset
File: skin_cancer.csv

## Exploratory Data Analysis (EDA)
- Memvisualisasikan dan menganalisis distribusi fitur.
- Mengambil sampel images per kelas/fitur.
  
## Feature Engineering
- Data Augmentation
- Split Data menjadi Train, Test dan Validation Sets
- Visualize Augmented Data

## ANN TRAINING (SEQUENTIAL API)
- Tanpa Data Augmentation
- Dengan Data Augmentation

## ANN IMPROVEMENT (SEQUENTIAL API/FUNCTIONAL API)
- Best Model : berdasarkan hasil evaluasi, model VGG16 menunjukkan performa yang lebih baik dibandingkan dengan model ResNet50 dalam hal test accuracy dan precision.
- Fine Tuning VGG16 Implementation

## Hasil
- Analisis model menunjukkan bahwa VGG16 mampu menangkap lebih banyak fitur relevan dari gambar lesi kulit dibandingkan dengan ResNet50. Tren akurasi dan loss selama pelatihan dan validasi menunjukkan bahwa VGG16 memiliki kemampuan genralisasi yang lebih baik pada dataset validasi dibandingkan dengan ResNet50. Meskipn demikian, masih ada ruang untuk dapat dilakukuan peningkatan lebih lanjut dalam hal peningkatan akurasi dan kemampuan generalisasi model.

# Future Improvement
- Untuk meningkatkan performa model, terdapat beberapa hal yang dapat dilakukan diantaranya adalah menerapkan teknink augmentasi data tambahan seperti pengaturan brightness, contrast, dan pembalikan vertikal untuk lebih memperkaya set dari data train. Kemudian dilakukan penerapan fine-tuning pada lebih banyak layer dalam model pre-trained untuk memungkinkan model belajar fitur spesifik dari dataset ini. Serta dapat dilakukan dengan mencoba model lain sepeerti EfficientNet atau DenseNet yang mungkin memberikan hasil lebih baik pada model.

# Aplikasi Industri
- Model ini dapat memberikan penilaian objektif yang dapat membantu dokter kulit dalam mendiagnosis lesi kulit. Dengan memberikan informasi tambahan berdasarkan analisis gambar, model ini dapat meningkatkan akurasi diagnosis dan mengurangi human error.
- Model ini bisa diterapkan dalam layanan telemedicine, memungkinkan pasien pada daerah terpencil untuk mendapatkan diagnosis awal darri foto lesi kulit yang dikirimkan. Hal ini dapat meningkatkan aksesibilitas layanan kesehatan.
- Serta model dapat digunakan sebagai alat bantu dalam pelatihan dokter dan tenaga medis lainnya, memberikan contoh nyata dari berbagai jenis lesi kulit dan bagaimana mereka diklasifikasikan oleh model.
