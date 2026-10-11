# Refleksi-Mata-Kuliah-Semester-2
Pengalaman belajar setiap mata kuliah di semester 2
<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Portofolio Refleksi PPG Penjas - Bayu Rahayu</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        brand: {
                            50: '#f0fdf4',
                            100: '#dcfce7',
                            500: '#22c55e',
                            600: '#16a34a',
                            700: '#15803d',
                            800: '#166534',
                            900: '#14532d',
                        }
                    }
                }
            }
        }
    </script>
    <style>
        .tab-btn.active {
            background-color: #16a34a;
            color: white;
            border-color: #16a34a;
        }
        .indicator-card {
            transition: all 0.3s ease;
        }
        .indicator-card:hover {
            transform: translateY(-2px);
        }
    </style>
</head>
<body class="bg-slate-50 font-sans text-slate-800 antialiased min-h-screen flex flex-col">

    <!-- Header / Banner -->
    <header class="bg-gradient-to-r from-slate-900 via-brand-900 to-slate-900 text-white py-10 px-4 sm:px-6 lg:px-8 shadow-lg border-b-4 border-brand-500">
        <div class="max-w-6xl mx-auto flex flex-col md:flex-row justify-between items-center gap-6">
            <div class="text-center md:text-left">
                <div class="inline-flex items-center gap-2 bg-brand-500/20 text-brand-100 text-xs font-semibold px-3 py-1 rounded-full border border-brand-500/30 mb-3">
                    <i class="fa-solid font-bold fa-graduation-cap"></i> Portofolio Digital Refleksi Semester 2
                </div>
                <h1 class="text-3xl sm:text-4xl font-extrabold tracking-tight text-white">
                    Bayu Rahayu, S.Pd.
                </h1>
                <p class="text-slate-300 text-sm mt-1 flex flex-wrap items-center justify-center md:justify-start gap-4">
                    <span><i class="fa-solid fa-id-card text-brand-500 mr-1"></i> NIM: 2186250029</span>
                    <span><i class="fa-solid fa-user-graduate text-brand-500 mr-1"></i> Prodi: PPG Penjas B</span>
                    <span><i class="fa-solid fa-school text-brand-500 mr-1"></i> Lokasi PPL: SMPN 4 Ciamis</span>
                </p>
            </div>
            <div class="bg-white/10 backdrop-blur-md p-4 rounded-xl border border-white/10 text-center min-w-[200px]">
                <span class="block text-xs uppercase tracking-wider text-slate-300">Total Mata Kuliah</span>
                <span class="text-3xl font-black text-brand-500">5 Course</span>
                <span class="block text-xs text-slate-300 mt-1">Refleksi LK 3 Completed</span>
            </div>
        </div>
    </header>

    <!-- Main Content Layout -->
    <main class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8 py-8 flex-grow w-full">

        <!-- Navigation Tabs -->
        <div class="mb-8">
            <h2 class="text-xs uppercase font-bold tracking-wider text-slate-500 mb-3">Pilih Mata Kuliah Refleksi:</h2>
            <div class="flex flex-wrap gap-2 border-b border-slate-200 pb-4 overflow-x-auto" id="courseTabs">
                <button onclick="switchTab('pse')" id="tab-pse" class="tab-btn active px-4 py-2.5 rounded-lg border border-slate-300 font-medium text-sm flex items-center gap-2 transition-all shadow-sm">
                    <i class="fa-solid fa-heart-pulse"></i> PSE
                </button>
                <button onclick="switchTab('pmadl')" id="tab-pmadl" class="tab-btn px-4 py-2.5 rounded-lg border border-slate-300 font-medium text-sm flex items-center gap-2 bg-white text-slate-700 hover:bg-slate-100 transition-all shadow-sm">
                    <i class="fa-solid fa-layer-group"></i> PMADL (DUP & TaRL)
                </button>
                <button onclick="switchTab('ppl')" id="tab-ppl" class="tab-btn px-4 py-2.5 rounded-lg border border-slate-300 font-medium text-sm flex items-center gap-2 bg-white text-slate-700 hover:bg-slate-100 transition-all shadow-sm">
                    <i class="fa-solid fa-chalkboard-user"></i> PPL Mandiri
                </button>
                <button onclick="switchTab('pkp')" id="tab-pkp" class="tab-btn px-4 py-2.5 rounded-lg border border-slate-300 font-medium text-sm flex items-center gap-2 bg-white text-slate-700 hover:bg-slate-100 transition-all shadow-sm">
                    <i class="fa-solid fa-people-group"></i> Projek Kepemimpinan
                </button>
                <button onclick="switchTab('dt')" id="tab-dt" class="tab-btn px-4 py-2.5 rounded-lg border border-slate-300 font-medium text-sm flex items-center gap-2 bg-white text-slate-700 hover:bg-slate-100 transition-all shadow-sm">
                    <i class="fa-solid fa-lightbulb"></i> Design Thinking
                </button>
            </div>
        </div>

        <!-- Content Panels -->

        <!-- 1. Pembelajaran Sosial Emosional (PSE) -->
        <div id="panel-pse" class="course-panel space-y-6">
            <div class="bg-white rounded-xl p-6 border border-slate-200 shadow-sm flex items-start justify-between">
                <div>
                    <span class="bg-emerald-100 text-emerald-800 text-xs font-semibold px-2.5 py-0.5 rounded">Mata Kuliah 1</span>
                    <h2 class="text-2xl font-bold text-slate-900 mt-1">Pembelajaran Sosial Emosional (PSE)</h2>
                    <p class="text-sm text-slate-600 mt-1">Pengembangan 5 kompetensi CASEL, regulasi emosi guru, dan iklim kelas kondusif dalam PJOK.</p>
                </div>
            </div>

            <!-- 4C Grid -->
            <div class="grid md:grid-cols-2 gap-4">
                <div class="indicator-card bg-white p-5 rounded-xl border-l-4 border-blue-500 shadow-sm">
                    <div class="flex items-center gap-2 text-blue-600 font-bold mb-2">
                        <i class="fa-solid fa-link"></i>
                        <h3>Connection (Keterkaitan)</h3>
                    </div>
                    <p class="text-sm text-slate-700 leading-relaxed">
                        Materi PSE berbasis kerangka CASEL sangat erat dengan peran guru PJOK. Tugas guru tidak hanya mengajarkan keterampilan fisik/motorik, melainkan mengelola iklim kelas, membangun hubungan positif, serta membimbing siswa memiliki kesadaran diri, regulasi emosi, empati, dan tanggung jawab. Membantu menghadapi kelas gaduh atau konflik secara tenang, asertif, dan profesional.
                    </p>
                </div>

                <div class="indicator-card bg-white p-5 rounded-xl border-l-4 border-amber-500 shadow-sm">
                    <div class="flex items-center gap-2 text-amber-600 font-bold mb-2">
                        <i class="fa-solid fa-triangle-exclamation"></i>
                        <h3>Challenge (Tantangan & Perbedaan)</h3>
                    </div>
                    <p class="text-sm text-slate-700 leading-relaxed">
                        Refleks awal dulu saat kelas gaduh adalah menegur dengan suara keras/sanksi. PSE menantang hal ini dengan menekankan regulasi emosi guru terlebih dahulu (berhenti sejenak, ambil napas). Selain itu, bergeser dari aturan sepihak menjadi <i>class agreement</i> kolaboratif serta pengintegrasian PSE dalam modul ajar (Deep Learning, TaRL, Silih Asah-Asih-Asuh).
                    </p>
                </div>

                <div class="indicator-card bg-white p-5 rounded-xl border-l-4 border-emerald-500 shadow-sm">
                    <div class="flex items-center gap-2 text-emerald-600 font-bold mb-2">
                        <i class="fa-solid fa-brain"></i>
                        <h3>Concept (Konsep Utama)</h3>
                    </div>
                    <ul class="text-sm text-slate-700 list-disc list-inside space-y-1">
                        <li><b>5 Kompetensi CASEL:</b> Self-awareness, Self-management, Social Awareness, Relationship Skills, Responsible Decision-Making.</li>
                        <li><b>Penerapan PSE:</b> Rutin, terintegrasi mata pelajaran, dan pembiasaan budaya sekolah.</li>
                        <li><b>Komunikasi Asertif & Regulasi Emosi Guru:</b> Menciptakan iklim aman tanpa kekerasan verbal.</li>
                    </ul>
                </div>

                <div class="indicator-card bg-white p-5 rounded-xl border-l-4 border-purple-500 shadow-sm">
                    <div class="flex items-center gap-2 text-purple-600 font-bold mb-2">
                        <i class="fa-solid fa-arrows-rotate"></i>
                        <h3>Change (Perubahan Diri)</h3>
                    </div>
                    <p class="text-sm text-slate-700 leading-relaxed">
                        <b>Pra-Mengajar:</b> Mindfulness & menyusun kesepakatan kelas.<br>
                        <b>Saat Mengajar:</b> Komunikasi asertif (sopan tapi tegas) & integrasi PSE dalam PJOK (saling menghargai & kerja sama).<br>
                        <b>Pasca-Mengajar:</b> Refleksi rutin & kolaborasi sinergis dengan Guru BK, wali kelas, dan orang tua.
                    </p>
                </div>
            </div>

            <!-- Artefak Section -->
            <div class="bg-slate-900 text-white p-6 rounded-xl shadow-sm">
                <h3 class="text-lg font-bold mb-3 flex items-center gap-2 text-brand-500">
                    <i class="fa-solid fa-folder-open"></i> Analisis Artefak Pembelajaran
                </h3>
                <div class="space-y-3 text-sm text-slate-300">
                    <div>
                        <span class="font-semibold text-white">Artefak Dipilih:</span>
                        <p class="mt-0.5">1. Lembar Tugas Refleksi / Studi Kasus Individu & Kelompok (Kasus Pak AZ / Kelas Gaduh).<br>2. Modul Ajar PJOK Kurikulum Merdeka (Deep Learning) Kelas VIII SMPN 4 Ciamis (Materi Passing Bola Voli).</p>
                    </div>
                    <div>
                        <span class="font-semibold text-white">Alasan Pemilihan:</span>
                        <p class="mt-0.5">Merepresentasikan proses belajar yang utuh: dari pemahaman teoretis PSE, pemecahan kasus nyata di lapangan (problem solving), hingga penerapan praktis Modul Ajar terintegrasi untuk PPL.</p>
                    </div>
                    <div>
                        <span class="font-semibold text-white">Bagian Pendukung Refleksi:</span>
                        <p class="mt-0.5">Langkah regulasi emosi & komunikasi asertif pada studi kasus; serta Identifikasi Kesiapan Siswa, Integrasi CRT (Silih Asah-Asih-Asuh), dan Desain Langkah Pembelajaran Zona 1-3 pada Modul Ajar.</p>
                    </div>
                </div>
            </div>
        </div>

        <!-- 2. Pembelajaran Mendalam dan Asesmen Dasar Lanjutan (PMADL) -->
        <div id="panel-pmadl" class="course-panel hidden space-y-6">
            <div class="bg-white rounded-xl p-6 border border-slate-200 shadow-sm">
                <span class="bg-emerald-100 text-emerald-800 text-xs font-semibold px-2.5 py-0.5 rounded">Mata Kuliah 2</span>
                <h2 class="text-2xl font-bold text-slate-900 mt-1">Pembelajaran Mendalam & Asesmen Dasar Lanjutan</h2>
                <p class="text-sm text-slate-600 mt-1">Penerapan Desain Universal untuk Pembelajaran (DUP) dan Teaching at the Right Level (TaRL).</p>
            </div>

            <div class="grid md:grid-cols-2 gap-4">
                <div class="indicator-card bg-white p-5 rounded-xl border-l-4 border-blue-500 shadow-sm">
                    <div class="flex items-center gap-2 text-blue-600 font-bold mb-2">
                        <i class="fa-solid fa-link"></i>
                        <h3>Connection (Keterkaitan)</h3>
                    </div>
                    <p class="text-sm text-slate-700 leading-relaxed">
                        DUP dan TaRL sangat relevan dengan keberagaman murid PJOK (kebugaran, motorik, kepercayaan diri). Guru bukan sekadar melatih gerakan mekanis, tetapi perancang pengalaman belajar inklusif dan adaptif agar semua murid mendapat kesempatan setara untuk sukses.
                    </p>
                </div>

                <div class="indicator-card bg-white p-5 rounded-xl border-l-4 border-amber-500 shadow-sm">
                    <div class="flex items-center gap-2 text-amber-600 font-bold mb-2">
                        <i class="fa-solid fa-triangle-exclamation"></i>
                        <h3>Challenge (Tantangan & Perbedaan)</h3>
                    </div>
                    <p class="text-sm text-slate-700 leading-relaxed">
                        Mendobrak pandangan tradisional bahwa kesulitan belajar adalah "kurang bakat". Hambatan sebenarnya berasal dari desain pembelajaran yang kaku. Mengubah pendekatan seragam (*one-size-fits-all*) menjadi pembelajaran berjenjang berbasis pos/stasiun dan instruksi multimodal.
                    </p>
                </div>

                <div class="indicator-card bg-white p-5 rounded-xl border-l-4 border-emerald-500 shadow-sm">
                    <div class="flex items-center gap-2 text-emerald-600 font-bold mb-2">
                        <i class="fa-solid fa-brain"></i>
                        <h3>Concept (Konsep Utama)</h3>
                    </div>
                    <ul class="text-sm text-slate-700 list-disc list-inside space-y-1">
                        <li><b>Prinsip DUP:</b> Beragam cara Engagement, Representation, serta Action & Expression.</li>
                        <li><b>Prinsip TaRL:</b> Asesmen diagnostik awal, pengelompokan dinamis, dan zona ZPD.</li>
                        <li><b>Sintesis DUP + TaRL:</b> DUP memastikan akses masuk, TaRL memastikan kemajuan belajar sesuai titik awal.</li>
                    </ul>
                </div>

                <div class="indicator-card bg-white p-5 rounded-xl border-l-4 border-purple-500 shadow-sm">
                    <div class="flex items-center gap-2 text-purple-600 font-bold mb-2">
                        <i class="fa-solid fa-arrows-rotate"></i>
                        <h3>Change (Perubahan Diri)</h3>
                    </div>
                    <p class="text-sm text-slate-700 leading-relaxed">
                        Bergeser dari menyalahkan kondisi murid ke mengevaluasi desain mengajar. Selalu menyusun asesmen diagnostik cepat, menyiapkan media multimodal (kartu visual/video), dan mengaplikasikan stasiun belajar dinamis berjenjang.
                    </p>
                </div>
            </div>

            <div class="bg-slate-900 text-white p-6 rounded-xl shadow-sm">
                <h3 class="text-lg font-bold mb-3 flex items-center gap-2 text-brand-500">
                    <i class="fa-solid fa-folder-open"></i> Analisis Artefak Pembelajaran
                </h3>
                <div class="space-y-3 text-sm text-slate-300">
                    <div>
                        <span class="font-semibold text-white">Artefak Dipilih:</span>
                        <p class="mt-0.5">1. Studi Kasus Bu Rina (Lompat Jauh Gaya Jongkok - Slide Gamma).<br>2. Laporan Sintesis Strategi Pembelajaran Individu (Passing Voli Kelas VIII).<br>3. Esai Tilik Diri & Action Plan.</p>
                    </div>
                    <div>
                        <span class="font-semibold text-white">Alasan Pemilihan:</span>
                        <p class="mt-0.5">Menunjukkan rekam jejak perkembangan komprehensif: kemampuan mendiagnosis masalah ketimpangan, merancang skenario kontekstual 2x40 menit, hingga evaluasi diri "mengajar untuk semua".</p>
                    </div>
                    <div>
                        <span class="font-semibold text-white">Bagian Pendukung Refleksi:</span>
                        <p class="mt-0.5">Rancangan pos latihan berjenjang (pemula, menengah, mahir) pada studi kasus lompat jauh dan matriks skenario passing bola voli berbasis asesmen diagnostik.</p>
                    </div>
                </div>
            </div>
        </div>

        <!-- 3. PPL Mandiri -->
        <div id="panel-ppl" class="course-panel hidden space-y-6">
            <div class="bg-white rounded-xl p-6 border border-slate-200 shadow-sm">
                <span class="bg-emerald-100 text-emerald-800 text-xs font-semibold px-2.5 py-0.5 rounded">Mata Kuliah 3</span>
                <h2 class="text-2xl font-bold text-slate-900 mt-1">PPL Mandiri (SMPN 4 Ciamis)</h2>
                <p class="text-sm text-slate-600 mt-1">Praktik Pengalaman Lapangan dan Implementasi Nyata Teori Perkuliahan di Kelas PJOK.</p>
            </div>

            <div class="grid md:grid-cols-2 gap-4">
                <div class="indicator-card bg-white p-5 rounded-xl border-l-4 border-blue-500 shadow-sm">
                    <div class="flex items-center gap-2 text-blue-600 font-bold mb-2">
                        <i class="fa-solid fa-link"></i>
                        <h3>Connection (Keterkaitan)</h3>
                    </div>
                    <p class="text-sm text-slate-700 leading-relaxed">
                        Teori PSE, Design Thinking, dan PMADL menjadi landasan praktis PPL di SMPN 4 Ciamis. Mengajar langsung membantu menghubungkan psikologi perkembangan remaja dengan metodologi pembelajaran PJOK di lapangan.
                    </p>
                </div>

                <div class="indicator-card bg-white p-5 rounded-xl border-l-4 border-amber-500 shadow-sm">
                    <div class="flex items-center gap-2 text-amber-600 font-bold mb-2">
                        <i class="fa-solid fa-triangle-exclamation"></i>
                        <h3>Challenge (Tantangan & Perbedaan)</h3>
                    </div>
                    <p class="text-sm text-slate-700 leading-relaxed">
                        Asumsi awal bahwa Modul Ajar dapat diterapkan kaku terpatahkan. Keanekaragaman tingkat pemahaman & keaktifan tiap kelas menuntut fleksibilitas tinggi dan penyesuaian strategi secara *real-time* di lapangan.
                    </p>
                </div>

                <div class="indicator-card bg-white p-5 rounded-xl border-l-4 border-emerald-500 shadow-sm">
                    <div class="flex items-center gap-2 text-emerald-600 font-bold mb-2">
                        <i class="fa-solid fa-brain"></i>
                        <h3>Concept (Konsep Utama)</h3>
                    </div>
                    <ul class="text-sm text-slate-700 list-disc list-inside space-y-1">
                        <li><b>UbD & Pembelajaran Terdiferensiasi:</b> Menyesuaikan gaya & kesiapan belajar.</li>
                        <li><b>TaRL & Asesmen Formatif:</b> Memantau progres belajar siswa secara *real-time*.</li>
                        <li><b>Classroom Management:</b> Pendekatan afektif-komunikatif untuk iklim kondusif.</li>
                    </ul>
                </div>

                <div class="indicator-card bg-white p-5 rounded-xl border-l-4 border-purple-500 shadow-sm">
                    <div class="flex items-center gap-2 text-purple-600 font-bold mb-2">
                        <i class="fa-solid fa-arrows-rotate"></i>
                        <h3>Change (Perubahan Diri)</h3>
                    </div>
                    <p class="text-sm text-slate-700 leading-relaxed">
                        Lebih cermat menyusun pemetaan asesmen diagnostik awal, mengintegrasikan media interaktif berbasis teknologi, serta meningkatkan rutinitas refleksi diri pasca-mengajar.
                    </p>
                </div>
            </div>

            <div class="bg-slate-900 text-white p-6 rounded-xl shadow-sm">
                <h3 class="text-lg font-bold mb-3 flex items-center gap-2 text-brand-500">
                    <i class="fa-solid fa-folder-open"></i> Analisis Artefak Pembelajaran
                </h3>
                <div class="space-y-3 text-sm text-slate-300">
                    <div>
                        <span class="font-semibold text-white">Artefak Dipilih:</span>
                        <p class="mt-0.5">Modul Ajar/RPP Revisi, LKPD Terdiferensiasi, Dokumen Foto/Video Praktik Pembelajaran, serta Lembar Evaluasi & Umpan Balik Siswa SMPN 4 Ciamis.</p>
                    </div>
                    <div>
                        <span class="font-semibold text-white">Alasan Pemilihan:</span>
                        <p class="mt-0.5">Mewakili siklus lengkap: perencanaan, pelaksanaan, asesmen, hingga evaluasi pembelajaran nyata di sekolah.</p>
                    </div>
                    <div>
                        <span class="font-semibold text-white">Bagian Pendukung Refleksi:</span>
                        <p class="mt-0.5">Catatan revisi Modul Ajar (tantangan adaptasi), variasi tugas LKPD (penerapan diferensiasi), dan lembar umpan balik siswa (bukti perubahan efektivitas mengajar).</p>
                    </div>
                </div>
            </div>
        </div>

        <!-- 4. Projek Kepemimpinan -->
        <div id="panel-pkp" class="course-panel hidden space-y-6">
            <div class="bg-white rounded-xl p-6 border border-slate-200 shadow-sm">
                <span class="bg-emerald-100 text-emerald-800 text-xs font-semibold px-2.5 py-0.5 rounded">Mata Kuliah 4</span>
                <h2 class="text-2xl font-bold text-slate-900 mt-1">Projek Kepemimpinan</h2>
                <p class="text-sm text-slate-600 mt-1">Inovasi Program "GASPOL" (Invitasi Olahraga Tradisional) & Penguatan Karakter Pemuda.</p>
            </div>

            <div class="grid md:grid-cols-2 gap-4">
                <div class="indicator-card bg-white p-5 rounded-xl border-l-4 border-blue-500 shadow-sm">
                    <div class="flex items-center gap-2 text-blue-600 font-bold mb-2">
                        <i class="fa-solid fa-link"></i>
                        <h3>Connection (Keterkaitan)</h3>
                    </div>
                    <p class="text-sm text-slate-700 leading-relaxed">
                        Guru PJOK berperan sebagai *agent of change* dan pemimpin pembelajaran. Melalui projek "GASPOL", dirancang kegiatan yang mengaitkan pelestarian budaya lokal, pembentukan karakter (sportivitas, kepemimpinan), dan kesehatan fisik siswa.
                    </p>
                </div>

                <div class="indicator-card bg-white p-5 rounded-xl border-l-4 border-amber-500 shadow-sm">
                    <div class="flex items-center gap-2 text-amber-600 font-bold mb-2">
                        <i class="fa-solid fa-triangle-exclamation"></i>
                        <h3>Challenge (Tantangan & Perbedaan)</h3>
                    </div>
                    <p class="text-sm text-slate-700 leading-relaxed">
                        Mengubah kebiasaan perencanaan spontan menjadi berbasis kerangka terukur: Penerapan SMART Goals, pengaitan aksi lokal dengan target global SDGs (SDG 3, 4, 12/17), serta pentingnya *Positive Self-Talk* & *Growth Mindset*.
                    </p>
                </div>

                <div class="indicator-card bg-white p-5 rounded-xl border-l-4 border-emerald-500 shadow-sm">
                    <div class="flex items-center gap-2 text-emerald-600 font-bold mb-2">
                        <i class="fa-solid fa-brain"></i>
                        <h3>Concept (Konsep Utama)</h3>
                    </div>
                    <ul class="text-sm text-slate-700 list-disc list-inside space-y-1">
                        <li><b>Mind Mapping & Proposal GASPOL:</b> Pemetaan tujuan, target, & indikator keberhasilan.</li>
                        <li><b>SMART Goals:</b> Specific, Measurable, Achievable, Relevant, Time-bound (1 bulan).</li>
                        <li><b>Keterhubungan SDGs & Growth Mindset:</b> Sinergi aksi lokal dengan visi PBB 2030.</li>
                    </ul>
                </div>

                <div class="indicator-card bg-white p-5 rounded-xl border-l-4 border-purple-500 shadow-sm">
                    <div class="flex items-center gap-2 text-purple-600 font-bold mb-2">
                        <i class="fa-solid fa-arrows-rotate"></i>
                        <h3>Change (Perubahan Diri)</h3>
                    </div>
                    <p class="text-sm text-slate-700 leading-relaxed">
                        Menerapkan SMART Goals dalam setiap program ekstrakurikuler/PJOK, konsisten mengintegrasikan permainan tradisional, serta mempraktikkan penguatan positif (*positive self-talk*) dalam memimpin tim.
                    </p>
                </div>
            </div>

            <div class="bg-slate-900 text-white p-6 rounded-xl shadow-sm">
                <h3 class="text-lg font-bold mb-3 flex items-center gap-2 text-brand-500">
                    <i class="fa-solid fa-folder-open"></i> Analisis Artefak Pembelajaran
                </h3>
                <div class="space-y-3 text-sm text-slate-300">
                    <div>
                        <span class="font-semibold text-white">Artefak Dipilih:</span>
                        <p class="mt-0.5">Mind Map Projek "GASPOL" (Gobak Sodor, Boy-boyan, Bakiak, Tarik Tambang), Lembar SMART Goals, dan Bahan Bacaan Reflektif SDGs & Self-Motivation.</p>
                    </div>
                    <div>
                        <span class="font-semibold text-white">Alasan Pemilihan:</span>
                        <p class="mt-0.5">Menunjukkan transformasi ide kepemimpinan menjadi rencana aksi nyata yang sistematis, terukur, dan berorientasi nilai global.</p>
                    </div>
                    <div>
                        <span class="font-semibold text-white">Bagian Pendukung Refleksi:</span>
                        <p class="mt-0.5">Rumusan target terukur (*Measurable*: min. 10 perwakilan dari 3 SMA), tenggat waktu (*Time-Bound*: 1 bulan), serta pengaitan aksi lokal dengan SDG 12 & teknik *positive self-talk*.</p>
                    </div>
                </div>
            </div>
        </div>

        <!-- 5. Design Thinking -->
        <div id="panel-dt" class="course-panel hidden space-y-6">
            <div class="bg-white rounded-xl p-6 border border-slate-200 shadow-sm">
                <span class="bg-emerald-100 text-emerald-800 text-xs font-semibold px-2.5 py-0.5 rounded">Mata Kuliah 5</span>
                <h2 class="text-2xl font-bold text-slate-900 mt-1">Design Thinking</h2>
                <p class="text-sm text-slate-600 mt-1">Pendekatan *Human-Centered* dalam Memecahkan Masalah Pembelajaran PJOK.</p>
            </div>

            <div class="grid md:grid-cols-2 gap-4">
                <div class="indicator-card bg-white p-5 rounded-xl border-l-4 border-blue-500 shadow-sm">
                    <div class="flex items-center gap-2 text-blue-600 font-bold mb-2">
                        <i class="fa-solid fa-link"></i>
                        <h3>Connection (Keterkaitan)</h3>
                    </div>
                    <p class="text-sm text-slate-700 leading-relaxed">
                        Design Thinking memandu guru merancang pembelajaran jasmani yang humanis dan inklusif. Guru tidak hanya mengajarkan gerakan fisik, tetapi memahami ketakutan dan hambatan psikis murid (takut kena bola, takut jatuh).
                    </p>
                </div>

                <div class="indicator-card bg-white p-5 rounded-xl border-l-4 border-amber-500 shadow-sm">
                    <div class="flex items-center gap-2 text-amber-600 font-bold mb-2">
                        <i class="fa-solid fa-triangle-exclamation"></i>
                        <h3>Challenge (Tantangan & Perbedaan)</h3>
                    </div>
                    <p class="text-sm text-slate-700 leading-relaxed">
                        Mengubah pola pikir konvensional yang kaku menjadi pendekatan *user-centered*. Menggunakan siklus iterasi (perbaikan berulang), memandang kegagalan sebagai peluang belajar, serta melakukan eksperimen prototipe cepat.
                    </p>
                </div>

                <div class="indicator-card bg-white p-5 rounded-xl border-l-4 border-emerald-500 shadow-sm">
                    <div class="flex items-center gap-2 text-emerald-600 font-bold mb-2">
                        <i class="fa-solid fa-brain"></i>
                        <h3>Concept (Konsep Utama)</h3>
                    </div>
                    <ul class="text-sm text-slate-700 list-disc list-inside space-y-1">
                        <li><b>5 Tahap d.school:</b> Empathize, Define (HMW), Ideate, Prototype, & Test/Evaluate.</li>
                        <li><b>3 Ruang Inovasi (Tim Brown):</b> Inspirasi, Ideasi, dan Implementasi.</li>
                        <li><b>Scientific vs Design Thinking:</b> Pembuktian hipotesis vs Penciptaan solusi inovatif baru.</li>
                    </ul>
                </div>

                <div class="indicator-card bg-white p-5 rounded-xl border-l-4 border-purple-500 shadow-sm">
                    <div class="flex items-center gap-2 text-purple-600 font-bold mb-2">
                        <i class="fa-solid fa-arrows-rotate"></i>
                        <h3>Change (Perubahan Diri)</h3>
                    </div>
                    <p class="text-sm text-slate-700 leading-relaxed">
                        Mengidentifikasi hambatan murid dengan empati sebelum menyusun Modul Ajar, memodifikasi media/alat (bola busa, net rendah), serta rutin melakukan tes & iterasi berdasarkan umpan balik jujur dari murid.
                    </p>
                </div>
            </div>

            <div class="bg-slate-900 text-white p-6 rounded-xl shadow-sm">
                <h3 class="text-lg font-bold mb-3 flex items-center gap-2 text-brand-500">
                    <i class="fa-solid fa-folder-open"></i> Analisis Artefak Pembelajaran
                </h3>
                <div class="space-y-3 text-sm text-slate-300">
                    <div>
                        <span class="font-semibold text-white">Artefak Dipilih:</span>
                        <p class="mt-0.5">LK 1.3 (Pemetaan Kompetensi Guru), Infografis Kelompok 2 (NotebookLM - Inovasi PJOK), dan Lembar Aktivitas Refleksi Tabel 1.9 (Passing Bola Voli).</p>
                    </div>
                    <div>
                        <span class="font-semibold text-white">Alasan Pemilihan:</span>
                        <p class="mt-0.5">Menunjukkan alur belajar berkesinambungan: dari konsep empati (LK 1.3), rancangan visual inovasi kelompok, hingga aplikasi prototipe nyata dalam passing bola voli.</p>
                    </div>
                    <div>
                        <span class="font-semibold text-white">Bagian Pendukung Refleksi:</span>
                        <p class="mt-0.5">Adaptasi strategi penggunaan bola busa/plastik & net rendah untuk siswa yang kurang percaya diri serta komitmen menyusun Modul Ajar berdiferensiasi.</p>
                    </div>
                </div>
            </div>
        </div>

    </main>

    <!-- Footer -->
    <footer class="bg-slate-900 text-slate-400 py-6 text-center text-xs border-t border-slate-800">
        <p>© 2026 Portofolio Digital Refleksi PPG Penjas - Bayu Rahayu (NIM: 2186250029)</p>
        <p class="mt-1 text-slate-500">Dioptimalkan untuk Presentasi Refleksi Pembelajaran Semester 2</p>
    </footer>

    <script>
        function switchTab(tabId) {
            // Hide all panels
            const panels = document.querySelectorAll('.course-panel');
            panels.forEach(panel => panel.classList.add('hidden'));

            // Reset active button styling
            const buttons = document.querySelectorAll('.tab-btn');
            buttons.forEach(btn => {
                btn.classList.remove('active');
                btn.classList.add('bg-white', 'text-slate-700');
            });

            // Show selected panel
            const selectedPanel = document.getElementById('panel-' + tabId);
            if (selectedPanel) {
                selectedPanel.classList.remove('hidden');
            }

            // Set active button
            const selectedTab = document.getElementById('tab-' + tabId);
            if (selectedTab) {
                selectedTab.classList.add('active');
                selectedTab.classList.remove('bg-white', 'text-slate-700');
            }
        }
    </script>
</body>
</html>
