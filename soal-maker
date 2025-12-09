function buatSoal50Lengkap() {
  // 1. Membuat Form Baru
  // Saya beri nama baru agar tidak tertukar dengan yang lama
  var form = FormApp.create('SOAL PRA UTS TEKKOM PTA 2025/2026 (50 Soal)');
  form.setIsQuiz(true); 
  form.setDescription('Total 50 Soal. Pilihlah jawaban yang paling tepat.');
  
  // MENGAKTIFKAN ACAK URUTAN SOAL
  form.setShuffleQuestions(true);

  // 2. Data 50 Soal (Gabungan)
  // Format: q = Soal, correct = Indeks Kunci (0=A, 1=B, dst), opts = Pilihan
  var questions = [
    // --- 30 SOAL BAGIAN PERTAMA (Opsi A-D) ---
    // Kunci: B, A, B, B, B, B, B, D, B, B, B, A, A, B, B, A, B, A, A, B, B, A, A, A, A, A, A, A, A, A
    {q: "1. Apa fungsi utama dari compiler dalam proses pengolahan bahasa pemrograman?", correct: 1, opts: ["Menyimpan program", "Menerjemahkan program sumber ke program target", "Menampilkan program ke pengguna", "Memperbaiki kesalahan dalam program"]},
    {q: "2. Apa perbedaan utama antara compiler dan interpreter?", correct: 0, opts: ["Compiler menerjemahkan program seluruhnya sebelum dieksekusi, interpreter menerjemahkan baris per baris saat dijalankan", "Interpreter lebih cepat dari compiler", "Compiler hanya untuk bahasa mesin", "Interpreter tidak dapat mendeteksi error"]},
    {q: "3. Sebutkan fase pertama dalam proses compiler dan fungsi utamanya!", correct: 1, opts: ["Syntax analysis, membuat syntax tree", "Lexical analysis, mengelompokkan karakter menjadi token", "Code generation, menghasilkan kode mesin", "Semantic analysis, melakukan pengecekan tipe"]},
    {q: "4. Dalam apa bentuk intermediate code yang umum digunakan dalam compiler?", correct: 1, opts: ["Bahasa mesin langsung", "Tiga alamat kode (three-address code)", "Bytecode Java saja", "Kode C++"]},
    {q: "5. Apa peran utama table simbol dalam sebuah compiler?", correct: 1, opts: ["Menyimpan instruksi mesin", "Menyimpan nama dan atribut variabel dan fungsi", "Mengelola memori runtime", "Mengoptimasi kode"]},
    {q: "6. Jelaskan apa itu static scope dan bagaimana pengaruhnya terhadap variabel dalam program!", correct: 1, opts: ["Scope ditentukan secara waktu eksekusi", "Scope ditentukan oleh struktur program secara statis", "Semua variabel global", "Tidak ada deklarasi variabel"]},
    {q: "7. Apa kegunaan utama dari fase optimasi kode dalam compiler?", correct: 1, opts: ["Menghilangkan kesalahan sintaks", "Mempercepat atau memperkecil kode yang dihasilkan", "Mengubah kode ke bahasa lain", "Menambah fitur dalam program"]},
    {q: "8. Apa mekanisme passing parameter yang umum di C dan Java?", correct: 3, opts: ["Call-by-reference saja", "Call-by-value saja", "Call-by-name", "Call-by-value dan referensi tergantung tipe data"]},
    {q: "9. Bagaimana aliasing dapat mempengaruhi optimasi kode dalam compiler?", correct: 1, opts: ["Tidak berpengaruh", "Membuat beberapa variabel terhubung ke lokasi memori yang sama sehingga perubahan satu berpengaruh ke lainnya", "Mempercepat proses kompilasi", "Menghasilkan kode yang lebih bersih"]},
    {q: "10. Dalam bahasa yang menggunakan dynamic scope, bagaimana variabel di-resolve?", correct: 1, opts: ["Berdasarkan lokasi statis dalam kode", "Berdasarkan call stack saat runtime", "Semua variabel global", "Disimpan dalam symbol table statis"]},
    {q: "11. Apa tujuan dari syntax-directed translation dalam compiler?", correct: 1, opts: ["Menghasilkan kode assembly secara langsung", "Menghubungkan pemahaman syntax dengan tindakan semantik untuk menghasilkan intermediate code", "Memvalidasi input pengguna", "Membuat scanner"]},
    {q: "12. Bagaimana parse tree berkaitan dengan grammar context-free?", correct: 0, opts: ["Parse tree menunjukkan derivasi dari string yang dihasilkan grammar", "Parse tree adalah program dalam bahasa mesin", "Parse tree digunakan untuk scan token", "Parse tree adalah kode sumber asli"]},
    {q: "13. Sebutkan beda utama parsing top-down dan bottom-up!", correct: 0, opts: ["Top-down dimulai dari root tree, bottom-up dari daun ke root", "Bottom-up lebih lambat", "Top-down tidak menggunakan grammar", "Bottom-up hanya untuk bahasa pemrograman sederhana"]},
    {q: "14. Bagaimana left recursion mempengaruhi recursive-descent parser?", correct: 1, opts: ["Tidak ada efek", "Menyebabkan loop rekursi tak berujung", "Mempercepat parsing", "Memudahkan pembentukan syntax tree"]},
    {q: "15. Perlunya menghilangkan left recursion dalam grammar dikarenakan?", correct: 1, opts: ["Meningkatkan efisiensi kode", "Mencegah infinite recursion pada recursive-descent parsing", "Memudahkan pembuatan lexical analyzer", "Memperjelas semantic analysis"]},
    {q: "16. Apa itu token dalam konteks lexical analysis?", correct: 0, opts: ["Sekumpulan karakter yang membentuk sebuah lexeme dan nama token-nya", "Sebuah variabel dalam program", "Kode mesin", "Instruksi syntax analyzer"]},
    {q: "17. Bagaimana lexical analyzer menangani whitespace?", correct: 1, opts: ["Mengembalikan whitespace sebagai token", "Mengabaikan dan melewati whitespace", "Mengkonversi whitespace menjadi karakter khusus", "Menghasilkan error untuk whitespace"]},
    {q: "18. Apa fungsi dari regular expression dalam lexical analyzer?", correct: 0, opts: ["Mendefinisikan pola lexeme yang valid untuk token", "Menghasilkan kode mesin", "Mengkompilasi kode sumber", "Mengganti parser"]},
    {q: "19. Apa arti dari Kleene closure pada regular expressions?", correct: 0, opts: ["Mengulang pola nol atau lebih kali", "Mengulang pola tepat sekali", "Menentukan token terakhir", "Menghasilkan satu terminal"]},
    {q: "20. Mengapa token keywords tidak diperlakukan sebagai identifier meskipun identik secara pola?", correct: 1, opts: ["Karena ada kesalahan pengenalan token", "Karena keywords adalah reserved words", "Karena keywords lebih panjang dari identifier", "Karena keywords bukan bagian bahasa pemrograman"]},
    {q: "21. Jelaskan bagaimana three-address code digunakan dalam intermediate code generation!", correct: 1, opts: ["Sebagai kode tingkat tinggi", "Sebagai format yang mendekati kode mesin untuk optimasi dan generasi kode", "Sebagai token dalam lexical analysis", "Sebagai nama variabel"]},
    {q: "22. Apa yang dimaksud dengan semantic action dalam syntax-directed translation?", correct: 0, opts: ["Kode yang dijalankan saat parsing untuk membangun intermediate code", "Parsing token", "Error handling", "Membuat syntax tree"]},
    {q: "23. Bagaimana predictive parsing menghindari backtracking?", correct: 0, opts: ["Dengan menggunakan lookahead untuk memilih produksi yang benar secara unik", "Dengan mencoba semua kemungkinan produksi", "Dengan mengabaikan grammar", "Dengan mengubah grammar menjadi lexical analyzer"]},
    {q: "24. Dalam teknik lexical analysis, apa kegunaan character classes?", correct: 0, opts: ["Mendefinisikan grup karakter yang dapat diterima dalam pola tertentu", "Untuk menyimpan kode sumber", "Mengatur urutan parsing", "Mengoptimasi kode"]},
    {q: "25. Bagaimana aliasing dapat terjadi pada parameter passing call-by-reference?", correct: 0, opts: ["Ketika dua parameter formal merujuk pada lokasi memori yang sama dari parameter aktual", "Ketika parameter di-copy satu per satu", "Ketika parameter bukan tipe data yang sama", "Ketika parameter bukan variabel"]},
    {q: "26. Jelaskan prinsip dasar finite-state machines dalam lexical analysis!", correct: 0, opts: ["Mesin state yang mengenali token berdasarkan input karakter", "Mesin yang mengoptimasi teknik parsing", "Metode untuk membangun syntax tree", "Bahasa pemrograman tingkat tinggi"]},
    {q: "27. Apa keuntungan menggunakan intermediate code representation dibandingkan langsung ke kode mesin?", correct: 0, opts: ["Memudahkan optimasi dan portabilitas kode", "Memberi output cepat tanpa error", "Mengurangi ukuran program sumber", "Memudahkan debugging program di runtime"]},
    {q: "28. Apa itu ambiguity dalam grammar dan apakah predictive parser dapat menangani grammar ambigu?", correct: 0, opts: ["Ketidakjelasan grammar dalam menghasilkan parse tree; predictive parser tidak dapat menangani grammar ambigu", "Grammar yang terlalu sederhana", "Grammar yang tidak ada aturan", "Grammar dengan satu produksian"]},
    {q: "29. Apa pendekatan umum untuk mengatasi problem left recursion pada grammar?", correct: 0, opts: ["Menghilangkan left recursion dengan transformasi grammar menjadi right recursion", "Mengganti grammar dengan token", "Mengabaikan recusion", "Menggunakan lexical analyzer saja"]},
    {q: "30. Dalam konteks compiler, apa yang dimaksud dengan 'semantic checking'?", correct: 0, opts: ["Validasi makna program selain sintaks, termasuk pengecekan tipe dan konteks", "Parsing kata kunci", "Mengeksekusi kode", "Konversi kode"]},

    // --- 20 SOAL BAGIAN KEDUA (Opsi A-E) ---
    // Kunci Baru: B, E, C, C, C, E, B, D, D, E, C, A, D, E, C, B, D, D, B, A
    {q: "31. Apa yang dimaksud dengan compiler?", correct: 1, opts: ["Program yang mengubah bahasa mesin menjadi bahasa tingkat tinggi", "Program yang membaca program dalam bahasa sumber dan menerjemahkannya ke Bahasa target", "Program yang hanya berfungsi untuk memeriksa kesalahan sintaksis", "Program yang mengoptimalkan kode tanpa mengubah bahasanya", "Program yang hanya berfungsi untuk menggabungkan file-file program"]},
    {q: "32. Manakah yang bukan merupakan tahapan dalam proses kompilasi?", correct: 4, opts: ["Lexical analyzer", "Syntax analyzer", "Intermediate code generator", "Code optimizer", "Database manager"]},
    {q: "33. Apa fungsi utama dari preprocessor dalam sistem pemrosesan bahasa?", correct: 2, opts: ["Menghasilkan kode mesin", "Melakukan analisis sintaksis", "Menggabungkan program skeletal dan melakukan fungsi makro", "Mengoptimalkan kode", "Menerjemahkan bahasa assembly ke bahasa mesin"]},
    {q: "34. Manakah yang merupakan 'cousins of the compiler'?", correct: 2, opts: ["Debugger dan optimizer", "Loader dan linker", "Preprocessor, assembler, dan loader", "Scanner dan parser", "Interpreter dan emulator"]},
    {q: "35. Apa fungsi utama dari Lexical Analyzer?", correct: 2, opts: ["Menghasilkan kode objek", "Melakukan parsing", "Membaca program sumber karakter per karakter untuk menghasilkan token", "Mengoptimasi kode", "Mendeteksi error semantik"]},
    {q: "36. Manakah dari berikut ini yang BUKAN merupakan komponen dari token?", correct: 4, opts: ["Pattern", "Lexeme", "Attribute", "Symbol table", "Parser"]},
    {q: "37. Dalam terminologi bahasa, apa yang dimaksud dengan alphabet?", correct: 1, opts: ["Kumpulan semua kata dalam bahasa", "Himpunan hingga dari simbol", "Urutan karakter dalam string", "Aturan tata bahasa", "Kumpulan token"]},
    {q: "38. Manakah dari berikut ini yang merupakan operasi pada bahasa?", correct: 3, opts: ["Substitusi", "Rotasi", "Inversi", "Concatenation", "Diferensiasi"]},
    {q: "39. Apa fungsi utama dari Syntax Analyzer?", correct: 3, opts: ["Menghasilkan kode objek", "Melakukan optimasi kode", "Membaca program sumber karakter per karakter", "Menciptakan struktur sintaksis dari program sumber yang diberikan", "Mendeteksi error semantik"]},
    {q: "40. Manakah dari berikut ini yang BUKAN merupakan jenis parser?", correct: 4, opts: ["Top-down parser", "Bottom-up parser", "LL parser", "LR parser", "Horizontal parser"]},
    {q: "41. Dalam Context-Free Grammar (CFG), apa yang dimaksud dengan terminal?", correct: 2, opts: ["Simbol non-terminal", "Simbol start", "Token dalam kasus compiler", "Variabel sintaksis", "Aturan produksi"]},
    {q: "42. Apa yang dimaksud dengan derivasi paling kanan (rightmost derivation)?", correct: 0, opts: ["Selalu memilih non-terminal paling kanan untuk diganti pada setiap langkah derivasi", "Selalu memilih non-terminal paling kiri untuk diganti pada setiap langkah derivasi", "Menghasilkan parse tree dari atas ke bawah", "Menghasilkan parse tree dari bawah ke atas", "Menghilangkan ambiguitas dalam grammar"]},
    {q: "43. Apa fungsi utama dari Syntax Analyzer?", correct: 3, opts: ["Menghasilkan kode objek", "Melakukan optimasi kode", "Membaca program sumber karakter per karakter", "Menciptakan struktur sintaksis dari program sumber yang diberikan", "Mendeteksi error semantik"]},
    {q: "44. Manakah dari berikut ini yang BUKAN merupakan jenis parser?", correct: 4, opts: ["Top-down parser", "Bottom-up parser", "LL parser", "LR parser", "Horizontal parser"]},
    {q: "45. Dalam Context-Free Grammar (CFG), apa yang dimaksud dengan terminal?", correct: 2, opts: ["Simbol non-terminal", "Simbol start", "Token dalam kasus compiler", "Variabel sintaksis", "Aturan produksi"]},
    {q: "46. Jenis derivasi yang digunakan dalam parser top-down adalah:", correct: 1, opts: ["Rightmost derivation", "Leftmost derivation", "Inorder derivation", "Postorder derivation", "Preorder derivation"]},
    {q: "47. Parser bottom-up menghasilkan:", correct: 3, opts: ["Derivasi paling kiri", "Derivasi paling kanan", "Derivasi paling kiri terbalik", "Derivasi paling kanan terbalik", "Tidak ada yang benar"]},
    {q: "48. Manakah yang bukan merupakan jenis parser bottom-up?", correct: 3, opts: ["Shift-reduce parser", "Operator precedence parser", "LR parser", "LL parser", "SLR parser"]},
    {q: "49. Dalam implementasi shift-reduce parsing menggunakan stack, aksi 'shift' berarti:", correct: 1, opts: ["Mengganti handle di stack dengan simbol nonterminal", "Memindahkan simbol input berikutnya ke atas stack", "Mengurangi isi stack", "Mengumumkan parsing berhasil", "Mendeteksi error"]},
    {q: "50. Konflik shift/reduce terjadi ketika:", correct: 0, opts: ["Parser tidak dapat memutuskan antara shift atau reduce", "Parser tidak dapat memutuskan produksi mana yang digunakan untuk reduce", "Input string tidak dapat diterima", "Stack overflow", "Tidak ada yang benar"]}
  ];

  // 3. Loop untuk memasukkan soal ke Form
  questions.forEach(function(item) {
    var mcItem = form.addMultipleChoiceItem();
    mcItem.setTitle(item.q);
    mcItem.setPoints(2); // Saya set 2 poin per soal agar Total = 100
    
    // Membuat pilihan jawaban dan menandai yang benar
    var choices = [];
    item.opts.forEach(function(opt, index) {
      var isCorrect = (index === item.correct);
      choices.push(mcItem.createChoice(opt, isCorrect));
    });
    
    mcItem.setChoices(choices);
  });

  // 4. Log URL Form
  Logger.log('Form URL: ' + form.getEditUrl());
}
