# Rice Varieties Classification
Aplikasi ini dibuat untuk melakukan klasifikasi tiga varietas beras (Basmathi, IR-64, dan Ketan) menggunakan metode CNN (<i>Convolutional Neural Network</i>).
Program CNN dibuat menggunakan infrastruktur <i>Google Colaboratory</i> dengan bahasa pemrograman <i>Python</i> dan menggunakan <i>Framework Keras</i> dan TensorFlow yang kemudian disimpan dalam bentuk <i>file Jupyter Notebooks</i> “.ipynb”. File dari program tersebut disimpan ke layanan repositori <i>web development</i> pada <i>Platform Github</i>.
<i>Dataset</i> pelatihan dan pengujian disimpan pada <i>Github</i> dengan 3 macam kelas (varietas Beras Basmathi, IR-64, dan Ketan). Masing-masing jumlah <i>dataset</i> pelatihan setiap kelas/varietas sebanyak 75 gambar dengan format ".jpeg" dan untuk <i>dataset</i> pengujian tiap kelasnya sebanyak 15 gambar berformat ".jpeg". Untuk <i>folder dataset</i> pelatihan dan pengujian disimpan pada folder yang terpisah agar memudahkan dalam melihat pengujiannya.
Pada program klasifikasi varietas beras ini menggunakan dua macam arsitektur CNN, yaitu arsitektur MobileNetV1 dan VGG-16Net.
Teknik yang digunakan pada kedua arsitektur tersebut dilakukan dengan cara <i>Feature Extraction</i>, yaitu mentransfer hasil pelatihan dari kedua arsitektur tersebut yang telah dilatih pada <i>dataset ImageNet</i> dan untuk klasifikasinya (<i>densely connected layer</i>) menggunakan teknik <i>Global Average Pooling</i>.

Setelah dilakukannya pengujian, model dari hasil pengujian tersebut dapat disimpan dan dikonversi ke dalam bentuk <i>file Tensorflow Lite</i> ".tflite". File tersebut nantinya digunakan sebagai model yang dapat diimpor ke <i>Android Studio</i> yang tentunya juga mengimpor <i>library tensorflow</i> pada build.gradle di dalam <i>project Android Studio</i>. Kemudian dibuat aplikasi Android untuk klasifikasi varietas beras dengan menggunakan fasilitas kamera pada perangkat <i>Smartphone Android</i>.

![Rice Varieties Classification](https://github.com/Soedirman-Machine-Learning/rice-varieties-classification/blob/master/ezgif-3-377733b908a3.gif)
