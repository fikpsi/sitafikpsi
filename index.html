<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no, viewport-fit=cover">
    <meta http-equiv="X-Content-Type-Options" content="nosniff">
    <title>Sistem Informasi Tugas Akhir FIKPsi</title>
    
    <script crossorigin src="https://unpkg.com/react@18/umd/react.production.min.js"></script>
    <script crossorigin src="https://unpkg.com/react-dom@18/umd/react-dom.production.min.js"></script>
    <script src="https://unpkg.com/@babel/standalone/babel.min.js"></script>
    <script src="https://cdn.tailwindcss.com"></script>
    <script src="https://cdn.sheetjs.com/xlsx-latest/package/dist/xlsx.full.min.js"></script>
    <script src="https://cdn.jsdelivr.net/npm/marked/marked.min.js"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/dompurify/3.0.6/purify.min.js"></script>
    
    <link href="https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:wght@300;400;500;600;700;800&display=swap" rel="stylesheet">
    
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    fontFamily: { sans: ['"Plus Jakarta Sans"', 'sans-serif'] },
                    animation: { 
                        'fade-in': 'fadeIn 0.5s cubic-bezier(0.4, 0, 0.2, 1)', 
                        'slide-up': 'slideUp 0.6s cubic-bezier(0.4, 0, 0.2, 1)',
                        'pop-in': 'popIn 0.6s cubic-bezier(0.175, 0.885, 0.32, 1.275) forwards',
                        'blob': 'blob 10s infinite',
                        'pulse-slow': 'pulse 3s infinite',
                        'bounce-slight': 'bounceSlight 2s infinite'
                    },
                    keyframes: {
                        fadeIn: { '0%': { opacity: '0' }, '100%': { opacity: '1' } },
                        slideUp: { '0%': { opacity: '0', transform: 'translateY(20px)' }, '100%': { opacity: '1', transform: 'translateY(0)' } },
                        popIn: { '0%': { opacity: '0', transform: 'scale(0.5)' }, '100%': { opacity: '1', transform: 'scale(1)' } },
                        blob: {
                            "0%": { transform: "translate(0px, 0px) scale(1)" },
                            "33%": { transform: "translate(30px, -50px) scale(1.1)" },
                            "66%": { transform: "translate(-20px, 20px) scale(0.9)" },
                            "100%": { transform: "translate(0px, 0px) scale(1)" }
                        },
                        bounceSlight: {
                            "0%, 100%": { transform: "translateY(-3%)" },
                            "50%": { transform: "translateY(0)" }
                        }
                    },
                    colors: {
                        glass: {
                            100: 'rgba(255, 255, 255, 0.1)',
                            200: 'rgba(255, 255, 255, 0.2)',
                            300: 'rgba(255, 255, 255, 0.4)',
                            border: 'rgba(255, 255, 255, 0.5)',
                        }
                    }
                }
            }
        }
    </script>
    
    <style>
        body { 
            background-color: #f3e8ff; /* Light Purple Bg */
            -webkit-font-smoothing: antialiased; 
            overflow: hidden; 
            color: #4c1d95; /* Deep Purple Text */
        }
        
        /* Background Blobs for Glass Effect */
        .blob-cont {
            position: fixed; top: 0; left: 0; width: 100vw; height: 100vh; z-index: -1; overflow: hidden; pointer-events: none;
        }
        .blob {
            position: absolute; border-radius: 50%; filter: blur(80px); opacity: 0.6; animation: blob 10s infinite alternate;
        }
        .blob-1 { top: -10%; left: -10%; width: 600px; height: 600px; background: #c084fc; animation-delay: 0s; }
        .blob-2 { bottom: -10%; right: -10%; width: 600px; height: 600px; background: #818cf8; animation-delay: 2s; }
        .blob-3 { top: 30%; left: 30%; width: 500px; height: 500px; background: #f472b6; animation-delay: 4s; opacity: 0.4; }

        /* Enhanced Glassmorphism */
        .glass { 
            background: rgba(255, 255, 255, 0.65); 
            backdrop-filter: blur(20px); -webkit-backdrop-filter: blur(20px);
            border: 1px solid rgba(255, 255, 255, 0.8); 
            box-shadow: 0 8px 32px 0 rgba(31, 38, 135, 0.1);
        }
        
        .glass-dark {
            background: rgba(76, 29, 149, 0.05);
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255,255,255,0.3);
        }
        
        .touch-scroll { -webkit-overflow-scrolling: touch; }
        
        /* Custom Scrollbar */
        .custom-scrollbar::-webkit-scrollbar { width: 6px; height: 6px; }
        .custom-scrollbar::-webkit-scrollbar-track { background: transparent; }
        .custom-scrollbar::-webkit-scrollbar-thumb { background: rgba(168, 85, 247, 0.3); border-radius: 10px; }
        .custom-scrollbar::-webkit-scrollbar-thumb:hover { background: rgba(168, 85, 247, 0.6); }
        
        .input-modern { 
            width: 100%; padding: 0.75rem 1rem; border-radius: 1rem; 
            background-color: rgba(255, 255, 255, 0.7); 
            border: 1px solid rgba(255, 255, 255, 0.9); 
            outline: none; color: #4c1d95; transition: all 0.2s;
            backdrop-filter: blur(4px);
        }
        .input-modern:focus { 
            background-color: rgba(255, 255, 255, 1);
            border-color: #a855f7; 
            box-shadow: 0 0 0 4px rgba(168, 85, 247, 0.15); 
            transform: translateY(-1px);
        }

        .textarea-modern {
            width: 100%; padding: 0.75rem 1rem; border-radius: 1rem; 
            background-color: rgba(255, 255, 255, 0.7); 
            border: 1px solid rgba(255, 255, 255, 0.9); 
            outline: none; color: #4c1d95; transition: all 0.2s;
            backdrop-filter: blur(4px);
            min-height: 100px;
            resize: vertical;
        }
        .textarea-modern:focus { 
            background-color: rgba(255, 255, 255, 1);
            border-color: #a855f7; 
            box-shadow: 0 0 0 4px rgba(168, 85, 247, 0.15); 
            transform: translateY(-1px);
        }

        /* Typing Indicator Animation */
        .typing-dot {
            animation: typing 1.4s infinite ease-in-out both;
        }
        .typing-dot:nth-child(1) { animation-delay: -0.32s; }
        .typing-dot:nth-child(2) { animation-delay: -0.16s; }
        @keyframes typing {
            0%, 80%, 100% { transform: scale(0); }
            40% { transform: scale(1); }
        }
        
        /* Live Indicator */
        .live-indicator {
            width: 8px; height: 8px; background-color: #22c55e; border-radius: 50%;
            box-shadow: 0 0 0 0 rgba(34, 197, 94, 0.7);
            animation: pulse-green 2s infinite;
        }
        @keyframes pulse-green {
            0% { transform: scale(0.95); box-shadow: 0 0 0 0 rgba(34, 197, 94, 0.7); }
            70% { transform: scale(1); box-shadow: 0 0 0 6px rgba(34, 197, 94, 0); }
            100% { transform: scale(0.95); box-shadow: 0 0 0 0 rgba(34, 197, 94, 0); }
        }
    </style>
</head>
<body class="antialiased text-slate-800">
    <div class="blob-cont">
        <div class="blob blob-1"></div>
        <div class="blob blob-2"></div>
        <div class="blob blob-3"></div>
    </div>

    <div id="root"></div>

    <script type="text/babel">
        const { useState, useEffect, useRef, useMemo } = React;

        // --- ICONS (Lucide Style) ---
        const Icon = ({ path, className = "w-5 h-5", size = 20 }) => <svg className={className} width={size} height={size} fill="none" stroke="currentColor" viewBox="0 0 24 24" strokeWidth="2" strokeLinecap="round" strokeLinejoin="round"><path d={path} /></svg>;
        const PATHS = {
            Home: "M3 9l9-7 9 7v11a2 2 0 01-2 2H5a2 2 0 01-2-2z M9 22V12h6v10",
            Sparkles: "M9.937 15.5A2 2 0 008.5 14.063l-6.135-1.582a.5.5 0 010-.962l6.135-1.583A2 2 0 009.937 8.5l1.582-6.135a.5.5 0 01.963 0l1.582 6.135a2 2 0 001.437 1.437l6.135 1.583a.5.5 0 010 .962l-6.135 1.583a2 2 0 00-1.437 1.437l-1.582 6.135a.5.5 0 01-.963 0z",
            Lock: "M12 15v2m-6 4h12a2 2 0 002-2v-6a2 2 0 00-2-2H6a2 2 0 00-2 2v6a2 2 0 002 2zm10-10V7a4 4 0 00-8 0v4h8z",
            Trash: "M19 7l-.867 12.142A2 2 0 0116.138 21H7.862a2 2 0 01-1.995-1.858L5 7m5 4v6m4-6v6m1-10V4a1 1 0 00-1-1h-4a1 1 0 00-1 1v3M4 7h16",
            Plus: "M12 5v14m-7-7h14",
            Search: "M21 21l-6-6m2-5a7 7 0 11-14 0 7 7 0 0114 0z",
            Menu: "M4 6h16M4 12h16M4 18h16",
            Users: "M17 21v-2a4 4 0 00-4-4H5a4 4 0 00-4 4v2M16 3.13a4 4 0 010 7.75",
            User: "M20 21v-2a4 4 0 00-4-4H8a4 4 0 00-4 4v2 M12 11a4 4 0 100-8 4 4 0 000 8z",
            Book: "M4 19.5A2.5 2.5 0 016.5 17H20 M6.5 2H20v20H6.5A2.5 2.5 0 014 19.5v-15A2.5 2.5 0 016.5 2z",
            Chart: "M18 20V10 M12 20V4 M6 20v-6",
            Send: "M22 2L11 13 M22 2l-7 20-4-9-9-4 20-7z",
            Cloud: "M5.5 16a3.5 3.5 0 01-.369-6.98 4 4 0 117.753-1.977A4.5 4.5 0 1113.5 16h-8z",
            Graduation: "M22 10v6M2 10l10-5 10 5-10 5z M6 10l0 .6c0 2.4 2 4.5 5.7 4.9L12 16",
            Cog: "M12 15a3 3 0 100-6 3 3 0 000 6z M19.4 15a1.65 1.65 0 00.33 1.82l.06.06a2 2 0 010 2.83 2 2 0 01-2.83 0l-.06-.06a1.65 1.65 0 00-1.82-.33 1.65 1.65 0 00-1 1.51V21a2 2 0 01-2 2 2 2 0 01-2-2v-.09A1.65 1.65 0 009 19.4a1.65 1.65 0 00-1.82.33l-.06.06a2 2 0 01-2.83 0 2 2 0 010 2.83l.06-.06a1.65 1.65 0 00-.33 1.82V9a1.65 1.65 0 001.51 1H21a2 2 0 012 2 2 2 0 01-2 2h-.09a1.65 1.65 0 00-1.51 1z",
            Download: "M21 15v4a2 2 0 01-2 2H5a2 2 0 01-2-2v-4 M7 10l5 5 5-5 M12 15V3",
            Upload: "M21 15v4a2 2 0 01-2 2H5a2 2 0 01-2-2v-4 M17 8l-5-5-5 5 M12 3v12",
            ChevronDown: "M6 9l6 6 6-6",
            ArrowLeft: "M19 12H5 M12 19l-7-7 7-7",
            FileText: "M14 2H6a2 2 0 00-2 2v16a2 2 0 002 2h12a2 2 0 002-2V8z M14 2v6h6",
            Clip: "M21.44 11.05l-9.19 9.19a6 6 0 01-8.49-8.49l9.19-9.19a4 4 0 015.66 5.66l-9.2 9.19a2 2 0 01-2.83-2.83l8.49-8.48",
            Logout: "M9 21H5a2 2 0 01-2-2V5a2 2 0 012-2h4 M16 17l5-5-5-5 M21 12H9",
            X: "M18 6L6 18M6 6l12 12",
            Eye: "M1 12s4-8 11-8 11 8 11 8-4 8-11 8-11-8-11-8z M12 15a3 3 0 100-6 3 3 0 000 6z",
            ExternalLink: "M18 13v6a2 2 0 01-2 2H5a2 2 0 01-2-2V8a2 2 0 012-2h6 M15 3h6v6 M10 14L21 3",
            Robot: "M12 8V4H8 M16 4h-4 M4 14a2 2 0 012-2h12a2 2 0 01-2 2H6a2 2 0 01-2-2v-6z M10 18h4 M9 13v2 M15 13v2",
            Info: "M13 16h-1v-4h-1m1-4h.01M21 12a9 9 0 11-18 0 9 9 0 0118 0z",
            Sun: "M12 3v1m0 16v1m9-9h-1M4 12H3m15.364 6.364l-.707-.707M6.343 6.343l-.707-.707m12.728 0l-.707.707M6.343 17.657l-.707.707M16 12a4 4 0 11-8 0 4 4 0 018 0z",
            Edit: "M11 4H4a2 2 0 00-2 2v14a2 2 0 002 2h14a2 2 0 002-2V8z",
            FileUp: "M21 15v4a2 2 0 01-2 2H5a2 2 0 01-2-2v-4M17 8l-5-5-5 5M12 3v12",
            Bell: "M15 17h5l-1.405-1.405A2.032 2.032 0 0118 14.158V11a6.002 6.002 0 00-4-5.659V5a2 2 0 10-4 0v.341C7.67 6.165 6 8.388 6 11v3.159c0 .538-.214 1.055-.595 1.436L4 17h5m6 0v1a3 3 0 11-6 0v-1m6 0H9",
            Refresh: "M4 4v5h.582m15.356 2A8.001 8.001 0 004.582 9m0 0H9m11 11v-5h-.581m0 0a8.003 8.003 0 01-15.357-2m15.357 2H15",
            Wifi: "M5 12.55a11 11 0 0114.08 0 M1.42 9a16 16 0 0121.16 0 M8.53 16.11a6 6 0 016.95 0 M12 20h.01",
            Tag: "M7 7h.01M7 3h5c.512 0 1.024.195 1.414.586l7 7a2 2 0 010 2.828l-7 7a2 2 0 01-2.828 0l-7-7A1.994 1.994 0 013 12V7a4 4 0 014-4z",
            Mail: "M3 8l7.89 5.26a2 2 0 002.22 0L21 8M5 19h14a2 2 0 002-2V7a2 2 0 00-2-2H5a2 2 0 00-2 2v10a2 2 0 002 2z",
            Inbox: "M22 12h-6l-2 3h-4l-2-3H2v12h20V12z",
            PaperPlane: "M22 2L11 13M22 2l-7 20-4-9-9-4 20-7z"
        };

        const AUTH_TOKEN = "MTAxMDE5OTA="; 

        // --- DATA ---
        const INITIAL_DB = {
            'Data Dosen': [
                { id: 1, Nama: "Dr. Budi Santoso", NIDN: "112233", Keahlian: "Epidemiologi", Kuota: 10, Terisi: 5 },
                { id: 2, Nama: "Prof. Siti Aminah", NIDN: "445566", Keahlian: "Kesehatan Lingkungan", Kuota: 8, Terisi: 7 },
                { id: 3, Nama: "Rudi Hermawan, M.Kes", NIDN: "778899", Keahlian: "Promosi Kesehatan", Kuota: 12, Terisi: 3 }
            ],
            'Data Peminatan': [
                { id: 1, Nama: "PKIP" },
                { id: 2, Nama: "KESLING" },
                { id: 3, Nama: "KESPRO" },
                { id: 4, Nama: "EPID" },
                { id: 5, Nama: "GIZI KESMAS" },
                { id: 6, Nama: "K3" }
            ],
            'Mahasiswa Tugas Akhir': [
                { id: 1, Nama: "Ahmad Dani", NPM: "2020001", Prodi: "S1 Ilmu Kesehatan Masyarakat", Angkatan: "2020", Peminatan: "EPID", WhatsApp: "08123456789", Judul: "Analisis Faktor Risiko DBD", Pembimbing_1: "Dr. Budi Santoso", Pembimbing_2: "Rudi Hermawan, M.Kes", Penguji: "Prof. Siti Aminah", Status: "Sudah Hasil", StatusAkademik: "Aktif", BimbinganCount: 5, ProgresDeskripsi: "Sudah revisi bab 4", LinkLaporan: "https://drive.google.com/..." },
                { id: 2, Nama: "Rina Wati", NPM: "2020002", Prodi: "S1 Ilmu Kesehatan Masyarakat", Angkatan: "2020", Peminatan: "KESLING", WhatsApp: "08987654321", Judul: "Higiene Sanitasi Makanan Jajanan", Pembimbing_1: "Prof. Siti Aminah", Pembimbing_2: "-", Penguji: "Dr. Budi Santoso", Status: "Sudah Proposal", StatusAkademik: "Aktif", BimbinganCount: 2, ProgresDeskripsi: "Persiapan turun lapangan", LinkLaporan: "" },
                { id: 3, Nama: "Budi Setiawan", NPM: "2020003", Prodi: "S1 Psikologi", Angkatan: "2020", Peminatan: "Psikologi Industri", WhatsApp: "08123456700", Judul: "Pengaruh Work From Home Terhadap Kinerja", Pembimbing_1: "Rudi Hermawan, M.Kes", Pembimbing_2: "-", Penguji: "-", Status: "Belum Proposal", StatusAkademik: "Cuti", BimbinganCount: 0, ProgresDeskripsi: "-", LinkLaporan: "" },
                { id: 4, Nama: "Siska Amelia", NPM: "2017001", Prodi: "S1 Psikologi", Angkatan: "2017", Peminatan: "Psikologi Klinis", WhatsApp: "08129999888", Judul: "Depresi pada Mahasiswa Tingkat Akhir", Pembimbing_1: "Rudi Hermawan, M.Kes", Pembimbing_2: "-", Penguji: "-", Status: "Belum Proposal", StatusAkademik: "Limit DO", BimbinganCount: 0, ProgresDeskripsi: "-", LinkLaporan: "" }
            ],
            'Jadwal Ujian TA': [
                { id: 1, Mahasiswa: "Rina Wati", Jenis: "Seminar Proposal", Tanggal: "2024-12-15", Jam: "09:00", Ruang: "R. Sidang 1", Penguji_1: "Dr. Budi Santoso" }
            ],
            'Data Unduhan': [
                { id: 1, Judul: "Pedoman Penulisan Skripsi 2024", Kategori: "Pedoman", Link: "#" },
                { id: 2, Judul: "Template Proposal Penelitian", Kategori: "Template", Link: "#" }
            ],
            'Informasi': [
                { id: 1, Judul: "Jadwal Libur Semester", Isi: "Libur dimulai tanggal 25 Desember hingga 5 Januari.", Penulis: "Admin", Tanggal: "2024-12-20", Tipe: "Umum" }
            ],
            'Pesan': [
                { id: 1, sender: "Dr. Budi Santoso", receiver: "Ahmad Dani", subject: "Revisi Bab 1", content: "Mohon perbaiki latar belakang masalah sesuai catatan saya.", timestamp: new Date().toISOString(), isRead: false }
            ],
            'Pengajuan Judul': [],
            'Pendaftaran Sempro': [],
            'Pendaftaran Semhas': [],
            'Pendaftaran Sidang': [],
            'Layanan Surat': [
                { id: 1, Nama: "Ahmad Dani", NPM: "2020001", Jenis_Surat: "Surat Izin Penelitian", Tujuan: "Dinkes Kota Pontianak", Tanggal: "2024-12-01", Status: "Selesai" }
            ],
            'Laporan TA': [], 
            'Data Yudisium': [],
            'Konfigurasi': [
                { id: 1, app_name: 'SI Tugas Akhir FIKPsi', logo_url: "", ai_api_key: "", 
                  gform_pengajuan_judul: "", gform_sempro: "", gform_semhas: "", gform_sidang: "", gform_surat: "", gform_yudisium: "", gform_laporan_ta: ""
                }
            ]
        };

        const TABLE_CONFIG = {
            'Data Dosen': { 
                columns: [{key:'Nama', label:'Nama Lengkap'}, {key:'NIDN', label:'NIDN'}, {key:'Keahlian', label:'Bidang Keahlian'}, {key:'Kuota', label:'Kuota'}, {key:'Terisi', label:'Aktif'}], 
                form: [{key:'Nama', label:'Nama Lengkap'}, {key:'NIDN', label:'NIDN'}, {key:'Keahlian', label:'Keahlian'}, {key:'Kuota', label:'Kuota Maksimal', type:'number'}, {key:'Terisi', label:'Jumlah Bimbingan Saat Ini', type:'number'}]
            },
            'Data Peminatan': {
                columns: [{key: 'Nama', label: 'Nama Peminatan'}],
                form: [{key: 'Nama', label: 'Nama Peminatan'}]
            },
            'Mahasiswa Tugas Akhir': { 
                columns: [
                    {key:'Nama', label:'Nama'}, 
                    {key:'NPM', label:'NPM'}, 
                    {key:'Prodi', label:'Program Studi'}, 
                    {key:'StatusAkademik', label:'Status Akademik', render: (v) => (
                        <span className={`px-3 py-1 rounded-full text-xs font-bold ${
                            v === 'Aktif' ? 'bg-emerald-100 text-emerald-700' :
                            v === 'Cuti' ? 'bg-yellow-100 text-yellow-700' :
                            v === 'Limit DO' ? 'bg-red-100 text-red-700' :
                            'bg-gray-100 text-gray-700'
                        }`}>{v || 'Aktif'}</span>
                    )},
                    {key:'Pembimbing_1', label:'Pembimbing 1'}, 
                    {key:'Pembimbing_2', label:'Pembimbing 2'},
                    {key:'Status', label:'Tahapan', render: (v) => (
                        <span className={`px-3 py-1 rounded-full text-xs font-bold ${
                            v === 'Lulus' ? 'bg-green-100 text-green-700' :
                            v === 'Sudah Sidang' ? 'bg-blue-100 text-blue-700' :
                            v === 'Sudah Hasil' ? 'bg-pink-100 text-pink-700' :
                            v === 'Sudah Proposal' ? 'bg-orange-100 text-orange-700' :
                            'bg-gray-100 text-gray-600'
                        }`}>{v}</span>
                    )},
                    {key:'BimbinganCount', label:'Bimbingan (x)', render: (v) => <span className="font-mono font-bold text-purple-700 bg-purple-100 px-2 py-0.5 rounded">{v || 0}</span>},
                    {key:'ProgresDeskripsi', label:'Ket. Progres', render: (v) => <span className="text-xs text-gray-600 italic truncate max-w-[150px] block">{v ? (v.length > 25 ? v.substring(0,25)+'...' : v) : '-'}</span>}
                ], 
                form: [] // Dynamically generated in App component
            },
            // NEW: Config specifically for the Dosen View "Tugas Akhir Mahasiswa"
            'Tugas Akhir Mahasiswa (Dosen)': {
                columns: [
                    {key:'Nama', label:'Nama'}, 
                    {key:'NPM', label:'NPM'}, 
                    {key:'Judul', label:'Judul'},
                    {key:'Status', label:'Tahapan', render: (v) => (
                        <span className={`px-2 py-1 rounded text-xs font-bold ${
                            v === 'Lulus' ? 'bg-green-100 text-green-700' :
                            v === 'Sudah Sidang' ? 'bg-blue-100 text-blue-700' :
                            v === 'Sudah Hasil' ? 'bg-pink-100 text-pink-700' :
                            v === 'Sudah Proposal' ? 'bg-orange-100 text-orange-700' :
                            'bg-gray-100 text-gray-600'
                        }`}>{v}</span>
                    )},
                    {key:'LinkLaporan', label:'Link Laporan', render: (v) => v ? <a href={v} target="_blank" className="text-blue-600 hover:underline flex items-center gap-1 font-bold text-xs"><Icon path={PATHS.ExternalLink} size={14}/> Buka Laporan</a> : <span className="text-gray-300 italic text-xs">Belum ada</span>}
                ],
                form: [] // Read only for Dosen mostly
            },
            'Jadwal Ujian TA': {
                columns: [
                    {key:'Mahasiswa', label:'Mahasiswa'}, 
                    {key:'Jenis', label:'Jenis'}, 
                    {key:'Tanggal', label:'Tanggal', render: (v) => {
                        if (!v) return '-';
                        try {
                            const date = new Date(v);
                            // Cek validitas tanggal
                            if (isNaN(date.getTime())) return v;
                            return date.toLocaleDateString('id-ID', { weekday: 'long', year: 'numeric', month: 'long', day: 'numeric' });
                        } catch (e) { return v; }
                    }}, 
                    {key:'Jam', label:'Jam'}, 
                    {key:'Ruang', label:'Ruang'}
                ],
                form: [{key:'Mahasiswa', label:'Nama Mahasiswa'}, {key:'Jenis', label:'Jenis Ujian', type: 'select', options:[{value:'Seminar Proposal', label:'Sempro'}, {value:'Seminar Hasil', label:'Semhas'}, {value:'Sidang', label:'Sidang'}]}, {key:'Tanggal', label:'Tanggal', type:'date'}, {key:'Jam', label:'Jam'}, {key:'Ruang', label:'Ruangan'}]
            },
            'Data Unduhan': {
                columns: [
                    {key:'Judul', label:'Nama Berkas'},
                    {key:'Kategori', label:'Kategori'},
                    {key:'Link', label:'Link', render: (v) => <a href={v} target="_blank" className="bg-green-100 text-green-700 px-3 py-1 rounded-lg text-xs font-bold hover:bg-green-200 transition flex items-center w-fit gap-1"><Icon path={PATHS.Download} size={14}/> Unduh</a>}
                ],
                form: [
                    {key:'Judul', label:'Nama Dokumen'},
                    {key:'Kategori', label:'Kategori', type: 'select', options:[{value:'Pedoman', label:'Pedoman'}, {value:'Template', label:'Template'}, {value:'SK', label:'SK'}, {value:'Materi', label:'Materi'}]},
                    {key:'Link', label:'Link Download (Google Drive)', placeholder: 'https://...'}
                ]
            },
            'Informasi': {
                columns: [
                    {key:'Judul', label:'Judul'}, 
                    {key:'Penulis', label:'Oleh'}, 
                    {key:'Tanggal', label:'Tanggal', render: (v) => {
                         try {
                             return new Date(v).toLocaleDateString('id-ID', { weekday: 'long', year: 'numeric', month: 'long', day: 'numeric' });
                         } catch (e) { return v; }
                    }}, 
                    {key:'Tipe', label:'Kategori', render: (v) => (
                        <span className={`px-2 py-1 rounded text-xs font-bold ${
                            v === 'Jadwal' ? 'bg-blue-100 text-blue-700' :
                            v === 'Akademik' ? 'bg-purple-100 text-purple-700' :
                            'bg-gray-100 text-gray-700'
                        }`}>{v}</span>
                    )}
                ],
                form: [
                    {key:'Judul', label:'Judul Pengumuman'},
                    {key:'Isi', label:'Isi Pengumuman', type: 'textarea'},
                    {key:'Tipe', label:'Kategori', type: 'select', options:[{value:'Umum', label:'Umum'}, {value:'Akademik', label:'Akademik'}, {value:'Jadwal', label:'Jadwal'}]},
                    {key:'Tanggal', label:'Tanggal', type:'date'}
                ]
            },
            'Pengajuan Judul': {
                columns: [{key:'Nama', label:'Nama'}, {key:'NPM', label:'NPM'}, {key:'Judul', label:'Usulan Judul'}, {key:'Peminatan', label:'Peminatan'}],
                form: [
                    {key:'Nama', label:'Nama Lengkap'},
                    {key:'NPM', label:'NPM'},
                    {key:'Peminatan', label:'Peminatan', type: 'select', options:[]}, // Options will be populated dynamically
                    {key:'Judul', label:'Usulan Judul Penelitian'},
                    {key:'Masalah', label:'Rumusan Masalah Singkat', type:'text'}
                ]
            },
            'Pendaftaran Sempro': { columns: [{key:'Nama',label:'Nama'},{key:'Judul',label:'Judul'}], form: [{key:'Nama',label:'Nama'},{key:'Judul',label:'Judul'}]},
            'Pendaftaran Semhas': { columns: [{key:'Nama',label:'Nama'},{key:'Judul',label:'Judul'}], form: [{key:'Nama',label:'Nama'},{key:'Judul',label:'Judul'}]},
            'Pendaftaran Sidang': { columns: [{key:'Nama',label:'Nama'},{key:'Judul',label:'Judul'}], form: [{key:'Nama',label:'Nama'},{key:'Judul',label:'Judul'}]},
            'Layanan Surat': { columns: [{key:'Nama',label:'Nama'},{key:'Jenis_Surat',label:'Jenis'},{key:'Status',label:'Status'}], form: [{key:'Nama',label:'Nama'},{key:'Jenis_Surat',label:'Jenis'},{key:'Status',label:'Status',type:'select',options:[{value:'Diproses',label:'Diproses'},{value:'Selesai',label:'Selesai'}]}]},
            'Data Yudisium': { columns: [{key:'Nama',label:'Nama'},{key:'IPK',label:'IPK'}], form: [{key:'Nama',label:'Nama'},{key:'IPK',label:'IPK'}]},
            'Laporan TA': { // NEW: Table config for Laporan TA
                columns: [{key:'Nama', label:'Nama'}, {key:'NPM', label:'NPM'}, {key:'Judul', label:'Judul Laporan'}, {key:'Link', label:'Link Dokumen', render: (v) => <a href={v} target="_blank" className="text-blue-600 hover:underline flex items-center gap-1"><Icon path={PATHS.ExternalLink} size={14}/> Buka</a>}],
                form: [{key:'Nama', label:'Nama'}, {key:'NPM', label:'NPM'}, {key:'Judul', label:'Judul Laporan'}, {key:'Link', label:'Link Dokumen (G Drive)'}]
            }
        };

        // ... (useStickyState and useDatabase are the same)
        const useStickyState = (defaultValue, key) => {
            const [value, setValue] = useState(() => {
                try { return JSON.parse(window.localStorage.getItem(key)) || defaultValue; } catch { return defaultValue; }
            });
            useEffect(() => { window.localStorage.setItem(key, JSON.stringify(value)); }, [key, value]);
            return [value, setValue];
        };

        const useDatabase = (initialData, scriptUrl) => {
            const [localData, setLocalData] = useStickyState(initialData, 'sim_tugasakhir_db_v5_FIX'); 
            const [isOnline, setIsOnline] = useState(false);
            const [isLoading, setIsLoading] = useState(false);
            const [isBackgroundSyncing, setIsBackgroundSyncing] = useState(false);
            const [lastSyncTime, setLastSyncTime] = useState(null);

            // Sync Data Function (Updated to handle background sync)
            const syncData = async (url, isBackground = false) => {
                if (!url) return;
                
                if (isBackground) {
                    setIsBackgroundSyncing(true);
                } else {
                    setIsLoading(true);
                }

                try {
                    const res = await fetch(`${url}?action=read`, {
                        method: 'GET',
                        redirect: 'follow'
                    });
                    
                    if (res.ok) {
                        const cloudData = await res.json();
                        if (!cloudData.error) {
                            setLocalData(prev => ({...prev, ...cloudData}));
                            setIsOnline(true);
                            setLastSyncTime(new Date());
                        }
                    } else {
                        console.warn("Cloud read failed with status:", res.status);
                        setIsOnline(false);
                    }
                } catch (e) { 
                    console.warn("Sync Mode: Offline (Network Error/CORS)", e); 
                    setIsOnline(false);
                } finally {
                    if (isBackground) {
                        setIsBackgroundSyncing(false);
                    } else {
                        setIsLoading(false);
                    }
                }
            };

            // AUTO SYNC EFFECT (Polling every 10 seconds)
            useEffect(() => {
                if (scriptUrl && scriptUrl.startsWith('https://script.google.com')) {
                    // Initial load
                    syncData(scriptUrl, false);

                    // Polling interval
                    const intervalId = setInterval(() => {
                        syncData(scriptUrl, true); // true indicates background sync
                    }, 10000); // 10000ms = 10 seconds

                    return () => clearInterval(intervalId);
                } else {
                    setIsOnline(false);
                }
            }, [scriptUrl]);

            const sendToCloud = async (action, collection, data) => {
                if(!scriptUrl) return;
                setIsBackgroundSyncing(true); // Show indicator while saving
                try {
                    await fetch(scriptUrl, {
                        method: 'POST',
                        mode: 'no-cors', 
                        headers: { 'Content-Type': 'application/json' },
                        body: JSON.stringify({ action, collection, data })
                    });
                    console.log(`Cloud update sent: ${action} on ${collection}`);
                } catch(e) {
                    console.error("Cloud Sync Error (ignored in UI):", e);
                } finally {
                    setIsBackgroundSyncing(false);
                }
            };

            const crud = {
                add: (key, item) => {
                    const newItem = { id: Date.now(), ...item };
                    setLocalData(p => ({...p, [key]: [...(p[key]||[]), newItem]}));
                    sendToCloud('create', key, newItem);
                },
                del: (key, id) => {
                    setLocalData(p => ({...p, [key]: p[key].filter(x => x.id !== id)}));
                    sendToCloud('delete', key, { id });
                },
                update: (key, id, newItem) => {
                    setLocalData(p => ({...p, [key]: p[key].map(x => x.id === id ? {...x, ...newItem} : x)}));
                    sendToCloud('update', key, { id, ...newItem });
                },
                importBatch: (key, items) => {
                    const newItems = items.map(i => ({ id: Date.now() + Math.random(), ...i }));
                    setLocalData(p => ({...p, [key]: [...(p[key]||[]), ...newItems]}));
                    sendToCloud('batch', key, newItems);
                },
                batchUpdate: (updates) => {
                    setLocalData(p => ({...p, ...updates}));
                },
                // EXPOSE save function for manual custom logic
                save: sendToCloud
            };
            return { db: localData, ...crud, isOnline, isLoading, isBackgroundSyncing, lastSyncTime, refresh: () => scriptUrl && syncData(scriptUrl, false) };
        };

        // --- COMPONENTS ---
        const LoginCard = ({ isModal = false, db, handleRoleLogin, setShowLogin, onRefresh, isLoading }) => {
            const [loginRole, setLoginRole] = useState(null); 
            const [idInput, setIdInput] = useState('');
            const [passInput, setPassInput] = useState('');
            const [error, setError] = useState('');

            useEffect(() => {
                setIdInput('');
                setPassInput('');
                setError('');
            }, [loginRole]);

            const attemptLogin = () => {
                setError('');
                const cleanId = idInput.trim();
                const cleanPass = passInput.trim();

                if (loginRole !== 'admin' && !cleanId) {
                    setError('Mohon isi ID (NPM/NIDN)');
                    return;
                }
                
                if (!cleanPass) {
                    setError('Mohon isi Password');
                    return;
                }

                if (loginRole === 'admin') {
                    if (btoa(cleanPass) === AUTH_TOKEN) {
                        handleRoleLogin('admin');
                    } else {
                        setError('Password Admin Salah!');
                    }
                } else if (loginRole === 'tendik') {
                    if (cleanId === '101090' && cleanPass === '101090') {
                        handleRoleLogin('tendik', { Nama: 'Staf Akademik (Tendik)', NIDN: '101090' });
                    } else {
                        setError('ID atau Password Tendik Salah!');
                    }
                } else if (loginRole === 'mahasiswa') {
                    const user = (db['Mahasiswa Tugas Akhir'] || []).find(m => String(m.NPM).trim() === cleanId);
                    
                    if (user) {
                        if (cleanPass === String(user.NPM).trim()) { 
                            handleRoleLogin('mahasiswa', user);
                        } else {
                            setError('Password Salah! (Gunakan NPM)');
                        }
                    } else {
                        setError('NPM tidak ditemukan dalam sistem! Jika data baru saja ditambahkan, coba refresh data.');
                    }
                } else if (loginRole === 'dosen') {
                    const user = (db['Data Dosen'] || []).find(d => String(d.NIDN).trim() === cleanId);
                    
                    if (user) {
                         if (cleanPass === String(user.NIDN).trim()) { 
                             handleRoleLogin('dosen', user);
                         } else {
                             setError('Password Salah! (Gunakan NIDN)');
                         }
                    } else {
                        setError('NIDN tidak ditemukan dalam sistem! Jika data baru saja ditambahkan, coba refresh data.');
                    }
                }
            };

            const renderInputs = () => {
                if (!loginRole) return null;
                
                return (
                    <div className="space-y-4 animate-fade-in">
                        {loginRole !== 'admin' && (
                            <div>
                                <label className="text-xs font-bold text-purple-700 uppercase ml-1">
                                    {loginRole === 'mahasiswa' ? 'NPM' : loginRole === 'tendik' ? 'ID Tendik' : 'NIDN'}
                                </label>
                                <input className="input-modern" placeholder={loginRole === 'mahasiswa' ? '2020...' : '123...'} value={idInput} onChange={e => setIdInput(e.target.value)} autoFocus />
                            </div>
                        )}
                        <div>
                            <label className="text-xs font-bold text-purple-700 uppercase ml-1">Password</label>
                            <input type="password" className="input-modern" placeholder="••••••" value={passInput} onChange={e => setPassInput(e.target.value)} onKeyDown={e => e.key === 'Enter' && attemptLogin()} />
                        </div>
                        {error && <div className="p-3 bg-red-100 text-red-600 text-sm rounded-xl font-bold text-center border border-red-200 animate-pulse">{error}</div>}
                        <button onClick={attemptLogin} className="w-full py-3 bg-gradient-to-r from-purple-600 to-pink-600 text-white rounded-xl font-bold shadow-lg shadow-purple-500/30 hover:shadow-xl transition transform active:scale-95">Masuk</button>
                        <button onClick={() => setLoginRole(null)} className="w-full py-2 text-purple-500 text-sm hover:underline">Kembali</button>
                    </div>
                );
            };

            return (
                <div className={`glass p-8 md:p-10 rounded-3xl w-full max-w-sm shadow-2xl border border-white/60 relative overflow-hidden ${isModal ? '' : 'animate-slide-up'}`}>
                    <div className="absolute -top-10 -right-10 w-32 h-32 bg-purple-300 rounded-full blur-3xl opacity-30"></div>
                    <div className="absolute -bottom-10 -left-10 w-32 h-32 bg-pink-300 rounded-full blur-3xl opacity-30"></div>
                    {!loginRole && (
                        <div onClick={() => setLoginRole('admin')} className="cursor-pointer w-20 h-20 bg-gradient-to-br from-purple-100 to-white rounded-2xl flex items-center justify-center mx-auto mb-6 text-purple-600 shadow-lg shadow-purple-500/10 rotate-3 hover:rotate-6 transition-all duration-300 hover:scale-110 active:scale-95 group" title="Klik untuk akses Admin">
                            <Icon path={PATHS.Lock} size={36} className="group-hover:text-purple-800 transition-colors"/>
                        </div>
                    )}
                    <h3 className="text-2xl font-bold mb-2 text-center text-purple-900">{isModal ? 'Ganti Akses' : (loginRole ? `Login ${loginRole.charAt(0).toUpperCase() + loginRole.slice(1)}` : 'Selamat Datang')}</h3>
                    {!loginRole && <p className="text-center text-purple-600/70 text-xs mb-8">SI Tugas Akhir Terintegrasi FIKPsi</p>}
                    {!loginRole ? (
                        <div className="space-y-3 mb-6">
                            <button onClick={()=>setLoginRole('mahasiswa')} className="group w-full py-3.5 bg-white/70 hover:bg-white border border-white rounded-xl text-purple-700 font-bold transition flex items-center justify-center gap-3 shadow-sm hover:shadow-md hover:scale-[1.02]">
                                <span className="p-1 bg-purple-100 rounded-lg group-hover:bg-purple-200 transition"><Icon path={PATHS.Graduation} size={18}/></span> Mahasiswa
                            </button>
                            <button onClick={()=>setLoginRole('dosen')} className="group w-full py-3.5 bg-white/70 hover:bg-white border border-white rounded-xl text-purple-700 font-bold transition flex items-center justify-center gap-3 shadow-sm hover:shadow-md hover:scale-[1.02]">
                                <span className="p-1 bg-purple-100 rounded-lg group-hover:bg-purple-200 transition"><Icon path={PATHS.Users} size={18}/></span> Dosen
                            </button>
                            <button onClick={()=>setLoginRole('tendik')} className="group w-full py-3.5 bg-white/70 hover:bg-white border border-white rounded-xl text-purple-700 font-bold transition flex items-center justify-center gap-3 shadow-sm hover:shadow-md hover:scale-[1.02]">
                                <span className="p-1 bg-purple-100 rounded-lg group-hover:bg-purple-200 transition"><Icon path={PATHS.Cog} size={18}/></span> Tenaga Kependidikan
                            </button>
                        </div>
                    ) : renderInputs()}
                    {isModal && <button onClick={()=>setShowLogin(false)} className="absolute top-4 right-4 text-purple-300 hover:text-purple-600 transition"><Icon path={PATHS.X} size={20}/></button>}
                </div>
            );
        };

        const NotificationPopup = ({ data, onClose }) => (
            <div className="fixed inset-0 z-50 flex items-center justify-center p-4 bg-black/20 backdrop-blur-sm animate-fade-in" onClick={onClose}>
                <div className="glass bg-white p-6 rounded-3xl max-w-sm w-full shadow-2xl relative border-2 border-white/50 animate-pop-in" onClick={e=>e.stopPropagation()}>
                    <div className="absolute -top-12 left-1/2 transform -translate-x-1/2 w-24 h-24 bg-gradient-to-tr from-yellow-300 to-orange-400 rounded-full flex items-center justify-center border-4 border-white shadow-lg animate-blob">
                        <span className="text-4xl animate-bounce-slight">🔔</span>
                    </div>
                    <button onClick={onClose} className="absolute top-4 right-4 text-purple-300 hover:text-purple-600 transition"><Icon path={PATHS.X}/></button>
                    <div className="mt-10 text-center">
                        <h4 className="text-xl font-bold text-purple-900 mb-2">Halo, {data.user}!</h4>
                        <p className="text-xs font-bold text-pink-500 uppercase tracking-widest mb-4">{data.type}</p>
                        <div className="bg-purple-50 p-4 rounded-2xl border border-purple-100 text-sm text-gray-600 mb-6">
                            <p className="font-bold text-purple-800 mb-1">{data.title}</p>
                            <p>{data.message}</p>
                        </div>
                        <button onClick={onClose} className="bg-gradient-to-r from-purple-600 to-pink-500 text-white px-8 py-3 rounded-xl font-bold shadow-lg hover:shadow-purple-500/40 hover:scale-105 transition transform active:scale-95">
                            Oke, Mengerti!
                        </button>
                    </div>
                </div>
            </div>
        )

        // ... (WorkloadChart, GenericTable components are the same, just reused)
        const WorkloadChart = ({ dosenData }) => {
            return (
                <div className="space-y-5">
                    {dosenData.map((d, idx) => {
                        const percent = Math.min((d.Terisi / d.Kuota) * 100, 100);
                        const isFull = d.Terisi >= d.Kuota;
                        return (
                            <div key={d.id} className="relative group cursor-default">
                                <div className="flex justify-between text-sm mb-1.5 font-medium items-end">
                                    <div className="flex flex-col">
                                        <span className="text-purple-900 font-bold">{d.Nama}</span>
                                        <span className="text-[10px] text-purple-400">{d.Keahlian}</span>
                                    </div>
                                    <span className={`font-bold px-2 py-0.5 rounded-md text-xs ${isFull ? 'bg-red-100 text-red-600' : 'bg-green-100 text-green-600'}`}>
                                        {d.Terisi}/{d.Kuota}
                                    </span>
                                </div>
                                <div className="w-full bg-white/50 rounded-full h-2.5 overflow-hidden shadow-inner">
                                    <div className={`h-full rounded-full transition-all duration-1000 ease-out shadow-sm relative overflow-hidden ${isFull ? 'bg-gradient-to-r from-red-400 to-red-600' : 'bg-gradient-to-r from-violet-400 to-fuchsia-500'}`} style={{ width: `${percent}%`, transitionDelay: `${idx * 100}ms` }}>
                                        <div className="absolute top-0 left-0 w-full h-full bg-white/20 animate-pulse-slow"></div>
                                    </div>
                                </div>
                            </div>
                        )
                    })}
                </div>
            );
        };

        const GenericTable = ({ title, data, columns, formConfig, onAdd, onDel, onUpdate, onImport, allowAdd, allowDelete, allowEdit, allowImport, customFilters, statusFilterConfig, gformUrl, onBack }) => {
            const [isOpen, setIsOpen] = useState(false);
            const [form, setForm] = useState({});
            const [search, setSearch] = useState("");
            const [filterValues, setFilterValues] = useState({});
            const [activeStatus, setActiveStatus] = useState(null); // STATE FOR STATUS FILTER BUTTONS
            const [detailItem, setDetailItem] = useState(null);
            const [isEditing, setIsEditing] = useState(false);
            const [editForm, setEditForm] = useState({});
            const [showImport, setShowImport] = useState(false);

            // Reset filter when config changes (e.g. switching pages if component reused)
            // FIXED: Removed dependency on full object which caused resets on re-renders
            useEffect(() => {
                setActiveStatus(null);
            }, [statusFilterConfig ? statusFilterConfig.key : null]);

            const safeData = data || []; 

            const filtered = safeData.filter(d => {
                const matchesSearch = Object.values(d).some(v => String(v).toLowerCase().includes(search.toLowerCase()));
                
                // Logic for Dropdown Filters
                let matchesFilters = true;
                if (customFilters) {
                    matchesFilters = customFilters.every(f => {
                        const val = filterValues[f.key];
                        if (!val) return true; 
                        return d[f.key] === val;
                    });
                }

                // Logic for Button Status Filter (Mutually Exclusive)
                // FIXED: More robust comparison (trim and lowercase)
                let matchesStatus = true;
                if (statusFilterConfig && activeStatus) {
                    const rowValue = d[statusFilterConfig.key];
                    const normalize = (val) => val ? String(val).toLowerCase().trim() : '';
                    matchesStatus = normalize(rowValue) === normalize(activeStatus);
                }

                return matchesSearch && matchesFilters && matchesStatus;
            }).sort((a, b) => (a.Nama || '').localeCompare(b.Nama || ''));

            const handleTemplateDownload = () => {
                const headers = formConfig.map(f => f.key);
                const sampleRow = formConfig.map(f => {
                    if (f.type === 'number') return 10;
                    if (f.key === 'Progres') return 50;
                    if (f.key.includes('NPM')) return '2021...';
                    if (f.type === 'date') return '2024-01-01';
                    if (f.options && f.options.length > 0) return f.options[0].value; 
                    return `Contoh ${f.label}`;
                });
                const ws = XLSX.utils.aoa_to_sheet([headers, sampleRow]);
                const wscols = headers.map(h => ({ wch: Math.max(h.length + 5, 15) }));
                ws['!cols'] = wscols;
                const wb = XLSX.utils.book_new();
                XLSX.utils.book_append_sheet(wb, ws, "Template");
                XLSX.writeFile(wb, `Template_${title.replace(/\s+/g, '_')}.xlsx`);
            };

            const handleFileUpload = (e) => {
                const file = e.target.files[0];
                if (!file) return;
                const reader = new FileReader();
                reader.onload = (evt) => {
                    const bstr = evt.target.result;
                    const wb = XLSX.read(bstr, { type: 'binary' });
                    const wsname = wb.SheetNames[0];
                    const ws = wb.Sheets[wsname];
                    const data = XLSX.utils.sheet_to_json(ws);
                    const cleanData = data.filter(row => {
                        const values = Object.values(row);
                        return values.some(v => String(v).includes('Contoh') === false); 
                    });
                    if (confirm(`Akan mengimport ${cleanData.length} data. Lanjutkan?`)) {
                        onImport(cleanData);
                        e.target.value = null;
                        setShowImport(false);
                        alert('Import berhasil! Data sedang disinkronkan.');
                    }
                };
                reader.readAsBinaryString(file);
            };

            return (
                <div className="space-y-6 animate-fade-in pb-20">
                    <div className="flex flex-col md:flex-row justify-between gap-4 items-center">
                        <div className="flex items-center gap-3 w-full md:w-auto">
                            {onBack && (
                                <button onClick={onBack} className="p-3 bg-white/60 rounded-xl hover:bg-white transition shadow-sm text-purple-600 border border-white">
                                    <Icon path={PATHS.ArrowLeft} size={20}/>
                                </button>
                            )}
                            <h2 className="text-2xl font-bold text-purple-900 flex items-center gap-3">
                                <span className="w-2 h-8 bg-gradient-to-b from-purple-500 to-pink-500 rounded-full shadow-lg shadow-purple-500/30"></span> {title}
                            </h2>
                        </div>
                        <div className="flex flex-wrap gap-2 w-full md:w-auto items-center justify-end">
                            {allowImport && (
                                <div className="relative">
                                    <button onClick={()=>setShowImport(!showImport)} className={`px-4 py-2.5 rounded-xl font-bold text-sm transition shadow-lg flex items-center gap-2 transform active:scale-95 ${showImport ? 'bg-purple-100 text-purple-700' : 'bg-white text-purple-600 border border-purple-100 hover:bg-purple-50'}`}>
                                        <Icon path={PATHS.FileUp} size={18}/> Import Data
                                    </button>
                                    {showImport && (
                                        <div className="absolute right-0 top-full mt-2 bg-white p-4 rounded-xl shadow-2xl z-50 w-64 border border-purple-100 animate-slide-up">
                                            <h4 className="font-bold text-sm mb-3 text-purple-900 border-b border-purple-50 pb-2">Import Excel</h4>
                                            <button onClick={handleTemplateDownload} className="w-full text-left px-3 py-2.5 text-xs font-bold text-purple-600 hover:bg-purple-50 rounded-lg mb-2 flex items-center gap-2 transition">
                                                <Icon path={PATHS.Download} size={14}/> 1. Unduh Template
                                            </button>
                                            <div className="relative group">
                                                <input type="file" accept=".xlsx, .xls" onChange={handleFileUpload} className="absolute inset-0 w-full h-full opacity-0 cursor-pointer z-10"/>
                                                <button className="w-full text-left px-3 py-2.5 text-xs font-bold text-white bg-gradient-to-r from-green-500 to-emerald-600 hover:shadow-lg rounded-lg flex items-center gap-2 transition group-active:scale-95">
                                                    <Icon path={PATHS.FileUp} size={14}/> 2. Upload File Excel
                                                </button>
                                            </div>
                                            <p className="text-[10px] text-gray-400 mt-2 text-center">Isi data di bawah header kolom.</p>
                                        </div>
                                    )}
                                </div>
                            )}
                            {customFilters && customFilters.map(f => (
                                <div key={f.key} className="relative flex-grow md:flex-grow-0">
                                    <select className="input-modern pl-3 py-2.5 text-sm w-full md:w-40 shadow-sm cursor-pointer bg-white/80 border-purple-100" value={filterValues[f.key] || ""} onChange={e => setFilterValues({...filterValues, [f.key]: e.target.value})}>
                                            <option value="">{f.label}</option>
                                            {f.options.map((opt, i) => <option key={i} value={opt}>{opt}</option>)}
                                    </select>
                                </div>
                            ))}
                            <div className="relative flex-grow md:flex-grow-0 group">
                                <Icon path={PATHS.Search} className="absolute left-3 top-3 text-purple-400 group-focus-within:text-purple-600 transition-colors" size={18}/>
                                <input className="input-modern pl-10 py-2.5 text-sm w-full md:w-48 shadow-sm" placeholder="Cari data..." value={search} onChange={e=>setSearch(e.target.value)}/>
                            </div>
                            {gformUrl && (
                                <a href={gformUrl} target="_blank" className="bg-gradient-to-r from-purple-600 to-indigo-600 text-white px-5 py-2.5 rounded-xl font-semibold text-sm hover:shadow-lg hover:shadow-purple-500/30 transition transform hover:-translate-y-0.5 flex items-center gap-2">
                                    <Icon path={PATHS.ExternalLink} size={18}/> Daftar
                                </a>
                            )}
                            {allowAdd && (
                                <button onClick={()=>setIsOpen(!isOpen)} className={`px-5 py-2.5 rounded-xl font-semibold text-sm transition shadow-lg flex items-center gap-2 transform active:scale-95 ${isOpen ? 'bg-red-50 text-red-500 border border-red-200' : 'bg-gradient-to-r from-pink-500 to-purple-600 text-white hover:shadow-purple-500/30 hover:-translate-y-0.5'}`}>
                                    <Icon path={isOpen ? PATHS.X : PATHS.Plus} size={18}/> {isOpen ? 'Batal' : 'Tambah'}
                                </button>
                            )}
                        </div>
                    </div>

                    {/* STATUS FILTER BUTTONS (TAB STYLE) */}
                    {statusFilterConfig && (
                        <div className="flex flex-wrap gap-2 animate-fade-in mb-2">
                            <button 
                                type="button"
                                onClick={() => setActiveStatus(null)} 
                                className={`px-4 py-2 rounded-xl text-xs font-bold transition-all duration-300 border ${!activeStatus ? 'bg-purple-600 text-white border-purple-600 shadow-md transform scale-105' : 'bg-white text-gray-500 border-gray-200 hover:border-purple-300 hover:text-purple-600'}`}
                            >
                                Semua
                            </button>
                            {statusFilterConfig.options.map(opt => (
                                <button 
                                    type="button"
                                    key={opt} 
                                    onClick={() => setActiveStatus(opt)} 
                                    className={`px-4 py-2 rounded-xl text-xs font-bold transition-all duration-300 border ${activeStatus === opt ? 'bg-purple-600 text-white border-purple-600 shadow-md transform scale-105' : 'bg-white text-gray-500 border-gray-200 hover:border-purple-300 hover:text-purple-600'}`}
                                >
                                    {opt}
                                </button>
                            ))}
                        </div>
                    )}

                    {isOpen && allowAdd && (
                        <form onSubmit={(e)=>{e.preventDefault(); onAdd(form); setForm({}); setIsOpen(false); }} className="glass p-6 md:p-8 rounded-3xl grid md:grid-cols-2 gap-6 shadow-xl border border-white/60 animate-slide-up relative z-10">
                            {formConfig.map(f => (
                                <div key={f.key} className={f.type === 'textarea' ? 'md:col-span-2' : ''}>
                                    <label className="text-xs font-bold text-purple-800/70 uppercase ml-1 mb-2 block tracking-wide">{f.label}</label>
                                    {f.type==='select' ? (
                                        <div className="relative">
                                            <select className="input-modern cursor-pointer appearance-none" value={form[f.key]||''} onChange={e=>setForm({...form,[f.key]:e.target.value})}>
                                                <option value="">Pilih...</option>{f.options.map(o=><option key={o.value} value={o.value}>{o.label}</option>)}
                                            </select>
                                            <Icon path={PATHS.ChevronDown} className="absolute right-3 top-3 text-purple-400 pointer-events-none" size={16}/>
                                        </div>
                                    ) : f.type === 'textarea' ? (
                                        <textarea className="textarea-modern" value={form[f.key]||''} onChange={e=>setForm({...form,[f.key]:e.target.value})} placeholder={f.placeholder || ''} required/>
                                    ) : (
                                        <input className="input-modern" type={f.type||'text'} value={form[f.key]||''} onChange={e=>setForm({...form,[f.key]:e.target.value})} placeholder={f.placeholder || ''} required/>
                                    )}
                                </div>
                            ))}
                            <button type="submit" className="md:col-span-2 bg-gradient-to-r from-purple-600 to-indigo-600 text-white py-3.5 rounded-xl font-bold mt-4 hover:shadow-xl hover:shadow-purple-500/30 transition transform hover:-translate-y-0.5 active:translate-y-0">Simpan Data</button>
                        </form>
                    )}

                    <div className="glass rounded-3xl overflow-hidden shadow-lg border border-white/60 overflow-x-auto relative z-0">
                        <table className="w-full text-sm text-left">
                            <thead className="bg-purple-50/80 backdrop-blur-md text-purple-900/70 font-bold uppercase text-xs border-b border-purple-100">
                                <tr>{columns.map(c=><th key={c.key} className="px-6 py-5 whitespace-nowrap">{c.label}</th>)}{allowDelete && <th className="px-6 py-5 text-center">Aksi</th>}</tr>
                            </thead>
                            <tbody className="divide-y divide-purple-50">
                                {filtered.map((row, idx)=>(
                                    <tr key={row.id} className="hover:bg-purple-50/60 transition duration-150 group" style={{animationDelay: `${idx*50}ms`}}>
                                            {columns.map(c=><td key={c.key} className="px-6 py-4 text-purple-900 font-medium whitespace-nowrap">
                                                {(c.key === 'Nama' || c.key === 'Mahasiswa' || c.key === 'Judul') ? (
                                                    <button onClick={() => {setDetailItem(row); setIsEditing(false);}} className="flex items-center gap-2 font-bold hover:text-pink-600 transition-colors text-left">
                                                        <div className="w-8 h-8 rounded-full bg-gradient-to-tr from-purple-200 to-pink-200 flex items-center justify-center text-purple-700 text-xs shadow-inner">
                                                            {row[c.key].substring(0,2).toUpperCase()}
                                                        </div>
                                                        <span className="truncate max-w-[200px] block" title={row[c.key]}>{row[c.key]}</span>
                                                    </button>
                                                ) : (c.render ? c.render(row[c.key], row) : row[c.key])}
                                            </td>)}
                                            {allowDelete && <td className="px-6 py-4 text-center"><button onClick={()=>onDel(row.id)} className="text-red-300 hover:text-red-600 bg-red-50/0 hover:bg-red-50 p-2 rounded-lg transition"><Icon path={PATHS.Trash}/></button></td>}
                                    </tr>
                                ))}
                            </tbody>
                        </table>
                        {filtered.length===0 && <div className="p-12 text-center flex flex-col items-center gap-4 text-purple-300">
                            <Icon path={PATHS.Search} size={48} className="opacity-20"/>
                            <span className="font-medium">Belum ada data ditemukan</span>
                        </div>}
                    </div>

                    {detailItem && (
                        <div className="fixed inset-0 z-[60] flex items-center justify-center bg-purple-900/20 backdrop-blur-sm p-4 animate-fade-in" onClick={() => setDetailItem(null)}>
                            <div className="glass bg-white p-6 md:p-8 rounded-3xl w-full max-w-lg shadow-2xl border border-white/60 relative overflow-y-auto max-h-[90vh] animate-slide-up" onClick={e => e.stopPropagation()}>
                                <button onClick={() => setDetailItem(null)} className="absolute top-4 right-4 text-gray-400 hover:text-gray-600 bg-white/50 rounded-full p-2 hover:bg-white transition"><Icon path={PATHS.X} size={20}/></button>
                                <h3 className="text-2xl font-bold text-purple-900 mb-6 border-b border-purple-100 pb-2 flex items-center gap-3">
                                    <Icon path={PATHS.Info} className="text-purple-500"/> {isEditing ? 'Edit Data' : 'Detail Data'}
                                </h3>
                                {!isEditing ? (
                                    <div className="space-y-4">
                                            {Object.entries(detailItem).map(([key, value]) => {
                                                if (key === 'id') return null;
                                                
                                                // 1. Custom Label Mapping untuk Tampilan Lebih Rapi
                                                const labelMap = {
                                                    BimbinganCount: 'Jumlah Bimbingan',
                                                    ProgresDeskripsi: 'Detail Progres',
                                                    LastUpdateProgres: 'Waktu Lapor Progres',
                                                    StatusAkademik: 'Status Akademik',
                                                    Pembimbing_1: 'Pembimbing 1',
                                                    Pembimbing_2: 'Pembimbing 2',
                                                    Jenis_Surat: 'Jenis Surat',
                                                    LinkLaporan: 'Link Laporan (G Drive)'
                                                };
                                                const displayLabel = labelMap[key] || key.replace(/_/g, ' ');

                                                // 2. Format Value Khusus
                                                let displayValue = value;
                                                // Format Tanggal Update
                                                if (key === 'LastUpdateProgres' && value) {
                                                    try { 
                                                        displayValue = new Date(value).toLocaleDateString('id-ID', {day: 'numeric', month: 'long', year: 'numeric', hour: '2-digit', minute:'2-digit'}); 
                                                    } catch(e){}
                                                }
                                                // Handle Angka 0 agar tidak dianggap kosong
                                                if (value === 0) displayValue = "0";

                                                return (
                                                    <div key={key} className="grid grid-cols-1 md:grid-cols-3 gap-1 md:gap-4 border-b border-purple-50 pb-2 last:border-0">
                                                        <div className="text-xs font-bold text-purple-400 uppercase tracking-wider pt-1">{displayLabel}</div>
                                                        <div className="md:col-span-2 text-gray-800 font-medium text-sm break-words whitespace-pre-wrap">
                                                            {(typeof displayValue === 'string' && displayValue.startsWith('http')) ? 
                                                                <a href={displayValue} target="_blank" className="text-blue-600 hover:underline flex items-center gap-1"><Icon path={PATHS.ExternalLink} size={14}/> Buka Link</a> : (displayValue || "-")}
                                                        </div>
                                                    </div>
                                                )
                                            })}
                                            {allowEdit && (
                                                <div className="mt-6 pt-4 border-t border-purple-100 flex justify-end">
                                                    <button onClick={() => { setEditForm(detailItem); setIsEditing(true); }} className="bg-purple-600 text-white px-6 py-2.5 rounded-xl font-bold hover:bg-purple-700 transition shadow-lg shadow-purple-500/30 flex items-center gap-2">
                                                        <Icon path={PATHS.Edit} size={18}/> Edit Data
                                                    </button>
                                                </div>
                                            )}
                                    </div>
                                ) : (
                                    <form onSubmit={(e) => {
                                        e.preventDefault();
                                        onUpdate(detailItem.id, editForm);
                                        setDetailItem({...detailItem, ...editForm});
                                        setIsEditing(false);
                                        // Alert removed here to let function handle it or can add it back if needed
                                    }} className="space-y-4 animate-fade-in">
                                            {formConfig.map(f => (
                                                <div key={f.key} className={f.type === 'textarea' ? 'md:col-span-2' : ''}>
                                                    <label className="text-xs font-bold text-purple-800/70 uppercase ml-1 mb-2 block tracking-wide">{f.label}</label>
                                                    {f.type === 'select' ? (
                                                        <div className="relative">
                                                            <select className="input-modern cursor-pointer appearance-none" value={editForm[f.key] || ''} onChange={e => setEditForm({...editForm, [f.key]: e.target.value})}>
                                                                <option value="">Pilih...</option>
                                                                {f.options.map(o => <option key={o.value} value={o.value}>{o.label}</option>)}
                                                            </select>
                                                            <Icon path={PATHS.ChevronDown} className="absolute right-3 top-3 text-purple-400 pointer-events-none" size={16}/>
                                                        </div>
                                                    ) : f.type === 'textarea' ? (
                                                        <textarea className="textarea-modern" value={editForm[f.key] || ''} onChange={e => setEditForm({...editForm, [f.key]: e.target.value})} placeholder={f.placeholder || ''} required/>
                                                    ) : (
                                                        <input className="input-modern" type={f.type || 'text'} value={editForm[f.key] || ''} onChange={e => setEditForm({...editForm, [f.key]: e.target.value})} placeholder={f.placeholder || ''} required/>
                                                    )}
                                                </div>
                                            ))}
                                            <div className="flex gap-3 pt-4">
                                                <button type="submit" className="flex-1 bg-gradient-to-r from-purple-600 to-indigo-600 text-white py-3 rounded-xl font-bold hover:shadow-xl transition transform active:scale-95">Simpan Perubahan</button>
                                                <button type="button" onClick={() => setIsEditing(false)} className="px-6 py-3 bg-red-50 text-red-600 rounded-xl font-bold hover:bg-red-100 transition">Batal</button>
                                            </div>
                                    </form>
                                )}
                            </div>
                        </div>
                    )}
                </div>
            );
        };

        const InboxSystem = ({ db, currentUser, role, onSend }) => {
            // ... (rest of code)
            const [activeTab, setActiveTab] = useState('masuk');
            const [composeMode, setComposeMode] = useState(false);
            const [selectedMsg, setSelectedMsg] = useState(null);
            const [newMsg, setNewMsg] = useState({ to: '', subject: '', content: '' });

            // 1. Get Messages
            const messages = (db['Pesan'] || []).filter(m => {
                if (activeTab === 'masuk') return m.receiver === currentUser.Nama;
                return m.sender === currentUser.Nama;
            }).sort((a, b) => new Date(b.timestamp) - new Date(a.timestamp));

            // 2. Logic for Recipient Options
            const recipientOptions = useMemo(() => {
                if (role === 'dosen') {
                    // Dosen can message their supervised students
                    return (db['Mahasiswa Tugas Akhir'] || [])
                        .filter(m => m.Pembimbing_1 === currentUser.Nama || m.Pembimbing_2 === currentUser.Nama || m.Penguji === currentUser.Nama)
                        .map(m => ({ value: m.Nama, label: `${m.Nama} (${m.NPM})` }));
                } else if (role === 'mahasiswa') {
                    // Mahasiswa can message their supervisors
                    const myData = (db['Mahasiswa Tugas Akhir'] || []).find(m => m.Nama === currentUser.Nama);
                    if (!myData) return [];
                    const lecturers = [];
                    if (myData.Pembimbing_1 && myData.Pembimbing_1 !== '-') lecturers.push(myData.Pembimbing_1);
                    if (myData.Pembimbing_2 && myData.Pembimbing_2 !== '-') lecturers.push(myData.Pembimbing_2);
                    if (myData.Penguji && myData.Penguji !== '-') lecturers.push(myData.Penguji);
                    return [...new Set(lecturers)].map(name => ({ value: name, label: name }));
                } else if (role === 'tendik') {
                    // Tendik can message everyone (Dosen & Mahasiswa)
                    const dosenList = (db['Data Dosen'] || []).map(d => ({ value: d.Nama, label: `${d.Nama} (Dosen)` }));
                    const mhsList = (db['Mahasiswa Tugas Akhir'] || []).map(m => ({ value: m.Nama, label: `${m.Nama} (Mahasiswa)` }));
                    return [...dosenList, ...mhsList];
                }
                return [];
            }, [role, currentUser, db]);

            const handleSend = (e) => {
                e.preventDefault();
                if(!newMsg.to || !newMsg.subject || !newMsg.content) return alert("Mohon lengkapi pesan.");
                
                onSend({
                    sender: currentUser.Nama,
                    receiver: newMsg.to,
                    subject: newMsg.subject,
                    content: newMsg.content,
                    timestamp: new Date().toISOString(),
                    isRead: false
                });
                
                setComposeMode(false);
                setNewMsg({ to: '', subject: '', content: '' });
                setActiveTab('keluar');
            };

            return (
                <div className="h-full flex flex-col animate-fade-in relative pb-0">
                    <div className="flex justify-between items-center mb-6">
                        <h2 className="text-2xl font-bold text-purple-900 flex items-center gap-3">
                            <Icon path={PATHS.Mail} className="text-pink-500"/> Kotak Masuk
                        </h2>
                        {!composeMode && (
                            <button onClick={() => setComposeMode(true)} className="bg-gradient-to-r from-purple-600 to-pink-600 text-white px-5 py-2.5 rounded-xl font-bold shadow-lg hover:shadow-purple-500/30 transition transform active:scale-95 flex items-center gap-2">
                                <Icon path={PATHS.Plus} size={18}/> Tulis Pesan
                            </button>
                        )}
                    </div>

                    {composeMode ? (
                        <div className="glass p-6 md:p-8 rounded-3xl shadow-xl border border-white/60 animate-slide-up">
                            <div className="flex justify-between items-center mb-6 border-b border-purple-100 pb-2">
                                <h3 className="font-bold text-lg text-purple-800">Tulis Pesan Baru</h3>
                                <button onClick={() => setComposeMode(false)} className="text-gray-400 hover:text-red-500"><Icon path={PATHS.X}/></button>
                            </div>
                            <form onSubmit={handleSend} className="space-y-4">
                                <div>
                                    <label className="text-xs font-bold text-purple-800/70 uppercase ml-1 mb-2 block">Kepada</label>
                                    <div className="relative">
                                        <select className="input-modern cursor-pointer appearance-none" value={newMsg.to} onChange={e => setNewMsg({...newMsg, to: e.target.value})} required>
                                            <option value="">Pilih Penerima...</option>
                                            {recipientOptions.map((opt, i) => <option key={i} value={opt.value}>{opt.label}</option>)}
                                        </select>
                                        <Icon path={PATHS.ChevronDown} className="absolute right-3 top-3 text-purple-400 pointer-events-none" size={16}/>
                                    </div>
                                    {recipientOptions.length === 0 && <p className="text-[10px] text-red-400 mt-1 ml-1">* Tidak ada kontak yang terhubung (Bimbingan/Pembimbing).</p>}
                                </div>
                                <div>
                                    <label className="text-xs font-bold text-purple-800/70 uppercase ml-1 mb-2 block">Subjek</label>
                                    <input className="input-modern" value={newMsg.subject} onChange={e => setNewMsg({...newMsg, subject: e.target.value})} placeholder="Contoh: Revisi Bab 1" required />
                                </div>
                                <div>
                                    <label className="text-xs font-bold text-purple-800/70 uppercase ml-1 mb-2 block">Isi Pesan</label>
                                    <textarea className="textarea-modern min-h-[150px]" value={newMsg.content} onChange={e => setNewMsg({...newMsg, content: e.target.value})} placeholder="Tulis pesan Anda di sini..." required />
                                </div>
                                <div className="flex justify-end gap-3 pt-2">
                                    <button type="button" onClick={() => setComposeMode(false)} className="px-6 py-3 bg-red-50 text-red-600 rounded-xl font-bold hover:bg-red-100 transition">Batal</button>
                                    <button type="submit" className="bg-purple-600 text-white px-8 py-3 rounded-xl font-bold hover:bg-purple-700 transition shadow-lg flex items-center gap-2">
                                        <Icon path={PATHS.PaperPlane} size={18}/> Kirim
                                    </button>
                                </div>
                            </form>
                        </div>
                    ) : (
                        <div className="glass rounded-3xl shadow-xl border border-white/60 overflow-hidden flex flex-col h-[70vh]">
                            <div className="flex border-b border-purple-100 bg-white/40">
                                <button onClick={() => {setActiveTab('masuk'); setSelectedMsg(null)}} className={`flex-1 py-4 font-bold text-sm flex items-center justify-center gap-2 transition ${activeTab === 'masuk' ? 'bg-purple-100/50 text-purple-700 border-b-2 border-purple-500' : 'text-gray-500 hover:bg-white/60'}`}>
                                    <Icon path={PATHS.Inbox} size={18}/> Kotak Masuk
                                </button>
                                <button onClick={() => {setActiveTab('keluar'); setSelectedMsg(null)}} className={`flex-1 py-4 font-bold text-sm flex items-center justify-center gap-2 transition ${activeTab === 'keluar' ? 'bg-purple-100/50 text-purple-700 border-b-2 border-purple-500' : 'text-gray-500 hover:bg-white/60'}`}>
                                    <Icon path={PATHS.PaperPlane} size={18}/> Pesan Keluar
                                </button>
                            </div>
                            
                            <div className="flex-1 overflow-y-auto p-4 custom-scrollbar bg-white/30">
                                {messages.length === 0 ? (
                                    <div className="h-full flex flex-col items-center justify-center text-gray-400 gap-3">
                                        <Icon path={PATHS.Mail} size={48} className="opacity-20"/>
                                        <span className="text-sm">Tidak ada pesan.</span>
                                    </div>
                                ) : (
                                    <div className="space-y-3">
                                        {messages.map((msg) => (
                                            <div key={msg.id} onClick={() => setSelectedMsg(selectedMsg?.id === msg.id ? null : msg)} className={`bg-white p-4 rounded-xl border transition cursor-pointer group ${selectedMsg?.id === msg.id ? 'border-purple-400 shadow-md ring-2 ring-purple-100' : 'border-white/60 hover:border-purple-200 hover:shadow-sm'}`}>
                                                <div className="flex justify-between items-start mb-1">
                                                    <div className="flex items-center gap-2">
                                                        <div className="w-8 h-8 rounded-full bg-gradient-to-br from-purple-100 to-pink-100 text-purple-600 flex items-center justify-center text-xs font-bold">
                                                            {(activeTab === 'masuk' ? msg.sender : msg.receiver).charAt(0)}
                                                        </div>
                                                        <div>
                                                            <div className="text-sm font-bold text-gray-800">{activeTab === 'masuk' ? msg.sender : `Ke: ${msg.receiver}`}</div>
                                                            <div className="text-[10px] text-gray-400">{new Date(msg.timestamp).toLocaleString('id-ID')}</div>
                                                        </div>
                                                    </div>
                                                    {activeTab === 'masuk' && !msg.isRead && <div className="w-2 h-2 bg-pink-500 rounded-full"></div>}
                                                </div>
                                                <div className="font-bold text-purple-900 text-sm mt-2 mb-1">{msg.subject}</div>
                                                <div className={`text-sm text-gray-600 ${selectedMsg?.id === msg.id ? '' : 'line-clamp-2'}`}>
                                                    {msg.content}
                                                </div>
                                                {selectedMsg?.id === msg.id && (
                                                    <div className="mt-4 pt-3 border-t border-gray-100 flex justify-end">
                                                        {activeTab === 'masuk' && (
                                                            <button onClick={(e) => { e.stopPropagation(); setComposeMode(true); setNewMsg({to: msg.sender, subject: `Re: ${msg.subject}`, content: `\n\n--- Pada ${new Date(msg.timestamp).toLocaleString()} ${msg.sender} menulis: ---\n${msg.content}`}); }} className="text-xs bg-purple-100 text-purple-700 px-3 py-1.5 rounded-lg font-bold hover:bg-purple-200 transition">Balas</button>
                                                        )}
                                                    </div>
                                                )}
                                            </div>
                                        ))}
                                    </div>
                                )}
                            </div>
                        </div>
                    )}
                </div>
            );
        };

        const StudentProgress = ({ db, currentUser, onUpdate }) => {
            // ... (StudentProgress component is the same)
            const studentData = (db['Mahasiswa Tugas Akhir'] || []).find(m => m.NPM === currentUser.NPM);
            
            // STATE: Gunakan nilai awal jika ada, tapi jangan reset otomatis
            const [formData, setFormData] = useState({
                judul: '',
                bimbingan: 0,
                deskripsi: ''
            });

            // STATE: Penanda apakah data awal sudah dimuat dari DB
            const [isDataLoaded, setIsDataLoaded] = useState(false);

            useEffect(() => {
                // Logika: Hanya update formData dari DB jika:
                // 1. Data mahasiswa ditemukan
                // 2. Data belum pernah dimuat sebelumnya (isDataLoaded false)
                // Ini mencegah form ter-reset saat auto-sync berjalan di background
                if (studentData && !isDataLoaded) {
                    setFormData({
                        judul: studentData.Judul || '',
                        bimbingan: studentData.BimbinganCount || 0,
                        deskripsi: studentData.ProgresDeskripsi || ''
                    });
                    setIsDataLoaded(true);
                }
            }, [studentData, isDataLoaded]);

            const handleSubmit = (e) => {
                e.preventDefault();
                if (!studentData) return alert("Data mahasiswa tidak ditemukan.");
                
                onUpdate('Mahasiswa Tugas Akhir', studentData.id, {
                    Judul: formData.judul,
                    BimbinganCount: parseInt(formData.bimbingan),
                    ProgresDeskripsi: formData.deskripsi,
                    LastUpdateProgres: new Date().toISOString()
                });
                alert("Data Skripsi & Progres berhasil diperbarui!");
            };

            if (!studentData) return <div className="p-8 text-center text-gray-500">Data mahasiswa tidak ditemukan. Hubungi admin.</div>;

            return (
                <div className="max-w-3xl mx-auto animate-fade-in">
                    <h2 className="text-2xl font-bold text-purple-900 mb-6 flex items-center gap-3">
                        <Icon path={PATHS.Chart} className="text-pink-500"/> Data & Progres Tugas Akhir
                    </h2>
                    
                    <div className="glass p-8 rounded-3xl shadow-xl border border-white/60">
                        <div className="mb-6 p-4 bg-purple-50 rounded-xl border border-purple-100 flex items-center justify-between">
                            <div>
                                <div className="text-xs font-bold text-purple-500 uppercase">Status Saat Ini</div>
                                <div className="font-bold text-lg text-purple-900">{studentData.Status || 'Belum Ada Status'}</div>
                            </div>
                            <div className="text-right">
                                <div className="text-xs font-bold text-purple-500 uppercase">Terakhir Diupdate</div>
                                <div className="text-sm font-medium text-gray-600">
                                    {studentData.LastUpdateProgres 
                                        ? new Date(studentData.LastUpdateProgres).toLocaleDateString('id-ID', {day: 'numeric', month: 'long', year: 'numeric', hour: '2-digit', minute: '2-digit'}) 
                                        : '-'}
                                </div>
                            </div>
                        </div>

                        <form onSubmit={handleSubmit} className="space-y-6">
                            {/* JUDUL SECTION (NEW) */}
                            <div>
                                <label className="text-sm font-bold text-purple-800 uppercase mb-2 block">Judul Tugas Akhir</label>
                                <textarea 
                                    className="textarea-modern min-h-[100px] font-semibold text-purple-900" 
                                    value={formData.judul} 
                                    onChange={e => setFormData({...formData, judul: e.target.value})} 
                                    placeholder="Masukkan Judul Skripsi Anda..." 
                                    required 
                                />
                                <p className="text-[10px] text-gray-500 mt-1">Pastikan judul sesuai dengan persetujuan pembimbing.</p>
                            </div>

                            <div>
                                <label className="text-sm font-bold text-purple-800 uppercase mb-2 block">Jumlah Bimbingan (Kali)</label>
                                <div className="relative">
                                    <input 
                                        type="number" 
                                        min="0"
                                        className="input-modern pl-12" 
                                        value={formData.bimbingan} 
                                        onChange={e => setFormData({...formData, bimbingan: e.target.value})} 
                                        required 
                                    />
                                    <div className="absolute left-4 top-3 text-purple-400 font-bold">#</div>
                                </div>
                                <p className="text-[10px] text-gray-500 mt-1">Total pertemuan bimbingan yang sudah dilakukan dengan pembimbing.</p>
                            </div>

                            <div>
                                <label className="text-sm font-bold text-purple-800 uppercase mb-2 block">Detail Progres Pengerjaan</label>
                                <textarea 
                                    className="textarea-modern min-h-[200px]" 
                                    value={formData.deskripsi} 
                                    onChange={e => setFormData({...formData, deskripsi: e.target.value})} 
                                    placeholder="Ceritakan sejauh mana pengerjaan skripsi Anda. Contoh: Sudah menyelesaikan Bab 3, sedang menyusun kuesioner..." 
                                    required 
                                />
                            </div>

                            <div className="pt-4 border-t border-purple-100">
                                <button type="submit" className="w-full bg-gradient-to-r from-purple-600 to-pink-600 text-white py-4 rounded-xl font-bold shadow-lg hover:shadow-purple-500/40 transition transform active:scale-95 flex items-center justify-center gap-2">
                                    <Icon path={PATHS.FileText} size={20}/> Simpan Perubahan
                                </button>
                            </div>
                        </form>
                    </div>
                </div>
            );
        };
        
        // ... (AdministrasiMenu is the same)
        const AdministrasiMenu = ({ setPage, config, userRole }) => {
            const menuItems = [
                { id: 'pengajuan_judul', label: 'Pengajuan Judul', icon: PATHS.FileText, color: 'bg-blue-100 text-blue-600', desc: 'Ajukan judul skripsi baru' },
                { id: 'sempro', label: 'Seminar Proposal', icon: PATHS.Book, color: 'bg-purple-100 text-purple-600', desc: 'Daftar ujian proposal' },
                { id: 'semhas', label: 'Seminar Hasil', icon: PATHS.Chart, color: 'bg-pink-100 text-pink-600', desc: 'Daftar ujian hasil' },
                { id: 'daftar_sidang', label: 'Sidang Akhir', icon: PATHS.Graduation, color: 'bg-emerald-100 text-emerald-600', desc: 'Daftar sidang skripsi' },
                { id: 'laporan_ta', label: 'Laporan Tugas Akhir', icon: PATHS.FileText, color: 'bg-cyan-100 text-cyan-600', desc: 'Upload laporan progres TA' }, // NEW ITEM
                { id: 'surat', label: 'Layanan Surat', icon: PATHS.Mail, color: 'bg-orange-100 text-orange-600', desc: 'Buat surat ijin riset dll' },
                { id: 'yudisium', label: 'Pendaftaran Yudisium', icon: PATHS.Tag, color: 'bg-yellow-100 text-yellow-600', desc: 'Daftar yudisium kelulusan' },
                { id: 'peminatan', label: 'Data Peminatan', icon: PATHS.Cog, color: 'bg-slate-100 text-slate-600', desc: 'Kelola data peminatan' },
            ];

            // Filter out 'peminatan' for students
            const visibleItems = menuItems.filter(item => {
                if (userRole === 'mahasiswa' && item.id === 'peminatan') return false;
                return true;
            });

            // Helper to get GForm URL
            const getGformUrl = (id) => {
                if (id === 'daftar_sidang') return config.gform_sidang;
                return config[`gform_${id}`];
            };

            return (
                <div className="space-y-8 animate-fade-in pb-20">
                    <div>
                        <h2 className="text-3xl font-bold text-purple-900 mb-2">Administrasi Akademik</h2>
                        <p className="text-purple-600">Pilih menu layanan administrasi yang tersedia di bawah ini.</p>
                    </div>

                    <div className="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6">
                        {visibleItems.map((item, idx) => {
                            const gformUrl = getGformUrl(item.id);
                            return (
                                <div key={item.id} className="relative group h-full" style={{animationDelay: `${idx * 100}ms`}}>
                                    <div className="glass p-6 rounded-3xl border border-white/60 shadow-lg hover:shadow-purple-500/20 transition duration-300 flex flex-col h-full relative overflow-hidden">
                                        
                                        {/* Main Content - Click to View Table */}
                                        <button
                                            onClick={() => setPage(item.id)}
                                            className="flex items-center gap-6 text-left flex-1 outline-none"
                                        >
                                            <div className={`absolute right-0 bottom-0 opacity-10 transform translate-x-1/4 translate-y-1/4 scale-150 group-hover:scale-175 transition duration-500 pointer-events-none`}>
                                                <Icon path={item.icon} size={100} />
                                            </div>

                                            <div className={`w-16 h-16 rounded-2xl ${item.color} flex-shrink-0 flex items-center justify-center shadow-inner group-hover:scale-110 transition duration-300`}>
                                                <Icon path={item.icon} size={32}/>
                                            </div>
                                            <div className="relative z-10">
                                                <span className="font-bold text-lg text-purple-900 group-hover:text-purple-700 transition block">{item.label}</span>
                                                <span className="text-xs text-gray-500 group-hover:text-gray-600">{item.desc}</span>
                                            </div>
                                        </button>

                                        {/* Register Button (if GForm URL exists) */}
                                        {gformUrl && (
                                            <div className="relative z-20 mt-4 pt-4 border-t border-purple-100">
                                                <a 
                                                    href={gformUrl} 
                                                    target="_blank" 
                                                    className="block w-full py-2.5 px-4 bg-gradient-to-r from-purple-600 to-indigo-600 text-white text-xs font-bold rounded-xl text-center shadow-md hover:shadow-lg hover:shadow-purple-500/30 transition transform hover:-translate-y-0.5 flex items-center justify-center gap-2"
                                                >
                                                    <Icon path={PATHS.ExternalLink} size={14}/> Daftar via GForm
                                                </a>
                                            </div>
                                        )}
                                    </div>
                                </div>
                            );
                        })}
                    </div>
                </div>
            );
        };

        const Dashboard = ({ db, userRole, currentUser }) => {
            // ... (Dashboard component is the same)
            const [greeting, setGreeting] = useState('');
            
            // Data Global (Mentah)
            const globalMhs = db['Mahasiswa Tugas Akhir'] || [];
            const rawDosen = db['Data Dosen'] || []; 
            const globalJadwal = db['Jadwal Ujian TA'] || [];
            
            // 1. Filter Data Mahasiswa (Hanya Bimbingan jika Dosen)
            const dashboardMhs = useMemo(() => {
                if (userRole === 'dosen' && currentUser?.Nama) {
                    const myName = String(currentUser.Nama).trim().toLowerCase();
                    return globalMhs.filter(m => {
                        const p1 = String(m.Pembimbing_1 || '').trim().toLowerCase();
                        const p2 = String(m.Pembimbing_2 || '').trim().toLowerCase();
                        // const penguji = String(m.Penguji || '').trim().toLowerCase(); // REMOVED: Tidak menghitung peran Penguji di Dashboard
                        return p1 === myName || p2 === myName;
                    });
                }
                return globalMhs; // Admin lihat semua
            }, [globalMhs, userRole, currentUser]);

            // 2. Hitung Beban Dosen (Tetap Global untuk Konteks)
            const allDosen = useMemo(() => {
                const counts = {};
                globalMhs.forEach(m => {
                      if(m.Pembimbing_1 && m.Pembimbing_1 !== '-' && m.Pembimbing_1.trim() !== '') {
                        const n = m.Pembimbing_1.trim();
                        counts[n] = (counts[n] || 0) + 1;
                      }
                      if(m.Pembimbing_2 && m.Pembimbing_2 !== '-' && m.Pembimbing_2.trim() !== '') {
                        const n = m.Pembimbing_2.trim();
                        counts[n] = (counts[n] || 0) + 1;
                      }
                });
                return rawDosen.map(d => ({
                    ...d,
                    Terisi: counts[d.Nama.trim()] || 0
                }));
            }, [globalMhs, rawDosen]);

            // 3. Filter Jadwal (Hanya Mahasiswa Bimbingan/Diri Sendiri jika Dosen)
            const dashboardJadwal = useMemo(() => {
                if (userRole === 'dosen' && currentUser?.Nama) {
                      const myName = String(currentUser.Nama).trim().toLowerCase();
                      const myStudentNames = new Set(dashboardMhs.map(m => m.Nama));
                      
                      return globalJadwal.filter(j => {
                          const isMyStudent = myStudentNames.has(j.Mahasiswa);
                          const isMySchedule = String(j.Penguji_1 || '').trim().toLowerCase() === myName;
                          return isMyStudent || isMySchedule;
                      });
                }
                return globalJadwal;
            }, [globalJadwal, dashboardMhs, userRole, currentUser]);

            useEffect(() => {
                const hour = new Date().getHours();
                if (hour < 11) setGreeting('Selamat Pagi');
                else if (hour < 15) setGreeting('Selamat Siang');
                else if (hour < 19) setGreeting('Selamat Sore');
                else setGreeting('Selamat Malam');
            }, []);

            const stats = {
                totalMhs: dashboardMhs.length,
                belumProposal: dashboardMhs.filter(m => m.Status === 'Belum Proposal').length,
                sempro: dashboardMhs.filter(m => m.Status === 'Sudah Proposal').length,
                semhas: dashboardMhs.filter(m => m.Status === 'Sudah Hasil').length,
                sidang: dashboardMhs.filter(m => m.Status === 'Sudah Sidang').length,
                totalDosen: allDosen.length 
            };

            const StatCard = ({ title, value, colorClass, iconClass, delay }) => (
                <div className="glass p-6 rounded-3xl shadow-lg border border-white/60 hover:transform hover:-translate-y-1 transition duration-300 relative overflow-hidden group animate-slide-up" style={{animationDelay: delay}}>
                    <div className={`absolute -right-6 -bottom-6 p-4 opacity-5 group-hover:opacity-10 transition-opacity ${iconClass} transform group-hover:scale-125 duration-500`}>
                        <Icon path={PATHS.Chart} size={100} />
                    </div>
                    <div className="text-purple-900/60 text-[10px] uppercase font-bold tracking-wider mb-2">{title}</div>
                    <div className={`text-4xl font-extrabold ${colorClass} drop-shadow-sm flex items-baseline gap-2`}>
                        {value} <span className="text-sm font-normal text-gray-400">Org</span>
                    </div>
                </div>
            );

            return (
                <div className="space-y-8 pb-24 animate-fade-in">
                    <div className="flex justify-between items-end">
                        <div>
                            <h1 className="text-3xl md:text-4xl font-bold text-purple-900 mb-1">{greeting}</h1>
                            <p className="text-purple-500 font-medium">Berikut ringkasan aktivitas akademik {userRole === 'dosen' ? 'bimbingan Anda' : 'hari ini'}.</p>
                        </div>
                        <div className="hidden md:block text-right">
                            <div className="text-2xl font-bold text-purple-800">{new Date().toLocaleDateString('id-ID', {weekday:'long', day:'numeric', month:'short'})}</div>
                        </div>
                    </div>

                    <div className="grid grid-cols-2 md:grid-cols-3 lg:grid-cols-3 gap-4 md:gap-6">
                        <StatCard title="Total Mahasiswa" value={stats.totalMhs} colorClass="text-purple-700" iconClass="text-purple-500" delay="0ms"/>
                        <StatCard title="Data Dosen" value={stats.totalDosen} colorClass="text-indigo-600" iconClass="text-indigo-500" delay="100ms"/>
                        <StatCard title="Belum Proposal" value={stats.belumProposal} colorClass="text-emerald-500" iconClass="text-emerald-500" delay="200ms"/>
                        <StatCard title="Sudah Proposal" value={stats.sempro} colorClass="text-orange-500" iconClass="text-orange-500" delay="300ms"/>
                        <StatCard title="Sudah Hasil" value={stats.semhas} colorClass="text-pink-500" iconClass="text-pink-500" delay="400ms"/>
                        <StatCard title="Sudah Sidang" value={stats.sidang} colorClass="text-rose-600" iconClass="text-rose-500" delay="500ms"/>
                    </div>

                    <div className="grid md:grid-cols-3 gap-6 md:gap-8">
                        <div className="md:col-span-2 glass p-6 md:p-8 rounded-3xl shadow-xl border border-white/60">
                            <h3 className="font-bold text-lg text-purple-900 mb-6 flex items-center gap-3">
                                <span className="p-2 bg-purple-100 text-purple-600 rounded-lg"><Icon path={PATHS.Chart}/></span> 
                                Beban Bimbingan Dosen (Global)
                            </h3>
                            <WorkloadChart dosenData={allDosen} />
                        </div>

                        <div className="bg-gradient-to-b from-slate-800 to-slate-900 text-white p-6 md:p-8 rounded-3xl shadow-2xl relative overflow-hidden flex flex-col h-96">
                            <div className="absolute top-0 right-0 w-64 h-64 bg-purple-500 opacity-20 rounded-full blur-3xl -mr-20 -mt-20"></div>
                            <h3 className="font-bold text-lg mb-6 flex items-center gap-3 relative z-10">
                                <span className="p-2 bg-white/10 rounded-lg"><Icon path={PATHS.Book}/></span>
                                Jadwal Terdekat
                            </h3>
                            <div className="space-y-3 overflow-y-auto flex-1 pr-2 custom-scrollbar relative z-10">
                                {dashboardJadwal.slice(0, 5).map((j, i) => (
                                    <div key={i} className="bg-white/5 backdrop-blur-sm p-3 rounded-xl border border-white/10 hover:bg-white/10 transition group">
                                        <div className="flex justify-between items-start mb-1">
                                            <div className="font-bold text-sm text-yellow-300 group-hover:text-yellow-200 transition">{j.Mahasiswa}</div>
                                            <span className="text-[10px] bg-purple-600 px-2 py-0.5 rounded text-white">{j.Jenis.split(' ')[1] || j.Jenis}</span>
                                        </div>
                                        <div className="text-xs text-slate-300 flex gap-3 mt-2">
                                            <span className="flex items-center gap-1"><Icon path={PATHS.Home} size={12}/> {j.Ruang}</span>
                                            <span className="flex items-center gap-1"><Icon path={PATHS.Sun} size={12}/> {j.Jam}</span>
                                        </div>
                                    </div>
                                ))}
                                {dashboardJadwal.length === 0 && <p className="text-sm text-slate-400 text-center py-10">Belum ada jadwal {userRole === 'dosen' ? 'untuk mahasiswa Anda' : ''}.</p>}
                            </div>
                        </div>
                    </div>
                </div>
            );
        };

        const App = () => {
            const [page, setPage] = useState('dashboard');
            const [userRole, setUserRole] = useState(null); 
            const [currentUser, setCurrentUser] = useState(null);
            const [showLogin, setShowLogin] = useState(false);
            const [menuOpen, setMenuOpen] = useState(false);
            const [notification, setNotification] = useState(null);
            
            const [config, setConfig] = useStickyState({ 
                app_name: 'SI Tugas Akhir FIKPsi', 
                scriptUrl: 'https://script.google.com/macros/s/AKfycby1xNCAWskg2zGUeEL1lR09yd9ozBIcymxk_-XGNlSoOA1m1mssSTle49IyeIRtgGCcUw/exec', 
                ai_api_key: '',        
                ai_key_openai: '', 
                ai_key_deepseek: '', 
                ai_key_groq: '',        
                ai_key_cohere: '',        
                ai_key_huggingface: '',
                gform_pengajuan_judul: '', 
                gform_sempro: '', 
                gform_semhas: '', 
                gform_sidang: '', 
                gform_surat: '', 
                gform_yudisium: '',
                gform_laporan_ta: '' // NEW: Config for GForm Laporan TA
            }, 'sim_config_ta_v5_FIX'); 

            // Expose 'save' from useDatabase
            const { db, add, del, update, isOnline, refresh, importBatch, batchUpdate, isLoading, isBackgroundSyncing, lastSyncTime, save } = useDatabase(INITIAL_DB, config.scriptUrl);

            // Passing simple crud object for AI
            const crud = { add, del, update };

            // --- SMART LOGIC FUNCTIONS ---

            // 1. Recalculate Dosen Quota based on active students & Auto-Create Dosen
            const recalculateDosenQuota = (mahasiswaList, dosenList) => {
                let updatedDosen = [...dosenList];
                const counts = {};
                const extractedNames = new Set();

                // 1. Hitung load & kumpulkan nama
                mahasiswaList.forEach(m => {
                    // Hitung beban dari Pembimbing 1
                    if(m.Pembimbing_1 && m.Pembimbing_1 !== '-' && m.Pembimbing_1.trim() !== '') {
                        const name = m.Pembimbing_1.trim();
                        counts[name] = (counts[name] || 0) + 1;
                        extractedNames.add(name);
                    }
                    // Hitung beban dari Pembimbing 2 (ADDED)
                    if(m.Pembimbing_2 && m.Pembimbing_2 !== '-' && m.Pembimbing_2.trim() !== '') {
                        const name = m.Pembimbing_2.trim();
                        counts[name] = (counts[name] || 0) + 1;
                        extractedNames.add(name);
                    }
                    
                    // Kumpulkan nama dari peran lain untuk sinkronisasi data dosen
                    if(m.Penguji && m.Penguji !== '-' && m.Penguji.trim() !== '') extractedNames.add(m.Penguji.trim());
                });
                
                // 2. Update kuota dosen yang sudah ada
                updatedDosen = updatedDosen.map(d => ({
                    ...d,
                    Terisi: counts[d.Nama.trim()] || 0
                }));

                // 3. Tambahkan dosen baru jika belum ada di database
                extractedNames.forEach(name => {
                    const exists = updatedDosen.some(d => d.Nama.toLowerCase().trim() === name.toLowerCase());
                    if (!exists) {
                        updatedDosen.push({
                            id: Date.now() + Math.random(),
                            Nama: name,
                            NIDN: "-", // Default
                            Keahlian: "Umum", // Default
                            Kuota: 10, // Default
                            Terisi: counts[name] || 0
                        });
                    }
                });

                return updatedDosen;
            };

            // 2. Handle Student Changes (Add/Update/Delete) -> Triggers Dosen Update
            const handleStudentChange = (action, id, data) => {
                let newMhsList = [...(db['Mahasiswa Tugas Akhir'] || [])];
                const oldDosenList = db['Data Dosen'] || [];
                
                if (action === 'add') {
                    const newItem = { id: Date.now(), ...data };
                    newMhsList.push(newItem);
                    save('create', 'Mahasiswa Tugas Akhir', newItem);
                } else if (action === 'update') {
                    newMhsList = newMhsList.map(m => m.id === id ? { ...m, ...data } : m);
                    save('update', 'Mahasiswa Tugas Akhir', { id, ...data });
                } else if (action === 'delete') {
                    newMhsList = newMhsList.filter(m => m.id !== id);
                    save('delete', 'Mahasiswa Tugas Akhir', { id });
                }

                const updatedDosen = recalculateDosenQuota(newMhsList, oldDosenList);

                // Find changed Dosen records and save them to Cloud
                updatedDosen.forEach(dNew => {
                    const dOld = oldDosenList.find(d => d.id === dNew.id);
                    // If new dosen (not in old) or Terisi count changed
                    if (!dOld) {
                        save('create', 'Data Dosen', dNew);
                    } else if (dOld.Terisi !== dNew.Terisi) {
                        save('update', 'Data Dosen', { id: dNew.id, Terisi: dNew.Terisi });
                    }
                });

                // Update Local State Immediately
                batchUpdate({
                    'Mahasiswa Tugas Akhir': newMhsList,
                    'Data Dosen': updatedDosen
                });
                
                if(action === 'add') alert('Data Mahasiswa berhasil disimpan & Kuota Dosen diperbarui!');
                if(action === 'update') alert('Data Mahasiswa berhasil diperbarui & Kuota Dosen diperbarui!');
            };

            // 3. Handle Title Submission -> Auto Creates/Updates Student
            const handlePengajuanJudul = (data) => {
                const newPengajuan = { id: Date.now(), ...data };
                const existingMhs = (db['Mahasiswa Tugas Akhir'] || []).find(m => m.NPM === data.NPM);
                let newMhsList = [...(db['Mahasiswa Tugas Akhir'] || [])];

                if (existingMhs) {
                    const updatedData = { ...existingMhs, Judul: data.Judul, Peminatan: data.Peminatan, Status: 'Belum Proposal' };
                    newMhsList = newMhsList.map(m => m.NPM === data.NPM ? updatedData : m);
                    save('update', 'Mahasiswa Tugas Akhir', updatedData); // Sync
                } else {
                    const newMhs = {
                        id: Date.now() + 1,
                        Nama: data.Nama,
                        NPM: data.NPM,
                        Prodi: "S1 Ilmu Kesehatan Masyarakat",
                        Angkatan: "20" + (data.NPM ? data.NPM.substring(2,4) : "20"), 
                        Peminatan: data.Peminatan,
                        Judul: data.Judul,
                        Status: "Belum Proposal",
                        Pembimbing_1: "-",
                        Pembimbing_2: "-"
                    };
                    newMhsList.push(newMhs);
                    save('create', 'Mahasiswa Tugas Akhir', newMhs); // Sync
                }

                save('create', 'Pengajuan Judul', newPengajuan); // Sync Pengajuan

                batchUpdate({
                    'Pengajuan Judul': [...(db['Pengajuan Judul'] || []), newPengajuan],
                    'Mahasiswa Tugas Akhir': newMhsList
                });
                alert("Pengajuan Judul tersimpan! Data Mahasiswa otomatis diperbarui ke 'Belum Proposal'.");
            };

            // 4. Handle Registration (Sempro/Semhas/Sidang) -> Updates Student Status
            const handleRegistration = (collectionName, data, targetStatus) => {
                const newReg = { id: Date.now(), ...data };
                const existingMhs = (db['Mahasiswa Tugas Akhir'] || []).find(m => m.Nama === data.Nama);
                let newMhsList = [...(db['Mahasiswa Tugas Akhir'] || [])];

                if (existingMhs) {
                    const updatedMhs = { ...existingMhs, Status: targetStatus };
                    newMhsList = newMhsList.map(m => m.id === existingMhs.id ? updatedMhs : m);
                    save('update', 'Mahasiswa Tugas Akhir', updatedMhs); // Sync Status Update
                }

                save('create', collectionName, newReg); // Sync Registration

                batchUpdate({
                    [collectionName]: [...(db[collectionName] || []), newReg],
                    'Mahasiswa Tugas Akhir': newMhsList
                });
                alert(`Pendaftaran berhasil disimpan! Status mahasiswa diperbarui menjadi '${targetStatus}'.`);
            };

            const handleRoleLogin = (role, userData = null) => {
                setUserRole(role);
                setCurrentUser(userData);
                setShowLogin(false);
                
                if (role === 'mahasiswa') {
                    setPage('sidang'); 
                } else if (role === 'tendik') {
                    setPage('informasi');
                } else {
                    setPage('dashboard'); 
                }

                // NOTIFIKASI LOGIC
                // ... (Notification logic remains same)
                const latestInfo = db['Informasi'] && db['Informasi'].length > 0 ? db['Informasi'][db['Informasi'].length - 1] : null;
                const latestJadwal = db['Jadwal Ujian TA'] && db['Jadwal Ujian TA'].length > 0 ? db['Jadwal Ujian TA'][db['Jadwal Ujian TA'].length - 1] : null;
                const unreadMsg = db['Pesan'] ? db['Pesan'].find(m => m.receiver === (userData ? userData.Nama : '') && !m.isRead) : null;

                let notifContent = null;

                if (role === 'mahasiswa' && userData) {
                    // Prioritas: Pesan Belum Dibaca -> Jadwal -> Info
                    if (unreadMsg) {
                        notifContent = {
                            type: 'Pesan Baru',
                            title: `Dari: ${unreadMsg.sender}`,
                            message: unreadMsg.content.length > 50 ? unreadMsg.content.substring(0,50) + '...' : unreadMsg.content
                        };
                    } else if (latestJadwal) {
                          notifContent = {
                            type: 'Jadwal Terbaru',
                            title: `Ujian ${latestJadwal.Jenis}`,
                            message: `${latestJadwal.Mahasiswa} akan ujian pada ${latestJadwal.Tanggal} di ${latestJadwal.Ruang}. Semangat!`
                        };
                    } else if (latestInfo) {
                        notifContent = {
                            type: 'Info Akademik',
                            title: latestInfo.Judul,
                            message: latestInfo.Isi.length > 80 ? latestInfo.Isi.substring(0, 80) + '...' : latestInfo.Isi
                        };
                    }

                } else {
                    // Untuk Dosen/Admin/Tendik: Pesan -> Info
                    if (unreadMsg) {
                        notifContent = {
                            type: 'Pesan Baru',
                            title: `Dari: ${unreadMsg.sender}`,
                            message: unreadMsg.content.length > 50 ? unreadMsg.content.substring(0,50) + '...' : unreadMsg.content
                        };
                    } else if (latestInfo) {
                        notifContent = {
                            type: 'Pengumuman Baru',
                            title: latestInfo.Judul,
                            message: latestInfo.Isi.length > 80 ? latestInfo.Isi.substring(0, 80) + '...' : latestInfo.Isi
                        };
                    }
                }

                if (notifContent) {
                    setTimeout(() => {
                        setNotification({
                            user: userData ? userData.Nama : (role === 'admin' ? 'Admin' : role === 'tendik' ? 'Staf Akademik' : 'Bapak/Ibu'), 
                            ...notifContent
                        });
                    }, 800); 
                }
            };

            const NavItem = ({ name, icon, label, onClick, isActive }) => (
                <button 
                    onClick={onClick} 
                    className={`w-full text-left px-4 py-3.5 rounded-2xl text-sm font-semibold transition-all duration-300 flex items-center justify-between mb-1.5 group
                    ${isActive
                        ? 'bg-white text-purple-700 shadow-lg shadow-purple-900/10' 
                        : 'text-purple-100/70 hover:bg-white/10 hover:text-white'
                    }`}
                >
                    <div className="flex items-center gap-3">
                        <Icon path={icon} className={isActive ? 'text-pink-500' : 'text-purple-300 group-hover:text-white'} /> {label}
                    </div>
                    {isActive && <div className="w-1.5 h-1.5 rounded-full bg-pink-500 shadow-sm"></div>}
                </button>
            );

            const dosenOptions = (db['Data Dosen'] || []).map(d => ({ value: d.Nama, label: d.Nama }));
            
            // --- NEW: Options Mahasiswa untuk Form Jadwal ---
            const mhsOptions = (db['Mahasiswa Tugas Akhir'] || [])
                .map(m => ({ value: m.Nama, label: `${m.Nama} - ${m.NPM}` }))
                .sort((a, b) => a.label.localeCompare(b.label));

            // --- NEW: Config Form Jadwal dengan Dropdown Mahasiswa ---
            const jadwalFormConfig = [
                {key:'Mahasiswa', label:'Nama Mahasiswa', type: 'select', options: mhsOptions},
                {key:'Jenis', label:'Jenis Ujian', type: 'select', options:[{value:'Seminar Proposal', label:'Sempro'}, {value:'Seminar Hasil', label:'Semhas'}, {value:'Sidang', label:'Sidang'}]},
                {key:'Tanggal', label:'Tanggal', type:'date'},
                {key:'Jam', label:'Jam'},
                {key:'Ruang', label:'Ruangan'}
            ];
            
            const mahasiswaFormConfig = [
                {key:'Nama', label:'Nama Mahasiswa'}, {key:'NPM', label:'NPM'},
                {key:'Prodi', label:'Program Studi', type: 'select', options:[
                    {value:'S1 Ilmu Kesehatan Masyarakat', label:'S1 Ilmu Kesehatan Masyarakat'}, 
                    {value:'S1 Psikologi', label:'S1 Psikologi'},
                    {value:'S2 Kesehatan Masyarakat', label:'S2 Kesehatan Masyarakat'}
                ]},
                {key:'Peminatan', label:'Peminatan', type: 'select', options: (db['Data Peminatan'] || []).map(p => ({ value: p.Nama, label: p.Nama })) },
                {key:'StatusAkademik', label:'Status Akademik', type: 'select', options:[
                    {value:'Aktif', label:'Aktif'}, 
                    {value:'Non-Aktif', label:'Non-Aktif'}, 
                    {value:'Cuti', label:'Cuti'},
                    {value:'Limit DO', label:'Limit DO'}
                ]},
                {key:'Status', label:'Tahapan', type: 'select', options:[
                    {value:'Belum Proposal', label:'Belum Proposal'}, 
                    {value:'Sudah Proposal', label:'Sudah Proposal'}, 
                    {value:'Sudah Hasil', label:'Sudah Hasil'}, 
                    {value:'Sudah Sidang', label:'Sudah Sidang'},
                    {value:'Lulus', label:'Lulus'}
                ]},
                {key:'Pembimbing_1', label:'Pembimbing 1', type: 'select', options: dosenOptions}, 
                {key:'Pembimbing_2', label:'Pembimbing 2', type: 'select', options: dosenOptions},
                {key:'Penguji', label:'Penguji', type: 'select', options: dosenOptions},
                {key:'Judul', label:'Judul Skripsi', type:'textarea'},
                {key:'LinkLaporan', label:'Link Laporan GDrive (Admin)', placeholder: 'https://...'} // Added for Admin Form
            ];

            const PAGE_MAP = {
                'pengajuan_judul': { title: 'Pengajuan Judul Skripsi', collection: 'Pengajuan Judul', configKey: 'Pengajuan Judul', status: 'Belum Proposal' },
                'sempro': { title: 'Seminar Proposal', collection: 'Pendaftaran Sempro', configKey: 'Pendaftaran Sempro', status: 'Sudah Proposal' },
                'semhas': { title: 'Seminar Hasil', collection: 'Pendaftaran Semhas', configKey: 'Pendaftaran Semhas', status: 'Sudah Hasil' },
                'daftar_sidang': { title: 'Sidang Akhir', collection: 'Pendaftaran Sidang', configKey: 'Pendaftaran Sidang', status: 'Sudah Sidang' },
                'surat': { title: 'Layanan Surat', collection: 'Layanan Surat', configKey: 'Layanan Surat', status: null }, 
                'yudisium': { title: 'Pendaftaran Yudisium', collection: 'Data Yudisium', configKey: 'Data Yudisium', status: null },
                'peminatan': { title: 'Data Peminatan', collection: 'Data Peminatan', configKey: 'Data Peminatan', status: null },
                'laporan_ta': { title: 'Laporan Tugas Akhir', collection: 'Laporan TA', configKey: 'Laporan TA', status: null } 
            };
            
            // --- NEW: Jadwal Data Definition with useMemo ---
            // UPDATED: Menambahkan Pembimbing 2 dan Penguji ke detail jadwal
            const jadwalData = useMemo(() => {
                return (db['Jadwal Ujian TA'] || []).map(j => {
                    const mhs = (db['Mahasiswa Tugas Akhir'] || []).find(m => m.Nama === j.Mahasiswa);
                    if (mhs) {
                        return { 
                            ...j, 
                            "Judul Tugas Akhir": mhs.Judul, 
                            "Pembimbing 1": mhs.Pembimbing_1,
                            "Pembimbing 2": mhs.Pembimbing_2, // Ditambahkan
                            "Penguji Mahasiswa": mhs.Penguji      // Ditambahkan (Penguji dari data mahasiswa)
                        };
                    }
                    return j;
                });
            }, [db]);

            // Helper to get GForm URL safely
            const getGformUrl = (pageId) => {
                if (pageId === 'daftar_sidang') return config.gform_sidang;
                return config[`gform_${pageId}`];
            }

            if (!userRole) {
                return (
                    <div className="flex items-center justify-center min-h-screen relative overflow-hidden">
                        <LoginCard isModal={false} db={db} handleRoleLogin={handleRoleLogin} setShowLogin={setShowLogin} onRefresh={refresh} isLoading={isLoading}/>
                    </div>
                )
            }

            const Sidebar = () => (
                <>
                    <div className={`fixed inset-0 bg-purple-900/40 backdrop-blur-sm z-30 md:hidden transition-opacity duration-300 ${menuOpen ? 'opacity-100' : 'opacity-0 pointer-events-none'}`} onClick={()=>setMenuOpen(false)}/>
                    <div className={`w-72 bg-[#2d0f59]/90 backdrop-filter backdrop-blur-xl h-screen fixed top-0 left-0 border-r border-white/10 flex flex-col z-40 transform transition-transform duration-300 ease-out md:translate-x-0 ${menuOpen ? 'translate-x-0' : '-translate-x-full'} shadow-2xl`}>
                        <div className="p-8 pb-6">
                            <div className="w-10 h-10 bg-gradient-to-tr from-pink-500 to-purple-600 rounded-xl mb-4 flex items-center justify-center text-white shadow-lg shadow-purple-500/30">
                                <Icon path={PATHS.Graduation} size={24}/>
                            </div>
                            <div className="font-extrabold text-2xl text-white tracking-tight leading-none">SI TA <span className="text-purple-400">FIKPsi</span></div>
                            <div className="text-[10px] font-bold text-purple-400/60 uppercase tracking-widest mt-1">Integrated System</div>
                        </div>
                        <nav className="flex-1 px-4 py-2 overflow-y-auto custom-scrollbar space-y-1">
                            {(userRole === 'admin' || userRole === 'dosen') && (
                                <NavItem name="dashboard" icon={PATHS.Home} label="Dashboard" onClick={()=>{setPage('dashboard'); setMenuOpen(false)}} isActive={page==='dashboard'}/>
                            )}
                            {(userRole === 'admin' || userRole === 'dosen') && (
                                <NavItem name="mahasiswa" icon={PATHS.Users} label="Data Mahasiswa" onClick={()=>{setPage('mahasiswa'); setMenuOpen(false)}} isActive={page==='mahasiswa'}/>
                            )}
                            {/* NEW: Menu Tugas Akhir Mahasiswa for Dosen */}
                            {userRole === 'dosen' && (
                                <NavItem name="tugas_akhir" icon={PATHS.FileText} label="Tugas Akhir Mahasiswa" onClick={()=>{setPage('tugas_akhir'); setMenuOpen(false)}} isActive={page==='tugas_akhir'}/>
                            )}
                            {userRole === 'admin' && (
                                <>
                                    <NavItem name="dosen" icon={PATHS.User} label="Data Dosen" onClick={()=>{setPage('dosen'); setMenuOpen(false)}} isActive={page==='dosen'}/>
                                    <NavItem name="peminatan" icon={PATHS.Cog} label="Data Peminatan" onClick={()=>{setPage('peminatan'); setMenuOpen(false)}} isActive={page==='peminatan'}/>
                                </>
                            )}
                            <NavItem name="informasi" icon={PATHS.Bell} label="Informasi" onClick={()=>{setPage('informasi'); setMenuOpen(false)}} isActive={page==='informasi'}/>
                            {/* UPDATED: Dosen ditambahkan ke akses menu Jadwal Ujian */}
                            {(userRole === 'admin' || userRole === 'mahasiswa' || userRole === 'tendik' || userRole === 'dosen') && (
                                <NavItem name="sidang" icon={PATHS.Sun} label="Jadwal Ujian" onClick={()=>{setPage('sidang'); setMenuOpen(false)}} isActive={page==='sidang'}/>
                            )}
                            {(userRole === 'admin' || userRole === 'mahasiswa') && (
                                <NavItem name="administrasi" icon={PATHS.Clip} label="Administrasi" onClick={()=>{setPage('administrasi'); setMenuOpen(false)}} isActive={page === 'administrasi' || Object.keys(PAGE_MAP).includes(page)}/>
                            )}
                            {(userRole === 'admin' || userRole === 'dosen' || userRole === 'mahasiswa') && (
                                <NavItem name="unduh" icon={PATHS.Cloud} label="Pusat Unduhan" onClick={()=>{setPage('unduh'); setMenuOpen(false)}} isActive={page==='unduh'}/>
                            )}
                            {userRole === 'mahasiswa' && (
                                <NavItem name="progres" icon={PATHS.Chart} label="Lapor Progres" onClick={()=>{setPage('progres'); setMenuOpen(false)}} isActive={page==='progres'}/>
                            )}
                            
                            <div className="pt-4 mt-2 mb-2 border-t border-white/10">
                                <p className="px-4 text-[10px] font-bold text-purple-400/50 uppercase tracking-widest mb-2">Komunikasi</p>
                                <NavItem name="pesan" icon={PATHS.Mail} label="Kotak Masuk" onClick={()=>{setPage('pesan'); setMenuOpen(false)}} isActive={page==='pesan'}/>
                            </div>
                        </nav>
                        
                        <div className="px-6 py-2">
                             <div className="flex items-center justify-between text-[10px] text-purple-300 bg-white/5 rounded-lg p-2 border border-white/5">
                                 <div className="flex items-center gap-2">
                                     <div className={`w-2 h-2 rounded-full ${isOnline ? 'bg-green-500 animate-pulse' : 'bg-red-500'}`}></div>
                                     {isBackgroundSyncing ? 'Menyimpan...' : (isOnline ? 'Live Sync' : 'Offline')}
                                 </div>
                                 <div className="opacity-60">{lastSyncTime ? lastSyncTime.toLocaleTimeString([], {hour: '2-digit', minute:'2-digit'}) : '--:--'}</div>
                             </div>
                        </div>

                        <div className="p-6 bg-black/20 mx-4 mb-4 rounded-2xl border border-white/5">
                            <div className="flex items-center gap-3 mb-3">
                                <div className="w-8 h-8 rounded-full bg-gradient-to-br from-purple-400 to-pink-400 flex items-center justify-center text-white text-xs font-bold">
                                    {userRole.charAt(0).toUpperCase()}
                                </div>
                                <div>
                                    <div className="text-white text-sm font-bold capitalize">{currentUser ? currentUser.Nama : userRole}</div>
                                    <div className="text-purple-400 text-[10px]">{userRole}</div>
                                </div>
                            </div>
                            <button onClick={()=>{setShowLogin(true); setMenuOpen(false)}} className="w-full py-2 bg-white/10 hover:bg-white/20 rounded-lg text-xs font-bold text-white transition flex items-center justify-center gap-2">
                                <Icon path={PATHS.Logout} size={14}/> Keluar / Ganti
                            </button>
                            {userRole === 'admin' && (
                                <button onClick={()=>{setPage('settings'); setMenuOpen(false)}} className="mt-2 w-full text-center text-[10px] text-purple-400 hover:text-white transition flex justify-center gap-1 items-center"><Icon path={PATHS.Cog} size={10}/> Pengaturan</button>
                            )}
                        </div>
                    </div>
                </>
            );

            return (
                <div className="flex min-h-screen relative">
                    <Sidebar/>
                    <div className="md:hidden fixed top-0 w-full glass z-20 px-6 py-4 flex justify-between items-center shadow-sm">
                         <div className="font-extrabold text-lg text-purple-800 flex items-center gap-2">
                            <div className="w-6 h-6 bg-pink-500 rounded-lg"></div> FIKPsi Sys
                         </div>
                         <button onClick={()=>setMenuOpen(true)} className="p-2 text-purple-600 bg-white rounded-xl shadow-sm border border-purple-100 active:scale-95 transition"><Icon path={PATHS.Menu} size={24}/></button>
                    </div>

                    <main className="flex-1 md:ml-72 p-4 md:p-8 pt-24 md:pt-10 h-screen overflow-y-auto touch-scroll">
                        {page === 'dashboard' && <Dashboard db={db} userRole={userRole} currentUser={currentUser}/>}
                        
                        {/* MAHASISWA PAGE */}
                        {page === 'mahasiswa' && <GenericTable 
                            key="tbl-mhs"
                            title="Data Mahasiswa & TA" 
                            data={(() => {
                                // 1. Ambil Data Mentah
                                let rawData = db['Mahasiswa Tugas Akhir'] || [];
                                
                                // 2. Filter Khusus Dosen (Case Insensitive & Trimmed)
                                if (userRole === 'dosen' && currentUser?.Nama) {
                                    const myName = String(currentUser.Nama).trim().toLowerCase();
                                    rawData = rawData.filter(m => {
                                        const p1 = String(m.Pembimbing_1 || '').trim().toLowerCase();
                                        const p2 = String(m.Pembimbing_2 || '').trim().toLowerCase();
                                        const penguji = String(m.Penguji || '').trim().toLowerCase();
                                        return p1 === myName || p2 === myName || penguji === myName;
                                    });
                                }

                                // 3. Deduplikasi Data berdasarkan NPM (Mencegah Double)
                                // Menggunakan Map: Jika ada NPM sama, data terakhir yang akan diambil (terupdate)
                                const uniqueData = new Map();
                                rawData.forEach(item => {
                                    if (item.NPM) {
                                        uniqueData.set(String(item.NPM).trim(), item);
                                    } else {
                                        // Jika tidak ada NPM, gunakan ID sebagai fallback key agar tidak hilang
                                        uniqueData.set(item.id, item); 
                                    }
                                });

                                return Array.from(uniqueData.values());
                            })()}
                            columns={TABLE_CONFIG['Mahasiswa Tugas Akhir'].columns} 
                            formConfig={mahasiswaFormConfig} 
                            onAdd={(d) => handleStudentChange('add', null, d)} 
                            onDel={(id) => handleStudentChange('delete', id)} 
                            onUpdate={(id, d) => handleStudentChange('update', id, d)}
                            onImport={data => importBatch('Mahasiswa Tugas Akhir', data)}
                            allowAdd={userRole==='admin'} 
                            allowDelete={userRole==='admin'}
                            allowEdit={userRole==='admin'}
                            allowImport={userRole==='admin'}
                            statusFilterConfig={{
                                key: 'Status',
                                options: ['Belum Proposal', 'Sudah Proposal', 'Sudah Hasil', 'Sudah Sidang', 'Lulus']
                            }}
                        />}
                        
                        {/* NEW: TUGAS AKHIR MAHASISWA PAGE FOR DOSEN */}
                        {page === 'tugas_akhir' && userRole === 'dosen' && <GenericTable 
                            key="tbl-ta-dosen"
                            title="Tugas Akhir Mahasiswa (Detail)" 
                            data={(() => {
                                let rawData = db['Mahasiswa Tugas Akhir'] || [];
                                const myName = String(currentUser.Nama).trim().toLowerCase();
                                // Filter students where dosen is supervisor or examiner
                                rawData = rawData.filter(m => {
                                    const p1 = String(m.Pembimbing_1 || '').trim().toLowerCase();
                                    const p2 = String(m.Pembimbing_2 || '').trim().toLowerCase();
                                    const penguji = String(m.Penguji || '').trim().toLowerCase();
                                    return p1 === myName || p2 === myName || penguji === myName;
                                });
                                // Deduplicate
                                const uniqueData = new Map();
                                rawData.forEach(item => {
                                    if (item.NPM) uniqueData.set(String(item.NPM).trim(), item);
                                    else uniqueData.set(item.id, item);
                                });
                                return Array.from(uniqueData.values());
                            })()}
                            columns={TABLE_CONFIG['Tugas Akhir Mahasiswa (Dosen)'].columns} 
                            formConfig={[]} // Read only
                            allowAdd={false} 
                            allowDelete={false}
                            allowEdit={false} // Only admin edits link
                            allowImport={false}
                        />}

                        {page === 'dosen' && <GenericTable 
                            key="tbl-dosen"
                            title="Data Dosen" 
                            data={db['Data Dosen']} 
                            columns={TABLE_CONFIG['Data Dosen'].columns} 
                            formConfig={TABLE_CONFIG['Data Dosen'].form} 
                            onAdd={d=>add('Data Dosen',d)} 
                            onDel={id=>del('Data Dosen',id)} 
                            onUpdate={(id, d)=>update('Data Dosen', id, d)}
                            onImport={data=>importBatch('Data Dosen', data)} 
                            allowAdd={userRole==='admin'} 
                            allowDelete={userRole==='admin'} 
                            allowEdit={userRole==='admin'} 
                            allowImport={userRole==='admin'}
                        />}

                        {page === 'peminatan' && <GenericTable 
                            key="tbl-peminatan"
                            title="Data Peminatan" 
                            data={db['Data Peminatan']} 
                            columns={TABLE_CONFIG['Data Peminatan'].columns} 
                            formConfig={TABLE_CONFIG['Data Peminatan'].form} 
                            onAdd={d=>add('Data Peminatan',d)} 
                            onDel={id=>del('Data Peminatan',id)} 
                            onUpdate={(id, d)=>update('Data Peminatan', id, d)}
                            allowAdd={userRole==='admin'} 
                            allowDelete={userRole==='admin'} 
                            allowEdit={userRole==='admin'}
                        />}
                        
                        {page === 'sidang' && <GenericTable 
                            key="tbl-sidang"
                            title="Jadwal Ujian" 
                            // UPDATED: Filter Jadwal Ujian khusus Dosen (Pembimbing 1, Pembimbing 2, atau Penguji)
                            data={(() => {
                                let data = jadwalData;
                                if (userRole === 'dosen' && currentUser?.Nama) {
                                     const myName = String(currentUser.Nama).trim().toLowerCase();
                                     data = data.filter(j => {
                                         const p1 = String(j["Pembimbing 1"] || '').trim().toLowerCase();
                                         const p2 = String(j["Pembimbing 2"] || '').trim().toLowerCase();
                                         const pengujiMhs = String(j["Penguji Mahasiswa"] || '').trim().toLowerCase();
                                         const pengujiJadwal = String(j.Penguji_1 || '').trim().toLowerCase();

                                         // Tampilkan jika Dosen adalah P1, P2, Penguji (di data Mhs), atau Penguji (di Jadwal)
                                         return p1 === myName || p2 === myName || pengujiMhs === myName || pengujiJadwal === myName;
                                     });
                                }
                                return data;
                            })()} 
                            columns={TABLE_CONFIG['Jadwal Ujian TA'].columns} 
                            formConfig={jadwalFormConfig} 
                            onAdd={d=>add('Jadwal Ujian TA',d)} 
                            onDel={id=>del('Jadwal Ujian TA',id)} 
                            onImport={data=>importBatch('Jadwal Ujian TA', data)}
                            allowAdd={userRole==='admin' || userRole==='tendik'} 
                            allowDelete={userRole==='admin' || userRole==='tendik'}
                            allowImport={userRole==='admin'}
                        />}
                        
                        {page === 'informasi' && <GenericTable 
                            key="tbl-info"
                            title="Papan Informasi & Pengumuman" 
                            data={db['Informasi'] || []} 
                            columns={TABLE_CONFIG['Informasi'].columns} 
                            formConfig={TABLE_CONFIG['Informasi'].form} 
                            onAdd={d => add('Informasi', { ...d, Penulis: currentUser?.Nama || (userRole === 'admin' ? 'Admin' : 'Staf') })} 
                            onDel={id=>del('Informasi',id)} 
                            onUpdate={(id, d)=>update('Informasi', id, d)}
                            allowAdd={userRole==='admin' || userRole==='dosen' || userRole==='tendik'} 
                            allowDelete={userRole==='admin' || userRole==='dosen' || userRole==='tendik'}
                            allowEdit={userRole==='admin' || userRole==='dosen' || userRole==='tendik'}
                        />}

                        {page === 'administrasi' && <AdministrasiMenu setPage={setPage} config={config} userRole={userRole} />}
                        
                        {PAGE_MAP[page] && (
                            <GenericTable 
                                key={`tbl-admin-${page}`}
                                title={PAGE_MAP[page].title}
                                data={db[PAGE_MAP[page].collection] || []}
                                columns={TABLE_CONFIG[PAGE_MAP[page].configKey].columns}
                                formConfig={TABLE_CONFIG[PAGE_MAP[page].configKey].form}
                                onAdd={(d) => {
                                    if(page === 'pengajuan_judul') {
                                        handlePengajuanJudul(d);
                                    } else if(PAGE_MAP[page].status) {
                                        handleRegistration(PAGE_MAP[page].collection, d, PAGE_MAP[page].status);
                                    } else {
                                        add(PAGE_MAP[page].collection, d);
                                        alert('Data Tersimpan!');
                                    }
                                }}
                                onDel={id=>del(PAGE_MAP[page].collection, id)}
                                onImport={data=>importBatch(PAGE_MAP[page].collection, data)}
                                allowAdd={userRole==='admin'} 
                                allowDelete={userRole==='admin'}
                                allowImport={userRole==='admin'}
                                gformUrl={getGformUrl(page)}
                                onBack={()=>setPage('administrasi')}
                            />
                        )}

                        {page === 'unduh' && <GenericTable
                            key="tbl-unduh"
                            title="Pusat Unduhan Berkas"
                            data={db['Data Unduhan'] || []}
                            columns={TABLE_CONFIG['Data Unduhan'].columns}
                            formConfig={TABLE_CONFIG['Data Unduhan'].form}
                            onAdd={d=>add('Data Unduhan',d)}
                            onDel={id=>del('Data Unduhan',id)}
                            onImport={data=>importBatch('Data Unduhan', data)}
                            allowAdd={userRole==='admin'}
                            allowDelete={userRole==='admin'}
                            allowImport={userRole==='admin'}
                        />}

                        {page === 'progres' && userRole === 'mahasiswa' && (
                            <StudentProgress db={db} currentUser={currentUser} onUpdate={(collection, id, data) => update(collection, id, data)} />
                        )}

                        {page === 'pesan' && (
                            <InboxSystem db={db} currentUser={currentUser} role={userRole} onSend={(msg) => { add('Pesan', msg); alert('Pesan terkirim!'); }} />
                        )}
                        
                        {page === 'settings' && userRole === 'admin' && (
                            <div className="max-w-lg mx-auto glass p-8 rounded-3xl shadow-xl border border-white/60 animate-slide-up">
                                <h2 className="text-2xl font-bold mb-8 text-purple-900 text-center flex items-center justify-center gap-2"><Icon path={PATHS.Cog}/> Pengaturan Sistem</h2>
                                <div className="space-y-5">
                                    <div><label className="text-xs font-bold text-purple-800/70 uppercase mb-2 block">Nama Aplikasi</label><input className="input-modern" value={config.app_name} onChange={e=>setConfig(p=>({...p,app_name:e.target.value}))}/></div>
                                    <div><label className="text-xs font-bold text-purple-800/70 uppercase mb-2 block">Google Sheet Script URL</label><input className="input-modern" placeholder="https://script.google.com/..." value={config.scriptUrl} onChange={e=>setConfig(p=>({...p,scriptUrl:e.target.value}))}/></div>
                                    <div className="pt-4 border-t border-purple-100">
                                        <p className="text-sm font-bold text-purple-900 mb-4">Link Google Form (Pendaftaran)</p>
                                        <div className="grid grid-cols-2 gap-3">
                                            <div className="col-span-2"><label className="text-[10px] font-bold text-purple-500 uppercase block">Form Pengajuan Judul</label><input className="input-modern" value={config.gform_pengajuan_judul || ''} onChange={e=>setConfig(p=>({...p,gform_pengajuan_judul:e.target.value}))}/></div>
                                            <div><label className="text-[10px] font-bold text-purple-500 uppercase block">Form Sempro</label><input className="input-modern" value={config.gform_sempro || ''} onChange={e=>setConfig(p=>({...p,gform_sempro:e.target.value}))}/></div>
                                            <div><label className="text-[10px] font-bold text-purple-500 uppercase block">Form Semhas</label><input className="input-modern" value={config.gform_semhas || ''} onChange={e=>setConfig(p=>({...p,gform_semhas:e.target.value}))}/></div>
                                            <div><label className="text-[10px] font-bold text-purple-500 uppercase block">Form Sidang</label><input className="input-modern" value={config.gform_sidang || ''} onChange={e=>setConfig(p=>({...p,gform_sidang:e.target.value}))}/></div>
                                            <div><label className="text-[10px] font-bold text-purple-500 uppercase block">Form Surat</label><input className="input-modern" value={config.gform_surat || ''} onChange={e=>setConfig(p=>({...p,gform_surat:e.target.value}))}/></div>
                                            <div><label className="text-[10px] font-bold text-purple-500 uppercase block">Form Yudisium</label><input className="input-modern" value={config.gform_yudisium || ''} onChange={e=>setConfig(p=>({...p,gform_yudisium:e.target.value}))}/></div>
                                            <div><label className="text-[10px] font-bold text-purple-500 uppercase block">Form Laporan TA</label><input className="input-modern" value={config.gform_laporan_ta || ''} onChange={e=>setConfig(p=>({...p,gform_laporan_ta:e.target.value}))}/></div>
                                        </div>
                                    </div>
                                    <button onClick={()=>{refresh(); alert('Pengaturan Disimpan!')}} className="w-full bg-purple-600 text-white py-3.5 rounded-xl font-bold hover:bg-purple-700 transition shadow-lg shadow-purple-500/30">Simpan & Refresh</button>
                                </div>
                            </div>
                        )}
                    </main>

                    {showLogin && (
                        <div className="fixed inset-0 bg-purple-900/40 backdrop-blur-md flex items-center justify-center z-50 p-4 animate-fade-in">
                            <LoginCard isModal={true} db={db} handleRoleLogin={handleRoleLogin} setShowLogin={setShowLogin} onRefresh={refresh} isLoading={isLoading} />
                        </div>
                    )}

                    {notification && (
                        <NotificationPopup data={notification} onClose={() => setNotification(null)} />
                    )}
                </div>
            );
        };

        const root = ReactDOM.createRoot(document.getElementById('root'));
        root.render(<App />);
    </script>
</body>
</html>
