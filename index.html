import React, { useState, useEffect, useMemo, useRef, useId } from 'react';
import { initializeApp } from 'firebase/app';
import { getAuth, signInAnonymously, onAuthStateChanged } from 'firebase/auth';
import { getFirestore, collection, onSnapshot, addDoc, deleteDoc, doc } from 'firebase/firestore';
import { 
  Home, Users, Building, Bell, LogIn, LogOut, Plus, Mail, Phone, 
  ChevronRight, ChevronLeft, Menu, X, Briefcase, DollarSign, Wrench, Eye, Flag, 
  Layers, Search, Filter, Calendar, Clock, User, AlertTriangle, Target,
  BarChart2, PieChart, TrendingUp, ChevronDown, ChevronUp, RotateCcw,
  MapPin, List, ZoomIn, ZoomOut, CheckCircle2, EyeOff, Download, Printer,
  ShieldCheck, Activity, CheckSquare, Globe, ExternalLink, Image as ImageIcon,
  Upload, Award, Star, History, Sparkles, Trash2, Edit3, Lock, Send,
  Volume2, Pause, Play
} from 'lucide-react';

// --- LOGO RASMI RISDA PAHANG & BANGUNAN PRN PAHANG (LOKAL + SANDARAN GOOGLE DRIVE) ---
const LOGO_HPC_DRIVE_ID = '1lee56ZbBsRbYAjg4V48vp7ROVcQF8vE1';
const LOGO_CREST_DRIVE_ID = '12QAe7WTrkpBDVW2kc48YnB5XjvOH9H6z';
const BANGUNAN_PRN_DRIVE_ID = '1n9Bh5nT3ylkqobJ2AVSvaAQvCFItcnZf';

const LOGO_HPC_URL = '/LOGO HPC BLACK.png';
const LOGO_CREST_URL = '/Logo RISDA Emas 2025.png';
const BANGUNAN_PRN_PRIMARY_URL = '/prn-pahang.jpg';
const BANGUNAN_PRN_URL = '/bangunan-risda.jpg';
const BANGUNAN_PRN_ALT_URL = '/Building Pahang.jpg';

// Komponen Paparan Logo RISDA terus menggunakan imej asal Google Drive / Lokal
const RisdaDriveLogo = ({ className = "h-12 w-auto", showGlow = true, isSecond = false }) => {
  const [imgStep, setImgStep] = useState(0);
  const driveId = isSecond ? LOGO_CREST_DRIVE_ID : LOGO_HPC_DRIVE_ID;
  const localFileUrl = isSecond ? LOGO_CREST_URL : LOGO_HPC_URL;
  const legacyLocalUrl = isSecond ? '/logo-second.png' : '/logo-gold.png';

  // Keutamaan pada pautan Google Drive & fail lokal sebenar supaya rupa asal logo dalam Drive dikekalkan
  const imageSources = [
    `https://drive.google.com/thumbnail?id=${driveId}&sz=w1000`,
    `https://lh3.googleusercontent.com/d/${driveId}`,
    `https://drive.usercontent.google.com/download?id=${driveId}&export=view`,
    localFileUrl,
    legacyLocalUrl
  ];

  const activeSrc = imageSources[imgStep] || imageSources[0];

  return (
    <img 
      src={activeSrc} 
      alt={isSecond ? "Logo RISDA Emas 2025" : "Logo HPC RISDA"} 
      referrerPolicy="no-referrer"
      className={`${className} object-contain ${showGlow ? 'filter drop-shadow-[0_4px_10px_rgba(234,179,8,0.45)]' : ''} transition-transform duration-300`}
      onError={() => {
        if (imgStep + 1 < imageSources.length) {
          setImgStep(prev => prev + 1);
        }
      }}
      loading="eager"
    />
  );
};

// --- KOMPONEN LOGO RISDA BUDAYA BERPRESTASI TINGGI (VEKTOR TULEN LUAR TALIAN) ---
const RisdaHpcLogo = ({ className = "h-12 w-auto", showGlow = true }) => {
  const uid = useId().replace(/:/g, '');
  const gradId = `hpcGoldGrad_${uid}`;

  return (
    <svg viewBox="0 0 420 150" className={`${className} ${showGlow ? 'filter drop-shadow-[0_4px_10px_rgba(234,179,8,0.4)]' : ''}`} fill="none" xmlns="http://www.w3.org/2000/svg">
      <defs>
        <linearGradient id={gradId} x1="0%" y1="0%" x2="100%" y2="100%">
          <stop offset="0%" stopColor="#FEF08A" />
          <stop offset="45%" stopColor="#EAB308" />
          <stop offset="85%" stopColor="#CA8A04" />
          <stop offset="100%" stopColor="#A16207" />
        </linearGradient>
      </defs>
      {/* Ikon Daun Getah Emas */}
      <g fill={`url(#${gradId})`}>
        <path d="M 30 92 C 24 64 38 36 66 22 L 58 56 L 30 92 Z" />
        <path d="M 72 20 C 92 12 116 11 136 16 C 114 29 90 42 66 53 L 72 20 Z" />
        <path d="M 35 97 L 68 62 L 106 46 C 95 62 77 75 54 84 L 35 97 Z" />
        <path d="M 42 102 L 66 86 C 86 79 104 70 118 57 C 106 82 82 99 54 104 C 49 105 45 104 42 102 Z" />
      </g>
      {/* Teks RISDA Rapat & Kemas */}
      <g fill={`url(#${gradId})`} fontFamily="Arial Black, Impact, sans-serif" fontWeight="900" fontSize="58">
        <text x="126" y="88">RIS</text>
        <text x="304" y="88">A</text>
      </g>
      {/* Huruf D Bersepadu Dengan Meter Prestasi Tanpa Kotak Hitam */}
      <g transform="translate(245, 40)">
        <path d="M 0 0 H 22 C 44 0 56 11 56 24 C 56 37 44 48 22 48 H 0 Z" stroke={`url(#${gradId})`} strokeWidth="8" fill="none" strokeLinejoin="round" />
        <path d="M 15 35 A 16 16 0 0 1 25 11" stroke="#ef4444" strokeWidth="4.5" strokeLinecap="round" fill="none" />
        <path d="M 28 11 A 16 16 0 0 1 41 20" stroke="#f59e0b" strokeWidth="4.5" strokeLinecap="round" fill="none" />
        <path d="M 42 23 A 16 16 0 0 1 38 37" stroke="#22c55e" strokeWidth="4.5" strokeLinecap="round" fill="none" />
        <line x1="25" y1="31" x2="38" y2="16" stroke="#FFFFFF" strokeWidth="3" strokeLinecap="round" />
        <circle cx="25" cy="31" r="4" fill="#FEF08A" />
      </g>
      {/* Slogan Bawah */}
      <text x="215" y="116" fill="#FFFFFF" fontFamily="Arial, sans-serif" fontWeight="900" fontSize="16.5" letterSpacing="1.8" textAnchor="middle">
        BUDAYA BERPRESTASI TINGGI
      </text>
      <line x1="48" y1="132" x2="96" y2="132" stroke="#94A3B8" strokeWidth="1.5" />
      <text x="215" y="136" fill="#CBD5E1" fontFamily="Arial, sans-serif" fontWeight="700" fontSize="11" letterSpacing="2.8" textAnchor="middle">
        HIGH PERFORMANCE CULTURE
      </text>
      <line x1="334" y1="132" x2="382" y2="132" stroke="#94A3B8" strokeWidth="1.5" />
    </svg>
  );
};

// --- KOMPONEN LOGO BULAT RASMI RISDA (VEKTOR TULEN LUAR TALIAN) ---
const RisdaGoldLogo = ({ className = "h-12 w-auto", showGlow = true }) => {
  const uid = useId().replace(/:/g, '');
  const goldGradId = `goldGrad_${uid}`;
  const goldLightId = `goldLight_${uid}`;
  const textArcId = `risdaTextArc_${uid}`;

  return (
    <svg viewBox="0 0 500 500" className={`${className} ${showGlow ? 'filter drop-shadow-[0_4px_8px_rgba(234,179,8,0.5)]' : ''}`} fill="none" xmlns="http://www.w3.org/2000/svg">
      <defs>
        <linearGradient id={goldGradId} x1="0%" y1="0%" x2="100%" y2="100%">
          <stop offset="0%" stopColor="#FEF08A" />
          <stop offset="35%" stopColor="#EAB308" />
          <stop offset="75%" stopColor="#CA8A04" />
          <stop offset="100%" stopColor="#A16207" />
        </linearGradient>
        <linearGradient id={goldLightId} x1="0%" y1="0%" x2="0%" y2="100%">
          <stop offset="0%" stopColor="#FEF9C3" />
          <stop offset="100%" stopColor="#EAB308" />
        </linearGradient>
        <path id={textArcId} d="M 42 215 A 210 210 0 1 0 458 215" fill="none" />
      </defs>

      <circle cx="250" cy="250" r="240" fill="#1e3a8a" fillOpacity="0.25" stroke={`url(#${goldGradId})`} strokeWidth="10" />
      <circle cx="250" cy="250" r="190" stroke={`url(#${goldGradId})`} strokeWidth="4" strokeOpacity="0.85" />

      <text fill={`url(#${goldLightId})`} fontSize="15.5" fontWeight="900" letterSpacing="2.1" fontFamily="Arial, sans-serif">
        <textPath href={`#${textArcId}`} startOffset="50%" textAnchor="middle">
          PIHAK BERKUASA KEMAJUAN PEKEBUN KECIL PERUSAHAAN GETAH
        </textPath>
      </text>

      <g fill={`url(#${goldGradId})`}>
        <path d="M 250 38 C 224 76 214 122 250 168 C 286 122 276 76 250 38 Z" />
        <path d="M 164 112 C 162 138 196 180 240 188 C 234 150 196 116 164 112 Z" />
        <path d="M 336 112 C 338 138 304 180 260 188 C 266 150 304 116 336 112 Z" />
      </g>
      <g stroke="#1e3a8a" strokeWidth="3.5" strokeLinecap="round">
        <line x1="250" y1="54" x2="250" y2="162" />
        <line x1="250" y1="84" x2="235" y2="70" />
        <line x1="250" y1="84" x2="265" y2="70" />
        <line x1="250" y1="112" x2="232" y2="96" />
        <line x1="250" y1="112" x2="268" y2="96" />
        <line x1="174" y1="120" x2="236" y2="182" />
        <line x1="326" y1="120" x2="264" y2="182" />
      </g>

      <path d="M 92 192 C 114 342 386 342 408 192 C 358 228 298 242 250 242 C 202 242 142 228 92 192 Z" fill={`url(#${goldGradId})`} />
      <path d="M 96 184 C 118 334 382 334 404 184" stroke={`url(#${goldLightId})`} strokeWidth="7" fill="none" />

      <path d="M 235 246 L 265 246 L 258 296 L 242 296 Z" fill="#FFFFFF" />
      <g stroke="#A16207" strokeWidth="2.5" strokeLinecap="round">
        <path d="M 237 256 Q 250 253 263 256" fill="none" />
        <path d="M 239 266 Q 250 263 261 266" fill="none" />
        <path d="M 240 276 Q 250 273 260 276" fill="none" />
        <path d="M 241 286 Q 250 283 259 286" fill="none" />
      </g>
      <path d="M 204 294 Q 218 326 250 326 Q 282 326 296 294 Q 266 310 250 310 Q 234 310 204 294 Z" fill="#FFFFFF" />

      <text
        x="250"
        y="374"
        fill="#FFFFFF"
        fontSize="46"
        fontWeight="900"
        fontFamily="Arial Black, Arial, sans-serif"
        letterSpacing="3"
        textAnchor="middle"
      >
        RISDA
      </text>
    </svg>
  );
};

// --- FIREBASE INITIALIZATION (SELAMAT UNTUK LOCALHOST & VITE) ---
const firebaseConfig = {
  apiKey: "demo-api-key",
  authDomain: "demo-app.firebaseapp.com",
  projectId: "demo-app",
  storageBucket: "demo-app.appspot.com",
  messagingSenderId: "123456789",
  appId: "demo-app-id"
};

let app = null;
let auth = null;
let db = null;
try {
  app = initializeApp(firebaseConfig);
  auth = getAuth(app);
  db = getFirestore(app);
} catch (err) {
  console.warn("Firebase init skipped:", err);
}
const appId = 'risda-portal-app';

// --- ID GOOGLE SHEETS KAKITANGAN & SANDARAN CSV RASMI ---
const STAFF_SHEET_ID = "1Ss756oJTZquBIVMnz0iWyW5JMhw-fOMi4J8jmnZOVeA";
const FALLBACK_PUBLISHED_CSV_URL = "https://docs.google.com/spreadsheets/d/e/2PACX-1vRBHXzXmWa6an5B7a89MsZp9BvZXUW5rt-cBIyQmgneyhRNIUbXA9hqu9Bc1tl5cLfNDSSckUGEo8wL/pub?gid=0&single=true&output=csv";

// --- FUNGSI PARSER CSV (Memecahkan data dari Google Sheets) ---
const parseCSV = (str) => {
  const arr = [];
  let quote = false;
  let row = 0, col = 0;
  for (let c = 0; c < str.length; c++) {
    let cc = str[c], nc = str[c + 1];
    arr[row] = arr[row] || [];
    arr[row][col] = arr[row][col] || '';
    if (cc === '"' && quote && nc === '"') { arr[row][col] += cc; ++c; continue; }
    if (cc === '"') { quote = !quote; continue; }
    if (cc === ',' && !quote) { ++col; continue; }
    if (cc === '\r' && nc === '\n' && !quote) { ++row; col = 0; ++c; continue; }
    if (cc === '\n' && !quote) { ++row; col = 0; continue; }
    if (cc === '\r' && !quote) { ++row; col = 0; continue; }
    arr[row][col] += cc;
  }
  return arr;
};

// --- FUNGSI PEMBACA GOOGLE SHEETS PINTAS CORS (JSONP) ---
const fetchSheetViaJSONP = (sheetId, gid = '0') => {
  return new Promise((resolve, reject) => {
    const callbackName = 'gvizCallback_' + Date.now() + '_' + Math.floor(Math.random() * 10000);
    const script = document.createElement('script');
    const timeoutId = setTimeout(() => {
      cleanup();
      reject(new Error('Timeout JSONP Google Sheets'));
    }, 8000);

    const cleanup = () => {
      clearTimeout(timeoutId);
      delete window[callbackName];
      if (script.parentNode) script.parentNode.removeChild(script);
    };

    window[callbackName] = (response) => {
      cleanup();
      try {
        if (!response || response.status === 'error' || !response.table) {
          reject(new Error('Respons Google Sheets tidak sah'));
          return;
        }
        const cols = response.table.cols.map(c => (c.label || c.id || '').trim());
        const rows = response.table.rows.map(r =>
          (r.c || []).map(cell => {
            if (!cell) return '';
            if (cell.f !== undefined && cell.f !== null) return String(cell.f);
            if (cell.v !== undefined && cell.v !== null) return String(cell.v);
            return '';
          })
        );

        const hasHeaderInCols = cols.some(c => c.toUpperCase().includes('NAMA') || c.toUpperCase().includes('DAERAH') || c.toUpperCase().includes('USERNAME'));
        if (!hasHeaderInCols && rows.length > 0 && rows[0].some(c => c.toUpperCase().includes('NAMA') || c.toUpperCase().includes('DAERAH') || c.toUpperCase().includes('USERNAME'))) {
          resolve([rows[0], ...rows.slice(1)]);
        } else {
          resolve([cols, ...rows]);
        }
      } catch (err) {
        reject(err);
      }
    };

    script.src = `https://docs.google.com/spreadsheets/d/${sheetId}/gviz/tq?gid=${gid}&tqx=out:json;responseHandler:${callbackName}`;
    script.onerror = () => {
      cleanup();
      reject(new Error('Gagal memuatkan skrip Google Sheets'));
    };
    document.head.appendChild(script);
  });
};

// Pembantu memuatkan data Google Sheets dengan sandaran automatik
const loadStaffSheetSmart = async () => {
  try {
    const jsonpData = await fetchSheetViaJSONP(STAFF_SHEET_ID, '0');
    if (jsonpData && jsonpData.length > 1) return jsonpData;
  } catch (e) {
    // Teruskan ke CSV fallback
  }

  const urlsToTry = [
    `https://docs.google.com/spreadsheets/d/${STAFF_SHEET_ID}/gviz/tq?tqx=out:csv&gid=0&t=${Date.now()}`,
    `${FALLBACK_PUBLISHED_CSV_URL}&t=${Date.now()}`
  ];

  for (const url of urlsToTry) {
    try {
      const response = await fetch(url);
      if (response.ok) {
        const text = await response.text();
        if (text && !text.trim().startsWith('<!DOCTYPE')) {
          const parsed = parseCSV(text);
          if (parsed && parsed.length > 1) return parsed;
        }
      }
    } catch (e) {
      // Cuba URL seterusnya
    }
  }
  return [];
};

// --- PEMBANTU PARSE SEJARAH PERKHIDMATAN, APC & SME DARI GOOGLE SHEETS ---
const parseServiceHistoryList = (rawHistory, currentPtj, tarikhPtSekarang, tarikhLantikan) => {
  const entries = [];
  if (rawHistory && rawHistory !== '-') {
    const parts = rawHistory.split(/[;\n|]+/).map(p => p.trim()).filter(Boolean);
    parts.forEach((part) => {
      const matchColon = part.match(/^([^:–-]+(?:\s*[-–]\s*[^:]+)?)\s*:\s*(.+)$/);
      if (matchColon) {
        entries.push({
          tempoh: matchColon[1].trim(),
          tempat: matchColon[2].trim(),
          isCurrent: false
        });
      } else {
        entries.push({
          tempoh: 'Rekod Penempatan',
          tempat: part,
          isCurrent: false
        });
      }
    });
  }

  if (currentPtj && currentPtj !== '-') {
    const alreadyListed = entries.some(e =>
      e.tempat.toUpperCase().includes(currentPtj.toUpperCase()) &&
      (e.tempoh.toUpperCase().includes('KINI') || e.tempoh.toUpperCase().includes('SEKARANG'))
    );
    if (!alreadyListed) {
      const startLabel = tarikhPtSekarang && tarikhPtSekarang !== '-'
        ? tarikhPtSekarang
        : (entries.length === 0 && tarikhLantikan && tarikhLantikan !== '-' ? tarikhLantikan : 'Semasa');
      entries.push({
        tempoh: `${startLabel} – Kini`,
        tempat: currentPtj,
        isCurrent: true
      });
    } else {
      entries[entries.length - 1].isCurrent = true;
    }
  }

  return entries;
};

const parseApcYearsList = (rawApc) => {
  if (!rawApc || rawApc === '-' || rawApc.toUpperCase() === 'TIADA' || rawApc.toUpperCase() === 'TIDAK') {
    return [];
  }
  const years = rawApc.match(/\b(19|20)\d{2}\b/g);
  if (years && years.length > 0) {
    return [...new Set(years)].sort((a, b) => Number(b) - Number(a));
  }
  return rawApc.split(/[,;/|]+/).map(s => s.trim()).filter(s => s && s !== '-');
};

const parseSmeInfo = (rawSme) => {
  if (!rawSme || rawSme === '-') return { isSme: false, bidang: '' };
  const clean = rawSme.trim();
  const upper = clean.toUpperCase();
  if (['TIDAK', 'TIADA', 'NO', 'NONE', 'N/A', '-'].includes(upper)) {
    return { isSme: false, bidang: '' };
  }
  if (['YA', 'YES', 'DILANTIK', 'AKTIF', 'SME'].includes(upper)) {
    return { isSme: true, bidang: 'Subject Matter Expert (SME) RISDA' };
  }
  return { isSme: true, bidang: clean };
};

// --- PEMBANTU MUAT IMEJ SELAMAT UNTUK CANVAS (ELAK RALAT CORS / TAINTED CANVAS DI LOCALHOST) ---
const loadCleanCanvasImage = async (urls) => {
  const expandedUrls = [];
  for (const rawUrl of urls) {
    if (!rawUrl) continue;
    expandedUrls.push(rawUrl);
    if (rawUrl.startsWith('http://') || rawUrl.startsWith('https://')) {
      const cleanNoProto = rawUrl.replace(/^https?:\/\//, '');
      expandedUrls.push(`https://images.weserv.nl/?url=${encodeURIComponent(cleanNoProto)}`);
    }
  }

  for (const url of expandedUrls) {
    const loaded = await new Promise((resolve) => {
      const img = new Image();
      if (url.startsWith('http://') || url.startsWith('https://')) {
        img.crossOrigin = 'anonymous';
        img.referrerPolicy = 'no-referrer';
      }
      const timer = setTimeout(() => resolve(null), 5000);
      img.onload = () => {
        clearTimeout(timer);
        try {
          if (!img.width || !img.height) {
            resolve(null);
            return;
          }
          const testCanvas = document.createElement('canvas');
          testCanvas.width = 2;
          testCanvas.height = 2;
          const tCtx = testCanvas.getContext('2d');
          tCtx.drawImage(img, 0, 0, 2, 2);
          testCanvas.toDataURL('image/png');
          resolve(img);
        } catch (err) {
          resolve(null);
        }
      };
      img.onerror = () => {
        clearTimeout(timer);
        resolve(null);
      };
      img.src = url;
    });
    if (loaded) return loaded;
  }
  return null;
};

// --- PEMBANTU PENAPIS LUTSINAR (BUANG LATAR BELAKANG PUTIH & HITAM PADA LOGO) ---
const createTransparentLogoCanvas = (img, brightenDarkText = false) => {
  if (!img) return null;
  try {
    const off = document.createElement('canvas');
    off.width = img.width;
    off.height = img.height;
    const oCtx = off.getContext('2d');
    oCtx.drawImage(img, 0, 0);
    const imgData = oCtx.getImageData(0, 0, off.width, off.height);
    const d = imgData.data;

    for (let i = 0; i < d.length; i += 4) {
      const r = d[i];
      const g = d[i + 1];
      const b = d[i + 2];
      const a = d[i + 3];
      if (a === 0) continue;

      // Buang latar belakang putih (logo lama) atau hitam pekat (logo HPC baru)
      if (r > 236 && g > 236 && b > 236) {
        d[i + 3] = 0;
      } else if (r > 212 && g > 212 && b > 212) {
        const avg = (r + g + b) / 3;
        const factor = Math.max(0, (242 - avg) / 30);
        d[i + 3] = Math.round(a * factor);
      } else if (r < 22 && g < 22 && b < 22) {
        d[i + 3] = 0;
      } else if (r < 42 && g < 42 && b < 42) {
        const maxC = Math.max(r, g, b);
        const factor = Math.max(0, (maxC - 22) / 20);
        d[i + 3] = Math.round(a * factor);
      } else if (brightenDarkText && r < 95 && g < 95 && b < 95 && Math.abs(r - g) < 18 && Math.abs(g - b) < 18) {
        d[i] = 248;
        d[i + 1] = 250;
        d[i + 2] = 252;
      }
    }

    oCtx.putImageData(imgData, 0, 0);
    return off;
  } catch (e) {
    return img;
  }
};

// --- LUKISAN VEKTOR IKON RASMI: 3 WARGA KERJA + PERISAI TANDA SEMAK ---
const drawStaffShieldIcon = (ctx, cx, cy, size, options = {}) => {
  const {
    shieldFill = '#1e3a8a',
    shieldStroke = '',
    checkColor = '#ffffff',
    peopleFill = '#1d70b8',
    cutoutColor = '#ffffff'
  } = options;

  ctx.save();
  ctx.translate(cx, cy);
  const s = size / 100;
  ctx.scale(s, s);

  ctx.beginPath();
  ctx.moveTo(0, -46);
  ctx.quadraticCurveTo(10, -34, 24, -31);
  ctx.quadraticCurveTo(27, -14, 20, 2);
  ctx.quadraticCurveTo(12, 13, 0, 19);
  ctx.quadraticCurveTo(-12, 13, -20, 2);
  ctx.quadraticCurveTo(-27, -14, -24, -31);
  ctx.quadraticCurveTo(-10, -34, 0, -46);
  ctx.closePath();
  ctx.fillStyle = shieldFill;
  ctx.fill();
  if (shieldStroke) {
    ctx.strokeStyle = shieldStroke;
    ctx.lineWidth = 2.2;
    ctx.stroke();
  }

  ctx.strokeStyle = checkColor;
  ctx.lineWidth = 5.2;
  ctx.lineCap = 'round';
  ctx.lineJoin = 'round';
  ctx.beginPath();
  ctx.moveTo(-8.5, -15);
  ctx.lineTo(-2, -8.5);
  ctx.lineTo(10.5, -22);
  ctx.stroke();

  const drawPerson = (px, py, rHead, wBody, hBody) => {
    ctx.fillStyle = cutoutColor;
    ctx.beginPath();
    ctx.arc(px, py, rHead + 3.2, 0, Math.PI * 2);
    ctx.fill();

    ctx.beginPath();
    ctx.moveTo(px - wBody - 3.2, py + rHead + hBody + 2);
    ctx.quadraticCurveTo(px - wBody - 2, py + rHead + 1.5, px, py + rHead + 1.5);
    ctx.quadraticCurveTo(px + wBody + 2, py + rHead + 1.5, px + wBody + 3.2, py + rHead + hBody + 2);
    ctx.closePath();
    ctx.fill();

    ctx.fillStyle = peopleFill;
    ctx.beginPath();
    ctx.arc(px, py, rHead, 0, Math.PI * 2);
    ctx.fill();

    ctx.beginPath();
    ctx.moveTo(px - wBody, py + rHead + hBody);
    ctx.quadraticCurveTo(px - wBody + 1, py + rHead + 4.5, px, py + rHead + 4.5);
    ctx.quadraticCurveTo(px + wBody - 1, py + rHead + 4.5, px + wBody, py + rHead + hBody);
    ctx.closePath();
    ctx.fill();
  };

  drawPerson(-24, -4, 10.5, 19, 22);
  drawPerson(24, -4, 10.5, 19, 22);
  drawPerson(0, 3, 11.2, 21.5, 24);

  ctx.restore();
};

// --- FUNGSI PENJANA INFOGRAFIK KORPORAT BILANGAN STAF RISDA PAHANG (1920x1080 HD) ---
const generateInfographicDataUrl = async (dataset, customBuildingDataUrl = '') => {
  const loadWithTimeout = async (urls, ms = 2200) => {
    try {
      return await Promise.race([
        loadCleanCanvasImage(urls),
        new Promise((resolve) => setTimeout(() => resolve(null), ms))
      ]);
    } catch (e) {
      return null;
    }
  };

  const [rawRisdaCrest, rawHpcLogo, buildingImg] = await Promise.all([
    loadWithTimeout([
      LOGO_CREST_URL,
      `https://lh3.googleusercontent.com/d/${LOGO_CREST_DRIVE_ID}`,
      `https://drive.google.com/thumbnail?id=${LOGO_CREST_DRIVE_ID}&sz=w1000`
    ], 2200),
    loadWithTimeout([
      LOGO_HPC_URL,
      `https://lh3.googleusercontent.com/d/${LOGO_HPC_DRIVE_ID}`,
      `https://drive.google.com/thumbnail?id=${LOGO_HPC_DRIVE_ID}&sz=w1000`
    ], 2200),
    loadWithTimeout([
      customBuildingDataUrl,
      BANGUNAN_PRN_PRIMARY_URL,
      BANGUNAN_PRN_URL,
      `https://lh3.googleusercontent.com/d/${BANGUNAN_PRN_DRIVE_ID}`,
      `https://drive.google.com/thumbnail?id=${BANGUNAN_PRN_DRIVE_ID}&sz=w1200`
    ], 2200)
  ]);

  const risdaCrestTransparent = createTransparentLogoCanvas(rawRisdaCrest, false);
  const hpcLogoTransparent = createTransparentLogoCanvas(rawHpcLogo, true);

  const canvas = document.createElement('canvas');
  const W = 1920;
  const H = 1080;
  canvas.width = W;
  canvas.height = H;
  const ctx = canvas.getContext('2d');
  if (!ctx) return '';

  const drawRoundRect = (x, y, w, h, r) => {
    const radius = typeof r === 'number' ? { tl: r, tr: r, br: r, bl: r } : r;
    ctx.beginPath();
    ctx.moveTo(x + radius.tl, y);
    ctx.lineTo(x + w - radius.tr, y);
    ctx.quadraticCurveTo(x + w, y, x + w, y + radius.tr);
    ctx.lineTo(x + w, y + h - radius.br);
    ctx.quadraticCurveTo(x + w, y + h, x + w - radius.br, y + h);
    ctx.lineTo(x + radius.bl, y + h);
    ctx.quadraticCurveTo(x, y + h, x, y + h - radius.bl);
    ctx.lineTo(x, y + radius.tl);
    ctx.quadraticCurveTo(x, y, x + radius.tl, y);
    ctx.closePath();
  };

  const drawImageCover = (img, x, y, w, h, alignY = 0.5) => {
    const imgRatio = img.width / img.height;
    const targetRatio = w / h;
    let drawW = w, drawH = h, offsetX = 0, offsetY = 0;
    if (imgRatio > targetRatio) {
      drawW = h * imgRatio;
      offsetX = (w - drawW) / 2;
    } else {
      drawH = w / imgRatio;
      offsetY = (h - drawH) * alignY;
    }
    ctx.drawImage(img, x + offsetX, y + offsetY, drawW, drawH);
  };

  const drawImageContain = (img, x, y, w, h) => {
    const scale = Math.min(w / img.width, h / img.height);
    const dw = img.width * scale;
    const dh = img.height * scale;
    ctx.drawImage(img, x + (w - dw) / 2, y + (h - dh) / 2, dw, dh);
  };

  const now = new Date();
  const bulanTahun = now.toLocaleDateString('ms-MY', { month: 'long', year: 'numeric' }).toUpperCase();
  const bulanTahunTitle = now.toLocaleDateString('ms-MY', { month: 'long', year: 'numeric' });
  const totalStaf = dataset.length;

  const formatPtjPoster = (raw) => {
    const clean = (raw || 'Lain-lain').trim();
    const upper = clean.toUpperCase();
    if (upper.includes('PRN')) return 'Pejabat PRN - Pahang';
    const stripped = clean.replace(/^PRD\s*-\s*/i, '').trim();
    return `Pejabat PRD - ${stripped}`;
  };

  const ptjMap = {};
  dataset.forEach(s => {
    const label = formatPtjPoster(s.ptj);
    ptjMap[label] = (ptjMap[label] || 0) + 1;
  });

  const sortedPtjList = Object.entries(ptjMap)
    .map(([name, count]) => ({ name, count }))
    .sort((a, b) => {
      const aIsPrn = a.name.toUpperCase().includes('PRN');
      const bIsPrn = b.name.toUpperCase().includes('PRN');
      if (aIsPrn && !bIsPrn) return -1;
      if (!aIsPrn && bIsPrn) return 1;
      if (b.count !== a.count) return b.count - a.count;
      return a.name.localeCompare(b.name);
    });

  const gredCountMap = {};
  dataset.forEach(s => {
    const g = (s.skimGred && s.skimGred !== 'LAIN') ? s.skimGred : 'LAIN';
    gredCountMap[g] = (gredCountMap[g] || 0) + 1;
  });
  const sortedGredBars = Object.entries(gredCountMap)
    .map(([gred, count]) => ({ gred, count }))
    .sort((a, b) => b.count - a.count || a.gred.localeCompare(b.gred));

  // Susunan gred tepat mengikut hierarki pangkat & skim: G13, G12, N10, G10, G9, G7, G6, N6, W6, G5, N5, W5, FA5, JA5... hingga H1
  const exactGredOrder = [
    'G13', 'G12',
    'N10', 'G10',
    'G9',
    'G7',
    'G6', 'N6', 'W6',
    'G5', 'N5', 'W5', 'FA5', 'JA5',
    'N3', 'W3',
    'N2', 'W2', 'J2',
    'N1', 'W1',
    'H1'
  ];

  const matrixGreds = Object.keys(gredCountMap).sort((a, b) => {
    const cleanA = String(a || '').trim().toUpperCase();
    const cleanB = String(b || '').trim().toUpperCase();
    const idxA = exactGredOrder.indexOf(cleanA);
    const idxB = exactGredOrder.indexOf(cleanB);

    if (idxA !== -1 && idxB !== -1) return idxA - idxB;
    if (idxA !== -1) return cleanB === 'H1' ? -1 : idxA - 20;
    if (idxB !== -1) return cleanA === 'H1' ? 1 : 20 - idxB;
    return cleanA.localeCompare(cleanB, undefined, { numeric: true });
  });

  const bgGrad = ctx.createLinearGradient(0, 0, W, H);
  bgGrad.addColorStop(0, '#eaf1fa');
  bgGrad.addColorStop(0.5, '#f8fafc');
  bgGrad.addColorStop(1, '#e6eef8');
  ctx.fillStyle = bgGrad;
  ctx.fillRect(0, 0, W, H);

  ctx.save();
  const topWave = ctx.createLinearGradient(0, 0, 1280, 230);
  topWave.addColorStop(0, '#0f2354');
  topWave.addColorStop(0.65, '#1e3a8a');
  topWave.addColorStop(1, '#1d4ed8');
  ctx.fillStyle = topWave;
  ctx.beginPath();
  ctx.moveTo(0, 0);
  ctx.lineTo(1380, 0);
  ctx.lineTo(1310, 215);
  ctx.bezierCurveTo(920, 182, 480, 198, 0, 224);
  ctx.closePath();
  ctx.fill();

  ctx.clip();
  ctx.strokeStyle = 'rgba(255, 255, 255, 0.06)';
  ctx.lineWidth = 1.2;
  const hexSize = 36;
  for (let gx = 0; gx < 1380; gx += hexSize * 1.5) {
    for (let gy = 0; gy < 240; gy += hexSize * 0.86) {
      ctx.beginPath();
      ctx.moveTo(gx, gy);
      ctx.lineTo(gx + hexSize * 0.5, gy - hexSize * 0.43);
      ctx.lineTo(gx + hexSize, gy);
      ctx.lineTo(gx + hexSize * 0.5, gy + hexSize * 0.43);
      ctx.closePath();
      ctx.stroke();
    }
  }
  ctx.restore();

  const bldX = 1280, bldY = 0, bldW = 640, bldH = 222;
  ctx.save();
  ctx.beginPath();
  ctx.moveTo(bldX + 68, 0);
  ctx.lineTo(W, 0);
  ctx.lineTo(W, bldH);
  ctx.lineTo(bldX, bldH);
  ctx.closePath();
  ctx.clip();

  if (buildingImg) {
    drawImageCover(buildingImg, bldX, bldY, bldW, bldH, 0.36);
  } else {
    const skyFallback = ctx.createLinearGradient(bldX, 0, W, bldH);
    skyFallback.addColorStop(0, '#38bdf8');
    skyFallback.addColorStop(1, '#bae6fd');
    ctx.fillStyle = skyFallback;
    ctx.fillRect(bldX, 0, bldW, bldH);
    ctx.fillStyle = '#f59e0b';
    drawRoundRect(bldX + 150, 68, 360, 130, 8);
    ctx.fill();
    ctx.fillStyle = '#0f2354';
    ctx.font = '900 14px Arial, sans-serif';
    ctx.fillText('PEJABAT RISDA NEGERI PAHANG', bldX + 215, 110);
  }

  const leftBlend = ctx.createLinearGradient(bldX, 0, bldX + 125, 0);
  leftBlend.addColorStop(0, 'rgba(29, 78, 216, 1)');
  leftBlend.addColorStop(0.45, 'rgba(29, 78, 216, 0.55)');
  leftBlend.addColorStop(1, 'rgba(29, 78, 216, 0)');
  ctx.fillStyle = leftBlend;
  ctx.fillRect(bldX, 0, 125, bldH);
  ctx.restore();

  const goldSweep = ctx.createLinearGradient(0, 218, W, 208);
  goldSweep.addColorStop(0, '#ca8a04');
  goldSweep.addColorStop(0.28, '#fef08a');
  goldSweep.addColorStop(0.55, '#eab308');
  goldSweep.addColorStop(0.82, '#fef08a');
  goldSweep.addColorStop(1, '#ca8a04');
  ctx.strokeStyle = goldSweep;
  ctx.lineWidth = 7;
  ctx.beginPath();
  ctx.moveTo(0, 224);
  ctx.bezierCurveTo(480, 198, 920, 182, 1310, 215);
  ctx.lineTo(W, 222);
  ctx.stroke();

  const botLeftGrad = ctx.createLinearGradient(0, 560, 140, 1080);
  botLeftGrad.addColorStop(0, '#1e3a8a');
  botLeftGrad.addColorStop(1, '#0f2354');
  ctx.fillStyle = botLeftGrad;
  ctx.beginPath();
  ctx.moveTo(0, 565);
  ctx.quadraticCurveTo(118, 630, 86, 1080);
  ctx.lineTo(0, 1080);
  ctx.closePath();
  ctx.fill();

  const botRightGrad = ctx.createLinearGradient(W - 140, 560, W, 1080);
  botRightGrad.addColorStop(0, '#1e3a8a');
  botRightGrad.addColorStop(1, '#0f2354');
  ctx.fillStyle = botRightGrad;
  ctx.beginPath();
  ctx.moveTo(W, 565);
  ctx.quadraticCurveTo(W - 118, 630, W - 86, 1080);
  ctx.lineTo(W, 1080);
  ctx.closePath();
  ctx.fill();

  const logoAreaX = 46;
  const logoAreaY = 26;

  if (risdaCrestTransparent) {
    ctx.save();
    ctx.shadowColor = 'rgba(0, 0, 0, 0.32)';
    ctx.shadowBlur = 10;
    ctx.shadowOffsetY = 3;
    drawImageContain(risdaCrestTransparent, logoAreaX, logoAreaY, 142, 142);
    ctx.restore();
  } else {
    ctx.save();
    ctx.translate(logoAreaX + 71, logoAreaY + 71);
    ctx.strokeStyle = '#facc15';
    ctx.lineWidth = 3;
    ctx.beginPath();
    ctx.arc(0, 0, 58, 0, Math.PI * 2);
    ctx.stroke();
    ctx.fillStyle = '#eab308';
    ctx.beginPath();
    ctx.moveTo(-42, -14);
    ctx.quadraticCurveTo(0, 8, 42, -14);
    ctx.quadraticCurveTo(32, 34, 0, 34);
    ctx.quadraticCurveTo(-32, 34, -42, -14);
    ctx.fill();
    ctx.fillStyle = '#ffffff';
    ctx.font = '900 18px Arial, sans-serif';
    ctx.textAlign = 'center';
    ctx.fillText('RISDA', 0, 48);
    ctx.restore();
  }

  ctx.strokeStyle = 'rgba(250, 204, 21, 0.45)';
  ctx.lineWidth = 2;
  ctx.beginPath();
  ctx.moveTo(logoAreaX + 154, logoAreaY + 22);
  ctx.lineTo(logoAreaX + 154, logoAreaY + 122);
  ctx.stroke();

  if (hpcLogoTransparent) {
    ctx.save();
    ctx.shadowColor = 'rgba(0, 0, 0, 0.28)';
    ctx.shadowBlur = 8;
    ctx.shadowOffsetY = 2;
    drawImageContain(hpcLogoTransparent, logoAreaX + 166, logoAreaY + 8, 174, 126);
    ctx.restore();
  } else {
    ctx.save();
    ctx.fillStyle = '#facc15';
    ctx.font = '900 32px Arial Black, sans-serif';
    ctx.textAlign = 'center';
    ctx.fillText('RISDA', logoAreaX + 253, logoAreaY + 66);
    ctx.fillStyle = '#ffffff';
    ctx.font = '900 10.5px Arial, sans-serif';
    ctx.fillText('BUDAYA BERPRESTASI TINGGI', logoAreaX + 253, logoAreaY + 86);
    ctx.fillStyle = '#cbd5e1';
    ctx.font = 'bold 8px Arial, sans-serif';
    ctx.fillText('HIGH PERFORMANCE CULTURE', logoAreaX + 253, logoAreaY + 100);
    ctx.restore();
  }

  ctx.strokeStyle = 'rgba(147, 197, 253, 0.35)';
  ctx.lineWidth = 2;
  ctx.beginPath();
  ctx.moveTo(logoAreaX + 354, logoAreaY + 18);
  ctx.lineTo(logoAreaX + 354, logoAreaY + 132);
  ctx.stroke();

  const titleX = logoAreaX + 376;
  ctx.save();
  ctx.textAlign = 'left';
  ctx.font = '900 48px Arial, sans-serif';
  ctx.fillStyle = 'rgba(9, 18, 44, 0.55)';
  ctx.fillText('BILANGAN STAF', titleX + 2, 74);
  ctx.fillText('RISDA NEGERI PAHANG', titleX + 2, 125);

  ctx.fillStyle = '#ffffff';
  ctx.fillText('BILANGAN STAF', titleX, 72);
  ctx.fillStyle = '#fef08a';
  ctx.fillText('RISDA NEGERI PAHANG', titleX, 123);
  ctx.restore();

  const ribbonText = `SETAKAT ${bulanTahun}`;
  ctx.font = '900 20px Arial, sans-serif';
  const ribbonW = Math.max(300, ctx.measureText(ribbonText).width + 64);
  const ribGrad = ctx.createLinearGradient(titleX, 138, titleX + ribbonW, 176);
  ribGrad.addColorStop(0, '#eab308');
  ribGrad.addColorStop(0.5, '#facc15');
  ribGrad.addColorStop(1, '#ca8a04');
  ctx.fillStyle = ribGrad;
  drawRoundRect(titleX, 138, ribbonW, 38, 19);
  ctx.fill();
  ctx.strokeStyle = '#ffffff';
  ctx.lineWidth = 2;
  ctx.stroke();

  ctx.fillStyle = '#0f2354';
  ctx.textAlign = 'center';
  ctx.fillText(ribbonText, titleX + ribbonW / 2, 164);

  const leftCardX = 42, leftCardY = 236, leftCardW = 580, leftCardH = 346;
  ctx.save();
  ctx.shadowColor = 'rgba(15, 35, 84, 0.14)';
  ctx.shadowBlur = 18;
  ctx.shadowOffsetY = 6;
  ctx.fillStyle = '#ffffff';
  drawRoundRect(leftCardX, leftCardY, leftCardW, leftCardH, 18);
  ctx.fill();
  ctx.restore();

  ctx.strokeStyle = '#bfdbfe';
  ctx.lineWidth = 2;
  drawRoundRect(leftCardX, leftCardY, leftCardW, leftCardH, 18);
  ctx.stroke();

  ctx.fillStyle = '#ffffff';
  ctx.beginPath();
  ctx.arc(leftCardX + 46, leftCardY + 14, 29, 0, Math.PI * 2);
  ctx.fill();
  ctx.strokeStyle = '#eab308';
  ctx.lineWidth = 3.5;
  ctx.stroke();
  drawStaffShieldIcon(ctx, leftCardX + 46, leftCardY + 15, 38, {
    shieldFill: '#1e3a8a',
    checkColor: '#ffffff',
    peopleFill: '#1d70b8',
    cutoutColor: '#ffffff'
  });

  ctx.textAlign = 'left';
  ctx.fillStyle = '#0f2354';
  ctx.font = '900 18px Arial, sans-serif';
  ctx.fillText('BILANGAN STAF MENGIKUT', leftCardX + 86, leftCardY + 26);
  ctx.fillText('PUSAT TANGGUNGJAWAB (PTJ)', leftCardX + 86, leftCardY + 48);

  const ptjBarColors = ['#1e3a8a', '#1d4ed8', '#0284c7', '#eab308', '#0d9488', '#2563eb', '#0ea5e9', '#3b82f6', '#d97706'];
  const maxPtjCount = Math.max(...sortedPtjList.map(p => p.count), 1);
  const displayPtjs = sortedPtjList.slice(0, 9);
  const rowStepPtj = displayPtjs.length > 0 ? Math.min(30, 268 / displayPtjs.length) : 30;

  displayPtjs.forEach((item, idx) => {
    const yPos = leftCardY + 74 + idx * rowStepPtj;
    ctx.fillStyle = idx % 2 === 0 ? '#f1f5f9' : '#f8fafc';
    drawRoundRect(leftCardX + 16, yPos - 15, leftCardW - 32, rowStepPtj - 4, 6);
    ctx.fill();

    ctx.fillStyle = '#0f172a';
    ctx.font = 'bold 13.5px Arial, sans-serif';
    ctx.textAlign = 'left';
    ctx.fillText(item.name, leftCardX + 24, yPos + 3);

    const barStartX = leftCardX + 212;
    const maxBarW = 282;
    const barW = Math.max(24, (item.count / maxPtjCount) * maxBarW);
    ctx.fillStyle = ptjBarColors[idx % ptjBarColors.length];
    drawRoundRect(barStartX, yPos - 11, barW, 18, { tl: 4, tr: 9, br: 9, bl: 4 });
    ctx.fill();

    const badgeX = leftCardX + leftCardW - 64;
    ctx.fillStyle = '#ffffff';
    ctx.strokeStyle = '#cbd5e1';
    ctx.lineWidth = 1.5;
    drawRoundRect(badgeX, yPos - 13, 42, 22, 11);
    ctx.fill();
    ctx.stroke();

    ctx.fillStyle = '#0f2354';
    ctx.font = '900 13.5px Arial, sans-serif';
    ctx.textAlign = 'center';
    ctx.fillText(String(item.count), badgeX + 21, yPos + 3);
  });

  const centerX = 880;
  ctx.save();
  ctx.shadowColor = 'rgba(15, 35, 84, 0.28)';
  ctx.shadowBlur = 24;
  ctx.shadowOffsetY = 8;

  const shieldGrad = ctx.createLinearGradient(centerX - 168, 165, centerX + 168, 378);
  shieldGrad.addColorStop(0, '#0f2354');
  shieldGrad.addColorStop(0.5, '#1e3a8a');
  shieldGrad.addColorStop(1, '#091534');

  ctx.beginPath();
  ctx.moveTo(centerX - 168, 184);
  ctx.quadraticCurveTo(centerX, 152, centerX + 168, 184);
  ctx.lineTo(centerX + 150, 294);
  ctx.quadraticCurveTo(centerX + 115, 352, centerX, 378);
  ctx.quadraticCurveTo(centerX - 115, 352, centerX - 150, 294);
  ctx.closePath();
  ctx.fillStyle = shieldGrad;
  ctx.fill();

  const shieldGoldBorder = ctx.createLinearGradient(centerX - 168, 165, centerX + 168, 378);
  shieldGoldBorder.addColorStop(0, '#fef08a');
  shieldGoldBorder.addColorStop(0.5, '#eab308');
  shieldGoldBorder.addColorStop(1, '#a16207');
  ctx.lineWidth = 7.5;
  ctx.strokeStyle = shieldGoldBorder;
  ctx.stroke();
  ctx.restore();

  ctx.fillStyle = '#ffffff';
  drawRoundRect(centerX - 134, 188, 268, 32, 16);
  ctx.fill();
  ctx.fillStyle = '#0f2354';
  ctx.font = '900 17px Arial, sans-serif';
  ctx.textAlign = 'center';
  ctx.fillText('JUMLAH KESELURUHAN', centerX, 210);

  ctx.save();
  ctx.font = '900 92px Arial, sans-serif';
  ctx.textAlign = 'center';
  ctx.fillStyle = 'rgba(0, 0, 0, 0.38)';
  ctx.fillText(String(totalStaf), centerX + 3, 299);

  const numGoldGrad = ctx.createLinearGradient(0, 224, 0, 306);
  numGoldGrad.addColorStop(0, '#fef9c3');
  numGoldGrad.addColorStop(0.45, '#facc15');
  numGoldGrad.addColorStop(1, '#ca8a04');
  ctx.fillStyle = numGoldGrad;
  ctx.fillText(String(totalStaf), centerX, 296);
  ctx.restore();

  ctx.fillStyle = '#ffffff';
  ctx.font = '900 22px Arial, sans-serif';
  ctx.textAlign = 'center';
  ctx.fillText('KAKITANGAN', centerX, 329);

  ctx.save();
  ctx.shadowColor = 'rgba(15, 35, 84, 0.14)';
  ctx.shadowBlur = 14;
  ctx.shadowOffsetY = 4;
  ctx.fillStyle = '#ffffff';
  ctx.beginPath();
  ctx.arc(centerX, 452, 66, 0, Math.PI * 2);
  ctx.fill();
  ctx.restore();

  ctx.strokeStyle = '#eab308';
  ctx.lineWidth = 3.5;
  ctx.beginPath();
  ctx.arc(centerX, 452, 66, 0, Math.PI * 2);
  ctx.stroke();

  drawStaffShieldIcon(ctx, centerX, 456, 98, {
    shieldFill: '#2c3e50',
    checkColor: '#ffffff',
    peopleFill: '#1d70b8',
    cutoutColor: '#ffffff'
  });

  ctx.fillStyle = '#ffffff';
  ctx.strokeStyle = '#bfdbfe';
  ctx.lineWidth = 2;
  drawRoundRect(centerX - 226, 524, 452, 56, 14);
  ctx.fill();
  ctx.stroke();

  drawStaffShieldIcon(ctx, centerX - 192, 553, 34, {
    shieldFill: '#2c3e50',
    checkColor: '#ffffff',
    peopleFill: '#1d70b8',
    cutoutColor: '#ffffff'
  });

  ctx.fillStyle = '#0f2354';
  ctx.font = 'bold 13.5px Arial, sans-serif';
  ctx.textAlign = 'center';
  ctx.fillText('Jumlah ini mewakili keseluruhan tenaga kerja', centerX + 14, 548);
  ctx.fillText(`RISDA di negeri Pahang setakat ${bulanTahunTitle}.`, centerX + 14, 568);

  const rightCardX = 1140, rightCardY = 236, rightCardW = 738, rightCardH = 346;
  ctx.save();
  ctx.shadowColor = 'rgba(15, 35, 84, 0.14)';
  ctx.shadowBlur = 18;
  ctx.shadowOffsetY = 6;
  ctx.fillStyle = '#ffffff';
  drawRoundRect(rightCardX, rightCardY, rightCardW, rightCardH, 18);
  ctx.fill();
  ctx.restore();

  ctx.strokeStyle = '#bfdbfe';
  ctx.lineWidth = 2;
  drawRoundRect(rightCardX, rightCardY, rightCardW, rightCardH, 18);
  ctx.stroke();

  ctx.fillStyle = '#0f2354';
  ctx.beginPath();
  ctx.arc(rightCardX + 46, rightCardY + 14, 28, 0, Math.PI * 2);
  ctx.fill();
  ctx.strokeStyle = '#eab308';
  ctx.lineWidth = 3.5;
  ctx.stroke();
  ctx.fillStyle = '#facc15';
  ctx.fillRect(rightCardX + 35, rightCardY + 14, 5, 10);
  ctx.fillStyle = '#ffffff';
  ctx.fillRect(rightCardX + 43, rightCardY + 9, 5, 15);
  ctx.fillStyle = '#38bdf8';
  ctx.fillRect(rightCardX + 51, rightCardY + 4, 5, 20);

  ctx.textAlign = 'left';
  ctx.fillStyle = '#0f2354';
  ctx.font = '900 18px Arial, sans-serif';
  ctx.fillText('BILANGAN KAKITANGAN', rightCardX + 86, rightCardY + 26);
  ctx.fillText('MENGIKUT GRED', rightCardX + 86, rightCardY + 48);

  const plotX = rightCardX + 58;
  const plotY = rightCardY + 84;
  const plotW = rightCardW - 82;
  const plotH = 188;

  const rawMaxGred = Math.max(...sortedGredBars.map(g => g.count), 10);
  const yMax = Math.ceil(rawMaxGred / 20) * 20;
  const yStep = yMax <= 60 ? 10 : 20;

  ctx.font = 'bold 11.5px Arial, sans-serif';
  ctx.textAlign = 'right';
  for (let val = 0; val <= yMax; val += yStep) {
    const gy = plotY + plotH - (val / yMax) * plotH;
    ctx.strokeStyle = val === 0 ? '#64748b' : '#e2e8f0';
    ctx.lineWidth = val === 0 ? 2 : 1;
    ctx.beginPath();
    ctx.moveTo(plotX, gy);
    ctx.lineTo(plotX + plotW, gy);
    ctx.stroke();

    ctx.fillStyle = '#475569';
    ctx.fillText(String(val), plotX - 8, gy + 4);
  }

  const gredPalette = ['#1e3a8a', '#eab308', '#0284c7', '#d97706', '#2563eb', '#0d9488', '#f59e0b', '#3b82f6'];
  const barCount = sortedGredBars.length;
  const slotW = barCount > 0 ? plotW / barCount : plotW;
  const barWidth = Math.max(12, Math.min(28, slotW * 0.68));

  sortedGredBars.forEach((item, i) => {
    const bx = plotX + i * slotW + (slotW - barWidth) / 2;
    const bh = Math.max(4, (item.count / yMax) * plotH);
    const by = plotY + plotH - bh;

    ctx.fillStyle = gredPalette[i % gredPalette.length];
    drawRoundRect(bx, by, barWidth, bh, { tl: 4, tr: 4, br: 0, bl: 0 });
    ctx.fill();

    ctx.fillStyle = '#0f2354';
    ctx.font = barCount > 16 ? '900 12px Arial, sans-serif' : '900 14px Arial, sans-serif';
    ctx.textAlign = 'center';
    ctx.fillText(String(item.count), bx + barWidth / 2, by - 6);

    ctx.fillStyle = '#334155';
    ctx.font = barCount > 16 ? 'bold 10.5px Arial, sans-serif' : 'bold 12px Arial, sans-serif';
    ctx.fillText(item.gred, bx + barWidth / 2, plotY + plotH + 17);
  });

  ctx.fillStyle = '#0f2354';
  drawRoundRect(plotX + plotW / 2 - 58, rightCardY + rightCardH - 36, 116, 26, 13);
  ctx.fill();
  ctx.strokeStyle = '#eab308';
  ctx.lineWidth = 2;
  ctx.stroke();
  ctx.fillStyle = '#fef08a';
  ctx.font = '900 13px Arial, sans-serif';
  ctx.textAlign = 'center';
  ctx.fillText('GRED', plotX + plotW / 2, rightCardY + rightCardH - 18);

  const tblBannerW = 760;
  const tblBannerX = (W - tblBannerW) / 2;
  const tblBannerY = 594;
  ctx.fillStyle = '#0f2354';
  drawRoundRect(tblBannerX, tblBannerY, tblBannerW, 34, 17);
  ctx.fill();
  ctx.strokeStyle = '#eab308';
  ctx.lineWidth = 2.5;
  ctx.stroke();
  ctx.fillStyle = '#ffffff';
  ctx.font = '900 18px Arial, sans-serif';
  ctx.textAlign = 'center';
  ctx.fillText('PERINCIAN BILANGAN STAF MENGIKUT PTJ DAN GRED', W / 2, tblBannerY + 23);

  const tblX = 42;
  const tblY = 636;
  const tblW = W - 84;
  const ptjColW = 265;
  const totalColW = 96;
  const gredColsTotalW = tblW - ptjColW - totalColW;
  const numGredCols = Math.max(matrixGreds.length, 1);
  const singleGredW = gredColsTotalW / numGredCols;

  const headerH = 54;
  const footerH = 38;
  const bodyRowsCount = Math.max(sortedPtjList.length, 1);
  const availableBodyH = H - tblY - headerH - footerH - 22;
  const rowH = Math.min(34, Math.max(24, availableBodyH / bodyRowsCount));
  const totalTblH = headerH + bodyRowsCount * rowH + footerH;

  ctx.save();
  ctx.shadowColor = 'rgba(15, 35, 84, 0.14)';
  ctx.shadowBlur = 14;
  ctx.shadowOffsetY = 4;
  ctx.fillStyle = '#ffffff';
  drawRoundRect(tblX, tblY, tblW, totalTblH, 14);
  ctx.fill();
  ctx.restore();

  ctx.save();
  drawRoundRect(tblX, tblY, tblW, totalTblH, 14);
  ctx.clip();

  ctx.fillStyle = '#0f2354';
  ctx.fillRect(tblX, tblY, ptjColW, headerH);
  ctx.fillStyle = '#facc15';
  ctx.beginPath();
  ctx.arc(tblX + 86, tblY + 24, 7, 0, Math.PI * 2);
  ctx.fill();
  ctx.beginPath();
  ctx.moveTo(tblX + 79, tblY + 26);
  ctx.lineTo(tblX + 93, tblY + 26);
  ctx.lineTo(tblX + 86, tblY + 38);
  ctx.closePath();
  ctx.fill();
  ctx.fillStyle = '#0f2354';
  ctx.beginPath();
  ctx.arc(tblX + 86, tblY + 24, 2.8, 0, Math.PI * 2);
  ctx.fill();

  ctx.fillStyle = '#ffffff';
  ctx.font = '900 18px Arial, sans-serif';
  ctx.textAlign = 'center';
  ctx.fillText('PTJ', tblX + ptjColW / 2 + 12, tblY + 34);

  ctx.fillStyle = '#1d4ed8';
  ctx.fillRect(tblX + ptjColW, tblY, gredColsTotalW, 24);
  ctx.fillStyle = '#fef08a';
  ctx.font = '900 13px Arial, sans-serif';
  ctx.fillText('GRED', tblX + ptjColW + gredColsTotalW / 2, tblY + 17);

  matrixGreds.forEach((g, idx) => {
    const gx = tblX + ptjColW + idx * singleGredW;
    ctx.fillStyle = idx % 2 === 0 ? '#1e3a8a' : '#172554';
    ctx.fillRect(gx, tblY + 24, singleGredW, headerH - 24);
    ctx.strokeStyle = 'rgba(255,255,255,0.18)';
    ctx.lineWidth = 1;
    ctx.strokeRect(gx, tblY + 24, singleGredW, headerH - 24);

    ctx.fillStyle = '#ffffff';
    ctx.font = numGredCols > 18 ? '900 12px Arial, sans-serif' : '900 13.5px Arial, sans-serif';
    ctx.textAlign = 'center';
    ctx.fillText(g, gx + singleGredW / 2, tblY + 44);
  });

  const totalHeadGrad = ctx.createLinearGradient(tblX + tblW - totalColW, tblY, tblX + tblW, tblY + headerH);
  totalHeadGrad.addColorStop(0, '#facc15');
  totalHeadGrad.addColorStop(1, '#eab308');
  ctx.fillStyle = totalHeadGrad;
  ctx.fillRect(tblX + tblW - totalColW, tblY, totalColW, headerH);
  ctx.fillStyle = '#0f2354';
  ctx.font = '900 17px Arial, sans-serif';
  ctx.textAlign = 'center';
  ctx.fillText('TOTAL', tblX + tblW - totalColW / 2, tblY + 34);

  const matrixCounts = {};
  const colTotals = {};
  matrixGreds.forEach(g => { colTotals[g] = 0; });

  dataset.forEach(s => {
    const pLabel = formatPtjPoster(s.ptj);
    const gLabel = (s.skimGred && s.skimGred !== 'LAIN') ? s.skimGred : 'LAIN';
    if (!matrixCounts[pLabel]) matrixCounts[pLabel] = {};
    matrixCounts[pLabel][gLabel] = (matrixCounts[pLabel][gLabel] || 0) + 1;
    colTotals[gLabel] = (colTotals[gLabel] || 0) + 1;
  });

  const highlightColColors = {
    G5: 'rgba(191, 219, 254, 0.45)',
    H1: 'rgba(224, 242, 254, 0.50)',
    N2: 'rgba(254, 240, 138, 0.42)',
    W2: 'rgba(254, 249, 195, 0.55)'
  };

  sortedPtjList.forEach((ptjItem, rIdx) => {
    const ry = tblY + headerH + rIdx * rowH;
    ctx.fillStyle = rIdx % 2 === 0 ? '#ffffff' : '#f1f5f9';
    ctx.fillRect(tblX, ry, tblW, rowH);

    const ptjDisplayUpper = ptjItem.name.replace(' - ', ' ').toUpperCase();
    ctx.fillStyle = '#0f2354';
    ctx.font = '900 13.5px Arial, sans-serif';
    ctx.textAlign = 'left';
    ctx.fillText(ptjDisplayUpper, tblX + 18, ry + rowH / 2 + 5);

    matrixGreds.forEach((g, cIdx) => {
      const gx = tblX + ptjColW + cIdx * singleGredW;
      if (highlightColColors[g]) {
        ctx.fillStyle = highlightColColors[g];
        ctx.fillRect(gx, ry, singleGredW, rowH);
      }
      ctx.strokeStyle = '#cbd5e1';
      ctx.lineWidth = 0.8;
      ctx.strokeRect(gx, ry, singleGredW, rowH);

      const val = (matrixCounts[ptjItem.name] && matrixCounts[ptjItem.name][g]) || 0;
      ctx.fillStyle = val > 0 ? '#0f172a' : '#64748b';
      ctx.font = val > 0 ? '900 14.5px Arial, sans-serif' : '600 13.5px Arial, sans-serif';
      ctx.textAlign = 'center';
      ctx.fillText(String(val), gx + singleGredW / 2, ry + rowH / 2 + 5);
    });

    const tx = tblX + tblW - totalColW;
    ctx.fillStyle = rIdx % 2 === 0 ? '#fef9c3' : '#fef08a';
    ctx.fillRect(tx, ry, totalColW, rowH);
    ctx.strokeStyle = '#cbd5e1';
    ctx.strokeRect(tx, ry, totalColW, rowH);

    ctx.fillStyle = '#0f2354';
    ctx.font = '900 15.5px Arial, sans-serif';
    ctx.textAlign = 'center';
    ctx.fillText(String(ptjItem.count), tx + totalColW / 2, ry + rowH / 2 + 5);
  });

  const fy = tblY + headerH + bodyRowsCount * rowH;
  ctx.fillStyle = '#0f2354';
  ctx.fillRect(tblX, fy, tblW - totalColW, footerH);

  ctx.fillStyle = '#fef08a';
  ctx.font = '900 17px Arial, sans-serif';
  ctx.textAlign = 'center';
  ctx.fillText('GRAND TOTAL', tblX + ptjColW / 2, fy + 25);

  matrixGreds.forEach((g, cIdx) => {
    const gx = tblX + ptjColW + cIdx * singleGredW;
    ctx.strokeStyle = 'rgba(255,255,255,0.2)';
    ctx.lineWidth = 1;
    ctx.strokeRect(gx, fy, singleGredW, footerH);

    const cVal = colTotals[g] || 0;
    ctx.fillStyle = cVal > 0 ? '#ffffff' : '#94a3b8';
    ctx.font = '900 15.5px Arial, sans-serif';
    ctx.textAlign = 'center';
    ctx.fillText(String(cVal), gx + singleGredW / 2, fy + 25);
  });

  const grandTotalX = tblX + tblW - totalColW;
  ctx.fillStyle = '#facc15';
  ctx.fillRect(grandTotalX, fy, totalColW, footerH);
  ctx.fillStyle = '#0f2354';
  ctx.font = '900 19px Arial, sans-serif';
  ctx.textAlign = 'center';
  ctx.fillText(String(totalStaf), grandTotalX + totalColW / 2, fy + 26);

  ctx.restore();

  ctx.strokeStyle = '#0f2354';
  ctx.lineWidth = 2.5;
  drawRoundRect(tblX, tblY, tblW, totalTblH, 14);
  ctx.stroke();

  return canvas.toDataURL('image/png');
};

// --- KOMPONEN PUBLIC DASHBOARD (STATISTIK AWAM TANPA LOG MASUK) ---
const PublicDashboard = () => {
  const [activeTab, setActiveTab] = useState('kakitangan');
  const [staffData, setStaffData] = useState([]);
  const [isLoading, setIsLoading] = useState(true);

  const [showInfographicModal, setShowInfographicModal] = useState(false);
  const [infographicUrl, setInfographicUrl] = useState('');
  const [isGeneratingInfo, setIsGeneratingInfo] = useState(false);
  const [customBuildingPhoto, setCustomBuildingPhoto] = useState(() => {
    try {
      return localStorage.getItem('risda_prn_building_photo_v1') || '';
    } catch (e) {
      return '';
    }
  });
  const buildingPhotoInputRef = useRef(null);

  const [selPtj, setSelPtj] = useState('');
  const [selSkim, setSelSkim] = useState('');
  const [selGred, setSelGred] = useState('');
  const [selJantina, setSelJantina] = useState('');

  const tabs = [
    { id: 'kakitangan', label: 'Statistik Kakitangan', icon: Users },
    { id: 'kpi', label: 'KPI Mesyuarat', icon: Target },
    { id: 'evetting', label: 'Status e-Vetting', icon: ShieldCheck },
    { id: 'kesihatan', label: 'Penyakit Kronik', icon: Activity },
    { id: 'pengesahan', label: 'Pengesahan Jawatan', icon: CheckSquare }
  ];

  useEffect(() => {
    if (activeTab !== 'kakitangan') return;
    const fetchGoogleSheetsData = async () => {
      setIsLoading(true);
      try {
        const parsedData = await loadStaffSheetSmart();
        
        if (parsedData.length > 1) {
          const headers = parsedData[0].map(h => h.trim().toUpperCase());
          const currentYear = new Date().getFullYear();
          
          const mappedData = parsedData.slice(1).map((row) => {
            const getVal = (keys) => {
              const arr = Array.isArray(keys) ? keys : [keys];
              for (let key of arr) {
                const idx = headers.findIndex(h => h.includes(key));
                if (idx !== -1 && row[idx]) return row[idx].trim();
              }
              return '-';
            };

            const nama = getVal('NAMA');
            const rawSkim = getVal('SKIM').trim().toUpperCase();
            const skimGred = rawSkim !== '-' ? rawSkim : 'LAIN';
            const skimGroup = (rawSkim || '').replace(/[0-9]/g, '').trim().toUpperCase() || 'LAIN';
            const rawPtj = getVal(['TANGGUNGJAWAB', 'TANGUNGGJAWAB', 'PTJ', 'PUSAT']);
            const ptj = rawPtj && rawPtj !== '-' ? rawPtj.replace(/PEJABAT RISDA DAERAH|PEJABAT PRD -|PEJABAT/gi, '').trim() : 'Lain-lain';
            const rawJantina = getVal('JANTINA').trim().toUpperCase();
            const jantina = rawJantina.startsWith('L') ? 'Lelaki' : (rawJantina.startsWith('P') ? 'Perempuan' : rawJantina);
            
            let umurSemasa = null; 
            let ageCohortStr = 'Lain-lain';
            const noKp = getVal(['NO KP', 'KAD PENGENALAN', 'IC']).replace(/[^0-9]/g, '');
            let tarikhLahir = getVal(['TARIKH LAHIR', 'DOB']);
            if ((!tarikhLahir || tarikhLahir === '-') && noKp && noKp.length >= 6) {
              const yy = noKp.substring(0, 2); 
              const mm = noKp.substring(2, 4); 
              const dd = noKp.substring(4, 6);
              const yearPrefix = parseInt(yy, 10) > 30 ? "19" : "20";
              tarikhLahir = `${dd}/${mm}/${yearPrefix}${yy}`;
            }
            if (tarikhLahir !== '-') {
              const parts = tarikhLahir.split(/[\/\-.]/);
              if (parts.length === 3) {
                const birthYear = parseInt(parts[2].length === 4 ? parts[2] : (parseInt(parts[2]) > 30 ? '19'+parts[2] : '20'+parts[2]), 10);
                if (birthYear > 1900 && birthYear <= currentYear) umurSemasa = currentYear - birthYear;
              }
            }
            if (umurSemasa) {
              if (umurSemasa < 30) ageCohortStr = 'Bawah 30 Thn';
              else if (umurSemasa <= 40) ageCohortStr = '31 - 40 Thn';
              else if (umurSemasa <= 50) ageCohortStr = '41 - 50 Thn';
              else ageCohortStr = '51 Thn Ke Atas';
            }
            
            const tarikhBersara = getVal('TARIKH BERSARA');
            const isRetiring = tarikhBersara.includes((currentYear + 1).toString());

            return { nama, skimGred, skimGroup, ptj, jantina, ageCohort: ageCohortStr, isRetiring };
          }).filter(s => s.nama !== '-' && s.nama !== '');
          setStaffData(mappedData);
        }
        setIsLoading(false);
      } catch (error) { 
        setIsLoading(false); 
      }
    };
    fetchGoogleSheetsData();
  }, [activeTab]);

  const uniquePtjs = useMemo(() => [...new Set(staffData.map(s => s.ptj))].sort(), [staffData]);
  const uniqueSkims = useMemo(() => [...new Set(staffData.map(s => s.skimGroup))].sort(), [staffData]);
  
  const uniqueGreds = useMemo(() => {
    let sourceStaff = staffData;
    if (selSkim && selSkim !== 'Semua') {
      sourceStaff = staffData.filter(s => s.skimGroup === selSkim);
    }
    return [...new Set(sourceStaff.map(s => s.skimGred).filter(g => g && g !== 'LAIN'))].sort((a, b) => {
      const numA = parseInt(a.replace(/\D/g, ''), 10) || 0;
      const numB = parseInt(b.replace(/\D/g, ''), 10) || 0;
      if (numA !== numB) return numB - numA;
      return a.localeCompare(b);
    });
  }, [staffData, selSkim]);

  useEffect(() => {
    if (selGred && selGred !== 'Semua' && !uniqueGreds.includes(selGred)) {
      setSelGred('');
    }
  }, [uniqueGreds, selGred]);

  const activeStaff = useMemo(() => {
    return staffData.filter(s => {
      if (selPtj && selPtj !== 'Semua' && s.ptj !== selPtj) return false;
      if (selSkim && selSkim !== 'Semua' && s.skimGroup !== selSkim) return false;
      if (selGred && selGred !== 'Semua' && s.skimGred !== selGred) return false;
      if (selJantina && selJantina !== 'Semua' && s.jantina !== selJantina) return false;
      return true;
    });
  }, [staffData, selPtj, selSkim, selGred, selJantina]);

  const handleResetPublicFilters = () => {
    setSelPtj(''); setSelSkim(''); setSelGred(''); setSelJantina('');
  };

  const hasActiveFilters = Boolean(
    (selPtj && selPtj !== 'Semua') || 
    (selSkim && selSkim !== 'Semua') || 
    (selGred && selGred !== 'Semua') || 
    (selJantina && selJantina !== 'Semua')
  );

  const handleOpenInfographic = async (overrideBuilding = customBuildingPhoto) => {
    setIsGeneratingInfo(true);
    setShowInfographicModal(true);
    try {
      const dataSource = activeStaff.length > 0 ? activeStaff : staffData;
      const url = await generateInfographicDataUrl(dataSource, overrideBuilding);
      if (url) {
        setInfographicUrl(url);
      } else {
        const fallbackCanvas = document.createElement('canvas');
        fallbackCanvas.width = 1280;
        fallbackCanvas.height = 720;
        const fCtx = fallbackCanvas.getContext('2d');
        if (fCtx) {
          fCtx.fillStyle = '#0f2354';
          fCtx.fillRect(0, 0, 1280, 720);
          fCtx.fillStyle = '#facc15';
          fCtx.font = 'bold 36px Arial, sans-serif';
          fCtx.fillText('RINGKASAN BILANGAN STAF RISDA NEGERI PAHANG', 60, 110);
          fCtx.fillStyle = '#ffffff';
          fCtx.font = 'bold 28px Arial, sans-serif';
          fCtx.fillText(`Jumlah Kakitangan: ${dataSource.length} orang`, 60, 175);
          setInfographicUrl(fallbackCanvas.toDataURL('image/png'));
        }
      }
    } catch (err) {
      console.error('Ralat menjana infografik:', err);
    } finally {
      setIsGeneratingInfo(false);
    }
  };

  const handleUploadBuildingPhoto = (e) => {
    const file = e.target.files?.[0];
    if (!file) return;
    const reader = new FileReader();
    reader.onload = async (ev) => {
      const dataUrl = String(ev.target?.result || '');
      setCustomBuildingPhoto(dataUrl);
      try {
        localStorage.setItem('risda_prn_building_photo_v1', dataUrl);
      } catch (err) {}
      await handleOpenInfographic(dataUrl);
    };
    reader.readAsDataURL(file);
  };

  const handleDownloadInfographicPNG = () => {
    if (!infographicUrl) return;
    const dateStamp = new Date().toISOString().slice(0, 10).replace(/-/g, '');
    const link = document.createElement('a');
    link.href = infographicUrl;
    link.download = `Summary_Staf_RISDA_Pahang_${dateStamp}.png`;
    document.body.appendChild(link);
    link.click();
    document.body.removeChild(link);
  };

  const handlePrintInfographicPDF = () => {
    if (!infographicUrl) return;
    const printWin = window.open('', '_blank');
    if (!printWin) return;
    printWin.document.open();
    printWin.document.write(`
      <!DOCTYPE html>
      <html>
        <head>
          <title>Infografik Bilangan Staf RISDA Negeri Pahang</title>
          <style>
            @page { size: landscape; margin: 0; }
            body { margin: 0; padding: 0; display: flex; justify-content: center; align-items: center; background: #fff; }
            img { width: 100vw; height: auto; max-height: 100vh; object-fit: contain; }
          </style>
        </head>
        <body>
          <img src="${infographicUrl}" />
          <script>window.onload = function() { setTimeout(function() { window.print(); }, 400); }</script>
        </body>
      </html>
    `);
    printWin.document.close();
  };

  const totalStaffCount = activeStaff.length;
  const male = activeStaff.filter(s => s.jantina === 'Lelaki').length;
  const female = activeStaff.filter(s => s.jantina === 'Perempuan').length;
  const malePct = totalStaffCount > 0 ? ((male / totalStaffCount) * 100).toFixed(1) : 0;
  const femalePct = totalStaffCount > 0 ? ((female / totalStaffCount) * 100).toFixed(1) : 0;

  const ageCohorts = ['Bawah 30 Thn', '31 - 40 Thn', '41 - 50 Thn', '51 Thn Ke Atas'];
  const ageGenderData = useMemo(() => {
    return ageCohorts.map(cohort => {
      const group = activeStaff.filter(s => s.ageCohort === cohort);
      return {
        cohort,
        total: group.length,
        male: group.filter(s => s.jantina === 'Lelaki').length,
        female: group.filter(s => s.jantina === 'Perempuan').length
      };
    });
  }, [activeStaff]);

  const maxAgeGenderSide = useMemo(() => {
    const vals = ageGenderData.flatMap(d => [d.male, d.female]);
    return Math.max(...vals, 1);
  }, [ageGenderData]);

  const skimStats = useMemo(() => {
    const counts = {};
    activeStaff.forEach(s => { counts[s.skimGroup] = (counts[s.skimGroup] || 0) + 1; });
    return Object.entries(counts).map(([name, count]) => ({ name, count })).sort((a, b) => b.count - a.count);
  }, [activeStaff]);
  
  const donutColors = ['#0ea5e9', '#a855f7', '#f59e0b', '#10b981', '#f43f5e', '#64748b'];
  let currentPct = 0;
  const stops = skimStats.map((item, i) => {
    const pct = totalStaffCount > 0 ? (item.count / totalStaffCount) * 100 : 0;
    const color = donutColors[i % donutColors.length];
    const stop = `${color} ${currentPct}% ${currentPct + pct}%`;
    currentPct += pct;
    return stop;
  }).join(', ');
  const conicBg = `conic-gradient(${stops || 'transparent 100%'})`;

  const ptjStats = useMemo(() => {
    const counts = {};
    activeStaff.forEach(s => { counts[s.ptj] = (counts[s.ptj] || 0) + 1; });
    return Object.entries(counts).map(([name, count]) => ({ name, count })).sort((a, b) => b.count - a.count).slice(0, 9);
  }, [activeStaff]);
  const maxPtj = Math.max(...ptjStats.map(p => p.count), 1);

  const gredStats = useMemo(() => {
    const gredCounts = {};
    activeStaff.forEach(s => {
      const g = s.skimGred || 'LAIN';
      gredCounts[g] = (gredCounts[g] || 0) + 1;
    });

    return Object.entries(gredCounts).map(([gred, total]) => {
      const num = parseInt(gred.replace(/\D/g, ''), 10) || 0;
      return { gred, num, total };
    }).sort((a, b) => {
      if (b.num !== a.num) return b.num - a.num;
      return b.total - a.total;
    });
  }, [activeStaff]);

  const gredSvgWidth = Math.max(520, gredStats.length * 46);
  const maxGredTotal = Math.max(...gredStats.map(g => g.total), 1);
  const gredPoints = gredStats.map((item, i) => {
    const count = gredStats.length;
    const padX = 24;
    const usableW = gredSvgWidth - padX * 2;
    const x = count > 1 ? padX + (i / (count - 1)) * usableW : gredSvgWidth / 2;
    const y = 135 - ((item.total / maxGredTotal) * 100);
    return { x, y, val: item.total, gred: item.gred };
  });
  const gredPathD = gredPoints.length > 1
    ? `M${gredPoints[0].x},${gredPoints[0].y} ` + gredPoints.slice(1).map(p => `L${p.x},${p.y}`).join(' ')
    : '';
  const gredAreaD = gredPoints.length > 1
    ? `${gredPathD} L${gredPoints[gredPoints.length - 1].x},150 L${gredPoints[0].x},150 Z`
    : '';

  return (
    <div className="flex flex-col md:flex-row bg-[#0b1120] text-slate-200 rounded-2xl shadow-2xl border border-slate-700/60 overflow-hidden min-h-[800px] font-sans mb-12">
      <div className="w-full md:w-64 lg:w-72 bg-[#121a2f] border-r border-slate-700/60 flex flex-col shrink-0">
        <div className="p-5 border-b border-slate-700/60 bg-gradient-to-r from-blue-900/40 to-transparent">
           <h2 className="text-lg font-black text-white flex items-center tracking-wide"><Activity className="w-5 h-5 mr-2 text-cyan-400"/> Sistem Analitik</h2>
           <p className="text-[10px] text-cyan-200/60 mt-1 uppercase font-bold tracking-widest">Edisi Interaktif</p>
        </div>

        <div className="p-4 space-y-1.5 border-b border-slate-700/60">
           <div className="text-[10px] font-bold text-slate-500 uppercase mb-3 tracking-widest pl-1">Modul Utama</div>
           {tabs.map(tab => {
             const IconComponent = tab.icon;
             return (
               <button 
                  key={tab.id}
                  onClick={() => setActiveTab(tab.id)}
                  className={`w-full flex items-center px-4 py-2.5 rounded-lg text-sm font-semibold transition-all duration-300 ${activeTab === tab.id ? 'bg-indigo-600/90 text-white shadow-md border border-indigo-500/50 translate-x-1' : 'text-slate-400 hover:bg-slate-800/80 hover:text-slate-200 border border-transparent'}`}
                >
                   <IconComponent className={`w-4 h-4 mr-3 ${activeTab === tab.id ? 'text-cyan-300' : 'text-slate-500'}`} /> {tab.label}
               </button>
             );
           })}
        </div>

        {activeTab === 'kakitangan' && (
           <div className="p-4 flex-1 overflow-y-auto [&::-webkit-scrollbar]:w-1.5 [&::-webkit-scrollbar-track]:bg-transparent [&::-webkit-scrollbar-thumb]:bg-slate-700 [&::-webkit-scrollbar-thumb]:rounded-full">
              <div className="text-[10px] font-bold text-cyan-400 uppercase mb-4 tracking-widest flex justify-between items-center pl-1 pb-2 border-b border-slate-700/60">
                 <span className="flex items-center"><Filter className="w-3.5 h-3.5 mr-1.5 text-cyan-400"/> PENAPIS DATA</span>
                 {hasActiveFilters && (
                   <button onClick={handleResetPublicFilters} className="text-[10px] text-yellow-400 hover:text-yellow-300 font-semibold flex items-center transition-colors" title="Set Semula Semua Penapis"><RotateCcw className="w-3 h-3 mr-1"/> Semula</button>
                 )}
              </div>

              <div className="mb-4">
                 <label className="block text-xs font-semibold text-slate-300 mb-1.5">Pusat Tanggungjawab</label>
                 <select value={selPtj || 'Semua'} onChange={(e) => setSelPtj(e.target.value === 'Semua' ? '' : e.target.value)} className="w-full text-xs font-medium bg-[#0f172a] text-slate-200 border border-slate-700 rounded-lg px-3 py-2.5 outline-none focus:border-cyan-400 focus:ring-1 focus:ring-cyan-400 transition-all cursor-pointer">
                   <option value="Semua">Semua Pusat Tanggungjawab</option>{uniquePtjs.map(p => <option key={p} value={p}>{p}</option>)}
                 </select>
              </div>

              <div className="mb-4">
                 <label className="block text-xs font-semibold text-slate-300 mb-1.5">Kumpulan Skim</label>
                 <select value={selSkim || 'Semua'} onChange={(e) => { setSelSkim(e.target.value === 'Semua' ? '' : e.target.value); setSelGred(''); }} className="w-full text-xs font-medium bg-[#0f172a] text-slate-200 border border-slate-700 rounded-lg px-3 py-2.5 outline-none focus:border-purple-400 focus:ring-1 focus:ring-purple-400 transition-all cursor-pointer">
                   <option value="Semua">Semua Kumpulan Skim</option>{uniqueSkims.map(s => <option key={s} value={s}>Skim {s}</option>)}
                 </select>
              </div>

              <div className="mb-4">
                 <div className="flex justify-between items-center mb-1.5">
                   <label className="text-xs font-semibold text-slate-300">Gred Jawatan</label>
                   {selSkim && selSkim !== 'Semua' && <span className="text-[10px] font-bold text-yellow-400 font-mono">(Skim {selSkim})</span>}
                 </div>
                 <select value={selGred || 'Semua'} onChange={(e) => setSelGred(e.target.value === 'Semua' ? '' : e.target.value)} className="w-full text-xs font-medium font-mono bg-[#0f172a] text-slate-200 border border-slate-700 rounded-lg px-3 py-2.5 outline-none focus:border-yellow-400 focus:ring-1 focus:ring-yellow-400 transition-all cursor-pointer">
                   <option value="Semua">{selSkim && selSkim !== 'Semua' ? `Semua Gred Skim ${selSkim}` : 'Semua Gred Jawatan'}</option>
                   {uniqueGreds.map(g => <option key={g} value={g}>{g}</option>)}
                 </select>
              </div>

              <div className="mb-4">
                 <label className="block text-xs font-semibold text-slate-300 mb-1.5">Jantina</label>
                 <select value={selJantina || 'Semua'} onChange={(e) => setSelJantina(e.target.value === 'Semua' ? '' : e.target.value)} className="w-full text-xs font-medium bg-[#0f172a] text-slate-200 border border-slate-700 rounded-lg px-3 py-2.5 outline-none focus:border-emerald-400 focus:ring-1 focus:ring-emerald-400 transition-all cursor-pointer">
                   <option value="Semua">Semua Jantina</option><option value="Lelaki">Lelaki</option><option value="Perempuan">Perempuan</option>
                 </select>
              </div>
           </div>
        )}
      </div>

      <div className="flex-1 bg-[radial-gradient(ellipse_at_top_right,_var(--tw-gradient-stops))] from-slate-800 via-[#0b1120] to-[#070b14] p-5 md:p-8 overflow-y-auto [&::-webkit-scrollbar]:w-2 [&::-webkit-scrollbar-track]:bg-[#0b1120] [&::-webkit-scrollbar-thumb]:bg-slate-700 [&::-webkit-scrollbar-thumb]:rounded-full relative">
        {activeTab === 'kakitangan' ? (
          isLoading ? (
            <div className="flex flex-col items-center justify-center h-full">
              <div className="inline-block animate-spin rounded-full h-12 w-12 border-t-2 border-b-2 border-cyan-400 mb-4"></div>
              <p className="text-cyan-400 font-medium animate-pulse">Menghubungkan set data awam...</p>
            </div>
          ) : (
            <div className="animate-in fade-in zoom-in-95 duration-500">
              
              <div className="flex flex-col sm:flex-row justify-between items-start sm:items-center mb-6 gap-4">
                <div>
                   <h1 className="text-2xl md:text-3xl font-black text-white tracking-tight uppercase">GAMBARAN KESELURUHAN KAKITANGAN</h1>
                   <p className="text-xs text-slate-400 mt-0.5">Perincian bilangan tenaga kerja warga RISDA Negeri Pahang terus dari pangkalan data awam.</p>
                </div>
                <div className="flex flex-wrap sm:flex-col items-start sm:items-end gap-2">
                   <div className="flex flex-col sm:items-end">
                     <span className="text-[10px] font-bold text-slate-500 uppercase">Set Data Pada</span>
                     <span className="text-sm font-bold text-cyan-400">{new Date().toLocaleDateString('ms-MY', { day: '2-digit', month: 'long', year: 'numeric' })}</span>
                   </div>
                   <div className="flex items-center gap-2 mt-1">
                     <button
                       type="button"
                       onClick={() => handleOpenInfographic()}
                       disabled={isGeneratingInfo}
                       className="px-3.5 py-2 bg-gradient-to-r from-blue-800 to-indigo-700 hover:from-blue-700 hover:to-indigo-600 disabled:opacity-60 text-white text-xs font-bold rounded-lg shadow-lg border border-amber-400/70 flex items-center transition-all transform hover:scale-[1.02] cursor-pointer"
                       title="Jana & Muat Turun Ringkasan Infografik Rasmi"
                     >
                       <ImageIcon className="w-4 h-4 mr-1.5 text-yellow-400" />
                       {isGeneratingInfo ? 'Menjana Poster...' : 'Muat Turun Infografik'}
                     </button>
                     {hasActiveFilters && (
                       <button onClick={handleResetPublicFilters} className="text-[10px] text-slate-300 hover:text-white bg-slate-800 hover:bg-slate-700 px-2.5 py-2 rounded-lg border border-slate-600 flex items-center transition-colors">
                         <RotateCcw className="w-3 h-3 mr-1"/> Set Semula
                       </button>
                     )}
                   </div>
                </div>
              </div>

              <div className="bg-[#0f172a]/95 backdrop-blur-md border border-slate-700/70 rounded-2xl p-6 shadow-2xl mb-8 relative overflow-hidden">
                <div className="absolute top-0 right-0 w-96 h-96 bg-cyan-500/5 rounded-full blur-3xl pointer-events-none"></div>
                <div className="grid grid-cols-1 lg:grid-cols-12 gap-8 items-center">
                  
                  <div className="lg:col-span-3 bg-[#131d35]/70 rounded-xl p-5 border border-slate-700/50 flex flex-col justify-around h-full space-y-4 shadow-inner">
                    <div className="border-l-4 border-cyan-400 pl-3.5 py-1">
                      <div className="text-3xl md:text-4xl font-black text-white tracking-tight">{totalStaffCount}</div>
                      <div className="text-xs font-semibold text-slate-400 mt-0.5">Jumlah Kakitangan</div>
                    </div>
                    <div className="border-l-4 border-amber-500 pl-3.5 py-1">
                      <div className="text-2xl md:text-3xl font-black text-amber-400 tracking-tight">{male}</div>
                      <div className="text-xs font-semibold text-slate-400 mt-0.5">Kakitangan Lelaki</div>
                    </div>
                    <div className="border-l-4 border-rose-600 pl-3.5 py-1">
                      <div className="text-2xl md:text-3xl font-black text-rose-500 tracking-tight">{female}</div>
                      <div className="text-xs font-semibold text-slate-400 mt-0.5">Kakitangan Perempuan</div>
                    </div>
                  </div>

                  <div className="lg:col-span-3 flex flex-col items-center justify-around py-2 space-y-6">
                    <div className="flex flex-col items-center group">
                      <div className="text-3xl font-black text-amber-400 tracking-tight font-mono leading-none">{male}</div>
                      <span className="text-[11px] font-bold text-slate-400 mt-1 mb-2 font-mono">({malePct}%)</span>
                      <div className="relative w-16 h-20 flex items-center justify-center">
                        <svg viewBox="0 0 100 125" className="w-14 h-18 overflow-visible">
                          <defs>
                            <clipPath id="maleClip"><rect x="0" y={125 - (125 * (malePct / 100))} width="100" height="125" /></clipPath>
                          </defs>
                          <g fill="#334155" opacity="0.6">
                            <circle cx="50" cy="18" r="14" />
                            <path d="M28 40 C28 35, 34 35, 50 35 C66 35, 72 35, 72 40 L76 72 C76 76, 70 76, 68 72 L66 52 L62 52 L62 116 C62 120, 53 120, 53 116 L53 82 L47 82 L47 116 C47 120, 38 120, 38 116 L38 52 L34 52 L32 72 C30 76, 24 76, 24 72 Z" />
                          </g>
                          <g fill="#f59e0b" clipPath="url(#maleClip)">
                            <circle cx="50" cy="18" r="14" />
                            <path d="M28 40 C28 35, 34 35, 50 35 C66 35, 72 35, 72 40 L76 72 C76 76, 70 76, 68 72 L66 52 L62 52 L62 116 C62 120, 53 120, 53 116 L53 82 L47 82 L47 116 C47 120, 38 120, 38 116 L38 52 L34 52 L32 72 C30 76, 24 76, 24 72 Z" />
                          </g>
                        </svg>
                      </div>
                      <span className="text-[10px] font-bold text-amber-400 uppercase tracking-widest mt-1">Lelaki</span>
                    </div>

                    <div className="flex flex-col items-center group">
                      <div className="text-3xl font-black text-rose-500 tracking-tight font-mono leading-none">{female}</div>
                      <span className="text-[11px] font-bold text-slate-400 mt-1 mb-2 font-mono">({femalePct}%)</span>
                      <div className="relative w-16 h-20 flex items-center justify-center">
                        <svg viewBox="0 0 100 125" className="w-14 h-18 overflow-visible">
                          <defs>
                            <clipPath id="femaleClip"><rect x="0" y={125 - (125 * (femalePct / 100))} width="100" height="125" /></clipPath>
                          </defs>
                          <g fill="#334155" opacity="0.6">
                            <circle cx="50" cy="18" r="14" />
                            <path d="M34 40 C34 35, 38 35, 50 35 C62 35, 66 35, 66 40 L72 74 C72 78, 66 78, 64 74 L60 52 L57 52 L68 90 C69 94, 63 95, 62 92 L58 76 L58 116 C58 120, 52 120, 52 116 L52 82 L48 82 L48 116 C48 120, 42 120, 42 116 L42 76 L38 92 C37 95, 31 94, 32 90 L43 52 L40 52 L36 74 C34 78, 28 78, 28 74 Z" />
                          </g>
                          <g fill="#e11d48" clipPath="url(#femaleClip)">
                            <circle cx="50" cy="18" r="14" />
                            <path d="M34 40 C34 35, 38 35, 50 35 C62 35, 66 35, 66 40 L72 74 C72 78, 66 78, 64 74 L60 52 L57 52 L68 90 C69 94, 63 95, 62 92 L58 76 L58 116 C58 120, 52 120, 52 116 L52 82 L48 82 L48 116 C48 120, 42 120, 42 116 L42 76 L38 92 C37 95, 31 94, 32 90 L43 52 L40 52 L36 74 C34 78, 28 78, 28 74 Z" />
                          </g>
                        </svg>
                      </div>
                      <span className="text-[10px] font-bold text-rose-400 uppercase tracking-widest mt-1">Perempuan</span>
                    </div>
                  </div>

                  {/* KOTAK ATAS KANAN: PECAHAN UMUR & JANTINA */}
                  <div className="lg:col-span-6 bg-[#131d35]/60 rounded-xl p-5 border border-slate-700/50 flex flex-col justify-center">
                    <div className="flex flex-col sm:flex-row justify-between items-start sm:items-center mb-4 pb-2.5 border-b border-slate-700">
                      <div>
                        <h3 className="text-sm font-bold text-white tracking-wide flex items-center">
                          <TrendingUp className="w-4 h-4 mr-2 text-cyan-400"/> Pecahan Kakitangan Mengikut Umur & Jantina
                        </h3>
                        <p className="text-[11px] text-slate-400 mt-0.5">Taburan tenaga kerja lelaki dan perempuan mengikut kumpulan umur semasa</p>
                      </div>
                      <div className="flex items-center space-x-3 mt-2 sm:mt-0 text-xs font-bold">
                        <span className="flex items-center text-rose-400"><span className="w-2.5 h-2.5 rounded-full bg-rose-600 mr-1.5 inline-block"></span> Perempuan</span>
                        <span className="flex items-center text-amber-400"><span className="w-2.5 h-2.5 rounded-full bg-amber-500 mr-1.5 inline-block"></span> Lelaki</span>
                      </div>
                    </div>

                    <div className="space-y-3.5 pt-1">
                      {ageGenderData.map((item, idx) => {
                        const femaleWidthPct = maxAgeGenderSide > 0 ? (item.female / maxAgeGenderSide) * 100 : 0;
                        const maleWidthPct = maxAgeGenderSide > 0 ? (item.male / maxAgeGenderSide) * 100 : 0;

                        return (
                          <div 
                            key={idx} 
                            className="flex items-center group p-1.5 rounded-lg hover:bg-slate-800/40 transition-colors"
                          >
                            <div className="w-28 text-left text-xs font-bold text-slate-300 truncate pr-2 shrink-0 flex items-center">
                              <span className="w-2 h-2 rounded-full bg-cyan-400 mr-2 shrink-0"></span>
                              {item.cohort}
                            </div>
                            <div className="flex-1 flex items-center gap-1">
                              <div className="w-1/2 flex justify-end items-center h-6">
                                {item.female > 0 && (
                                  <div 
                                    className="h-full bg-rose-600/90 hover:bg-rose-500 rounded-l transition-all duration-500 flex items-center justify-start pl-2 shadow-sm min-w-[22px]" 
                                    style={{ width: `${Math.max(femaleWidthPct, 8)}%` }}
                                  >
                                    <span className="text-[11px] font-black text-white">{item.female}</span>
                                  </div>
                                )}
                              </div>
                              <div className="w-0.5 h-7 bg-slate-600 shrink-0"></div>
                              <div className="w-1/2 flex justify-start items-center h-6">
                                {item.male > 0 && (
                                  <div 
                                    className="h-full bg-amber-500 hover:bg-amber-400 rounded-r transition-all duration-500 flex items-center justify-end pr-2 shadow-sm min-w-[22px]" 
                                    style={{ width: `${Math.max(maleWidthPct, 8)}%` }}
                                  >
                                    <span className="text-[11px] font-black text-slate-950">{item.male}</span>
                                  </div>
                                )}
                              </div>
                            </div>
                            <span className="w-10 text-right text-xs font-black text-slate-300 pl-2">{item.total}</span>
                          </div>
                        );
                      })}
                    </div>
                  </div>
                </div>
              </div>

              {/* BARIS 2 KIRI: GRAF VISUAL PECAHAN MENGIKUT GRED JAWATAN */}
              <div className="grid grid-cols-1 lg:grid-cols-3 gap-6 mb-6">
                 <div className="lg:col-span-2 bg-slate-800/30 backdrop-blur-sm border border-slate-700/50 rounded-xl p-5 shadow-lg flex flex-col justify-between">
                    <div className="flex flex-col sm:flex-row justify-between items-start sm:items-center mb-6 gap-2">
                      <h3 className="text-sm font-semibold text-slate-200 flex items-center">
                        <TrendingUp className="w-4 h-4 mr-2 text-cyan-400"/> Pecahan Kakitangan Mengikut Gred Jawatan
                      </h3>
                      <span className="text-[11px] text-slate-400">Susunan hierarki gred tertinggi ke terendah (Klik titik untuk tapis)</span>
                    </div>
                    <div className="w-full overflow-x-auto pb-6 [&::-webkit-scrollbar]:h-1.5 [&::-webkit-scrollbar-thumb]:bg-slate-700 [&::-webkit-scrollbar-thumb]:rounded-full">
                      <div className="relative h-48" style={{ minWidth: `${gredSvgWidth}px` }}>
                        <svg viewBox={`0 0 ${gredSvgWidth} 150`} preserveAspectRatio="none" className="w-full h-full overflow-visible">
                          <defs>
                            <linearGradient id="gredAreaGradient" x1="0" y1="0" x2="0" y2="1">
                              <stop offset="0%" stopColor="#0ea5e9" stopOpacity="0.6" />
                              <stop offset="100%" stopColor="#0ea5e9" stopOpacity="0.0" />
                            </linearGradient>
                          </defs>
                          {gredPoints.length > 1 && (
                            <>
                              <path d={gredAreaD} fill="url(#gredAreaGradient)" />
                              <path d={gredPathD} fill="none" stroke="#0ea5e9" strokeWidth="3" />
                            </>
                          )}
                          {gredPoints.map((p, i) => {
                            const isSelected = selGred === p.gred;
                            return (
                              <g 
                                key={i} 
                                onClick={() => setSelGred(isSelected ? '' : p.gred)}
                                className="cursor-pointer group"
                              >
                                <circle 
                                  cx={p.x} 
                                  cy={p.y} 
                                  r={isSelected ? "7" : "5"} 
                                  fill={isSelected ? "#facc15" : "#0f172a"} 
                                  stroke={isSelected ? "#ffffff" : "#0ea5e9"} 
                                  strokeWidth="2.5" 
                                  className="transition-all duration-300"
                                />
                                <text 
                                  x={p.x} 
                                  y={p.y - 14} 
                                  fill={isSelected ? "#facc15" : "#e2e8f0"} 
                                  fontSize="12" 
                                  fontWeight="bold" 
                                  textAnchor="middle"
                                >
                                  {p.val}
                                </text>
                              </g>
                            );
                          })}
                        </svg>
                        <div className="absolute bottom-0 left-0 right-0 h-5">
                          {gredPoints.map((p, i) => {
                            const isSelected = selGred === p.gred;
                            return (
                              <button
                                key={i}
                                onClick={() => setSelGred(isSelected ? '' : p.gred)}
                                style={{ left: `${(p.x / gredSvgWidth) * 100}%` }}
                                className={`absolute -translate-x-1/2 top-1 text-[10px] font-mono font-bold transition-colors ${isSelected ? 'text-yellow-400 underline' : 'text-slate-400 hover:text-white'}`}
                                title={`Tapis Gred ${p.gred}`}
                              >
                                {p.gred}
                              </button>
                            );
                          })}
                        </div>
                      </div>
                    </div>
                 </div>

                 <div className="bg-slate-800/30 backdrop-blur-sm border border-slate-700/50 rounded-xl p-5 shadow-lg flex flex-col items-center justify-center">
                    <h3 className="text-sm font-semibold text-slate-200 mb-6 flex items-center w-full"><PieChart className="w-4 h-4 mr-2 text-fuchsia-400"/> Komposisi Skim</h3>
                    <div className="relative w-36 h-36 rounded-full flex items-center justify-center mb-6 shadow-[0_0_15px_rgba(0,0,0,0.5)]" style={{ background: conicBg }}>
                      <div className="absolute inset-2.5 bg-[#0f1526] rounded-full flex flex-col items-center justify-center">
                         <span className="text-2xl font-black text-white">{totalStaffCount}</span>
                         <span className="text-[9px] font-bold text-slate-400 uppercase tracking-wide">Staf</span>
                      </div>
                    </div>
                    <div className="w-full grid grid-cols-2 gap-x-2 gap-y-2">
                       {skimStats.slice(0, 6).map((item, i) => (
                          <div key={i} className="flex items-center text-[10px] font-medium text-slate-300">
                             <div className="w-2.5 h-2.5 rounded-full mr-1.5 shrink-0" style={{ backgroundColor: donutColors[i % donutColors.length] }}></div>
                             <span className="truncate flex-1">Skim {item.name}</span>
                             <span className="font-bold text-white ml-1">{item.count}</span>
                          </div>
                       ))}
                    </div>
                 </div>
              </div>

              <div className="grid grid-cols-1 lg:grid-cols-2 gap-6 pb-4">
                 <div className="bg-slate-800/30 backdrop-blur-sm border border-slate-700/50 rounded-xl p-5 shadow-lg flex flex-col justify-between">
                    <div>
                      <h3 className="text-sm font-semibold text-slate-200 mb-2 flex items-center"><Target className="w-4 h-4 mr-2 text-rose-400"/> Status Persaraan & Unjuran Perkhidmatan</h3>
                      <p className="text-xs text-slate-400 mb-5">Unjuran penamatan perkhidmatan kakitangan aktif RISDA Pahang.</p>
                      <div className="grid grid-cols-2 gap-4">
                        <div className="bg-slate-800/60 p-4 rounded-xl border border-slate-700">
                          <span className="text-[10px] font-bold text-slate-400 uppercase tracking-wider block">Bakal Bersara ({new Date().getFullYear() + 1})</span>
                          <span className="text-3xl font-black text-rose-400 mt-1 block">{activeStaff.filter(s => s.isRetiring).length}</span>
                          <span className="text-[11px] text-slate-400 mt-1 block">kakitangan</span>
                        </div>
                        <div className="bg-slate-800/60 p-4 rounded-xl border border-slate-700">
                          <span className="text-[10px] font-bold text-slate-400 uppercase tracking-wider block">Kakitangan Aktif Terkini</span>
                          <span className="text-3xl font-black text-emerald-400 mt-1 block">{totalStaffCount}</span>
                          <span className="text-[11px] text-slate-400 mt-1 block">orang berkhidmat</span>
                        </div>
                      </div>
                    </div>
                    <div className="mt-4 pt-3 border-t border-slate-700/60 flex items-center justify-between text-xs text-slate-400">
                      <span>Nisbah Jantina Semasa:</span>
                      <span className="font-bold text-white"><span className="text-amber-400">{male} Lelaki</span> / <span className="text-rose-400">{female} Perempuan</span></span>
                    </div>
                 </div>

                 <div className="bg-slate-800/30 backdrop-blur-sm border border-slate-700/50 rounded-xl p-5 shadow-lg">
                    <h3 className="text-sm font-semibold text-slate-200 mb-5 flex items-center"><List className="w-4 h-4 mr-2 text-amber-400"/> Kepadatan Kakitangan (PTJ)</h3>
                    <div className="flex flex-col gap-3.5">
                       {ptjStats.map((item, i) => {
                          const wPct = maxPtj > 0 ? (item.count / maxPtj) * 100 : 0;
                          return (
                             <div key={i} className="flex items-center group">
                                <span className="w-24 text-[10px] font-medium text-slate-300 truncate pr-2" title={item.name}>{item.name}</span>
                                <div className="flex-1 h-3.5 bg-slate-800/80 rounded-sm overflow-hidden flex items-center">
                                   <div className="h-full bg-gradient-to-r from-indigo-600 to-indigo-400 rounded-sm relative" style={{ width: `${wPct}%` }}></div>
                                </div>
                                <span className="w-8 text-right text-xs font-bold text-indigo-300 ml-2">{item.count}</span>
                             </div>
                          );
                       })}
                    </div>
                 </div>
              </div>
            </div>
          )
        ) : (
          <div className="flex-1 flex flex-col items-center justify-center h-full p-8">
             <h3 className="text-2xl font-bold text-white mb-3">Menunggu Integrasi Data</h3>
             <p className="text-slate-400 text-center max-w-md mb-8">Modul <strong className="text-white">{tabs.find(t => t.id === activeTab)?.label}</strong> akan dipautkan ke pangkalan data awam tidak lama lagi.</p>
             <button onClick={() => setActiveTab('kakitangan')} className="px-6 py-2 bg-indigo-600 text-white font-bold rounded-lg">Kembali ke Statistik Kakitangan</button>
          </div>
        )}

        {showInfographicModal && (
          <div className="fixed inset-0 z-50 flex items-center justify-center p-4 bg-black/80 backdrop-blur-sm animate-in fade-in duration-200">
            <div className="bg-[#0f172a] border border-slate-700 rounded-2xl shadow-2xl w-full max-w-6xl max-h-[92vh] flex flex-col overflow-hidden">
              <div className="p-4 sm:px-6 bg-gradient-to-r from-[#0f2354] to-[#1e3a8a] border-b border-slate-700 flex flex-wrap justify-between items-center gap-3">
                <div>
                  <h3 className="text-lg font-black text-white flex items-center">
                    <ImageIcon className="w-5 h-5 mr-2 text-yellow-400" />
                    Ringkasan Infografik Bilangan Staf RISDA Negeri Pahang
                  </h3>
                  <p className="text-xs text-blue-200 mt-0.5">
                    Tema Korporat Biru & Emas, Logo Lutsinar & Bangunan PRN Pahang ({activeStaff.length} kakitangan).
                  </p>
                </div>
                <div className="flex flex-wrap items-center gap-2">
                  <input
                    ref={buildingPhotoInputRef}
                    type="file"
                    accept="image/*"
                    onChange={handleUploadBuildingPhoto}
                    className="hidden"
                  />
                  <button
                    type="button"
                    onClick={() => buildingPhotoInputRef.current?.click()}
                    className="px-3 py-2 bg-blue-950/80 hover:bg-blue-900 text-blue-100 text-xs font-bold rounded-lg border border-blue-700 flex items-center transition-colors"
                  >
                    <Upload className="w-3.5 h-3.5 mr-1.5 text-yellow-400" />
                    {customBuildingPhoto ? 'Tukar Gambar Bangunan' : 'Pilih Gambar Bangunan'}
                  </button>
                  <button
                    type="button"
                    onClick={handleDownloadInfographicPNG}
                    disabled={!infographicUrl}
                    className="px-4 py-2 bg-emerald-600 hover:bg-emerald-500 disabled:opacity-50 text-white text-xs sm:text-sm font-bold rounded-lg shadow-md flex items-center transition-colors"
                  >
                    <Download className="w-4 h-4 mr-1.5" /> Muat Turun Gambar (PNG)
                  </button>
                  <button
                    type="button"
                    onClick={handlePrintInfographicPDF}
                    disabled={!infographicUrl}
                    className="px-4 py-2 bg-yellow-500 hover:bg-yellow-400 disabled:opacity-50 text-blue-950 text-xs sm:text-sm font-bold rounded-lg shadow-md flex items-center transition-colors"
                  >
                    <Printer className="w-4 h-4 mr-1.5" /> Cetak / PDF
                  </button>
                  <button
                    type="button"
                    onClick={() => setShowInfographicModal(false)}
                    className="p-2 bg-blue-950 hover:bg-red-600 text-slate-300 hover:text-white rounded-lg transition-colors ml-1"
                    title="Tutup"
                  >
                    <X className="w-5 h-5" />
                  </button>
                </div>
              </div>

              <div className="p-4 sm:p-6 overflow-auto bg-[#070b14] flex justify-center items-center flex-1">
                {infographicUrl ? (
                  <img
                    src={infographicUrl}
                    alt="Infografik Bilangan Staf RISDA Negeri Pahang"
                    className="w-full h-auto max-h-[75vh] object-contain rounded-xl shadow-2xl border border-slate-700"
                  />
                ) : (
                  <p className="text-slate-400">Sedang menjana infografik...</p>
                )}
              </div>
            </div>
          </div>
        )}
      </div>
    </div>
  );
};

// --- KOMPONEN DASHBOARD SUMBER MANUSIA (HR) DALAMAN ---
const DashboardHR = () => {
  const [searchQuery, setSearchQuery] = useState('');
  const [filterPtj, setFilterPtj] = useState('Semua');
  const [filterSkim, setFilterSkim] = useState('Semua');
  const [filterTahunPT, setFilterTahunPT] = useState('');
  const [filterAgeCohort, setFilterAgeCohort] = useState('Semua');
  const [selectedStaff, setSelectedStaff] = useState(null);
  const [showRetiringOnly, setShowRetiringOnly] = useState(false);
  const [showAnalytics, setShowAnalytics] = useState(true);
  const [exportNotice, setExportNotice] = useState('');

  // Set semula tapisan
  const handleResetFilters = () => {
    setSearchQuery('');
    setFilterPtj('Semua');
    setFilterSkim('Semua');
    setShowRetiringOnly(false);
    setFilterTahunPT('');
    setFilterAgeCohort('Semua');
  };

  const isFiltered = searchQuery !== '' || filterPtj !== 'Semua' || filterSkim !== 'Semua' || showRetiringOnly || filterTahunPT !== '' || filterAgeCohort !== 'Semua';
  
  // State untuk Live Data dari Google Sheets
  const [staffData, setStaffData] = useState([]);
  const [isLoadingCSV, setIsLoadingCSV] = useState(true);

  useEffect(() => {
    const fetchGoogleSheetsData = async () => {
      try {
        const parsedData = await loadStaffSheetSmart();

        if (parsedData.length > 1) {
          const headers = parsedData[0].map(h => h.trim().toUpperCase());
          const pasanganColIdx = headers.findIndex(h => h.includes('NAMA PASANGAN') || h === 'PASANGAN');
          
          const currentDateObj = new Date();
          const currentYear = currentDateObj.getFullYear();
          const currentMonth = currentDateObj.getMonth() + 1;
          const currentDay = currentDateObj.getDate();
          
          const mappedData = parsedData.slice(1).map((row, index) => {
            const getVal = (keywords) => {
              const keys = Array.isArray(keywords) ? keywords : [keywords];
              for (let key of keys) {
                const idx = headers.findIndex(h => h.includes(key));
                if (idx !== -1 && row[idx]) return row[idx].trim();
              }
              return '-';
            };

            const nama = getVal('NAMA');
            const noKpIdx = headers.findIndex((h, i) => (pasanganColIdx === -1 || i < pasanganColIdx) && (h.includes('NO KP') || h.includes('KAD PENGENALAN') || h.includes('NO. KP') || h.includes('NO_KP') || h === 'IC'));
            const rawNoKp = (noKpIdx !== -1 && row[noKpIdx] ? row[noKpIdx].trim() : '').replace(/[^0-9]/g, '');
            const noKp = rawNoKp.length === 11 ? rawNoKp.padStart(12, '0') : rawNoKp;
            const rawGambar = getVal(['URL GAMBAR', 'GAMBAR', 'FOTO', 'PHOTO']);

            let tarikhLahir = getVal(['TARIKH LAHIR', 'TARIKH_LAHIR', 'DOB']);
            if ((!tarikhLahir || tarikhLahir === '-') && noKp && noKp.length >= 6) {
              const yy = noKp.substring(0, 2);
              const mm = noKp.substring(2, 4);
              const dd = noKp.substring(4, 6);
              const yearPrefix = parseInt(yy, 10) > 30 ? "19" : "20";
              tarikhLahir = `${dd}/${mm}/${yearPrefix}${yy}`;
            }

            // Umur Semasa Dinamik
            let birthYear = null;
            let umurSemasa = null;
            let ageCohortStr = 'Lain-lain';
            if (tarikhLahir !== '-') {
              const parts = tarikhLahir.split(/[\/\-.]/);
              if (parts.length === 3) {
                birthYear = parseInt(parts[2].length === 4 ? parts[2] : (parseInt(parts[2]) > 30 ? '19'+parts[2] : '20'+parts[2]), 10);
                if (birthYear > 1900 && birthYear <= currentYear) {
                    umurSemasa = currentYear - birthYear;
                    const bMonth = parseInt(parts[1], 10);
                    const bDay = parseInt(parts[0], 10);
                    if (currentMonth < bMonth || (currentMonth === bMonth && currentDay < bDay)) {
                        umurSemasa--;
                    }
                }
              }
            }
            if (umurSemasa) {
              if (umurSemasa < 30) ageCohortStr = 'Bawah 30 Thn';
              else if (umurSemasa <= 40) ageCohortStr = '31 - 40 Thn';
              else if (umurSemasa <= 50) ageCohortStr = '41 - 50 Thn';
              else ageCohortStr = '51 Thn Ke Atas';
            }

            // Resolusi URL Google Drive & Gambar Tempatan (/staf/NoKP.jpg)
            const resolveDriveUrl = (url) => {
              if (!url || url === '-') return '';
              const fileIdMatch = url.match(/\/d\/([a-zA-Z0-9_-]+)/);
              if (fileIdMatch && fileIdMatch[1]) return `https://lh3.googleusercontent.com/d/${fileIdMatch[1]}`;
              const idParamMatch = url.match(/[?&]id=([a-zA-Z0-9_-]+)/);
              if (idParamMatch && idParamMatch[1]) return `https://lh3.googleusercontent.com/d/${idParamMatch[1]}`;
              return url.startsWith('http') ? url : '';
            };

            const defaultAvatar = `https://ui-avatars.com/api/?name=${encodeURIComponent(nama)}&background=1e3a8a&color=facc15&size=128&bold=true`;
            const localJpg = noKp && noKp.length >= 6 ? `/staf/${noKp}.jpg` : '';
            const driveImageUrl = resolveDriveUrl(rawGambar);
            const finalGambar = localJpg || driveImageUrl || defaultAvatar;

            const noPekerja = getVal('NO PEKERJA');
            let rawSkim = getVal('SKIM');

            // Pengiraan Tempoh PT Terkini
            const tarikhPTSemasa = getVal(['DI TEMPATKAN', 'DITEMPATKAN', 'PT SEKARANG']);
            let ptDurationYears = 0;
            let ptDurationStr = '-';
            
            if (tarikhPTSemasa && tarikhPTSemasa !== '-') {
              const parts = tarikhPTSemasa.split(/[\/\-.]/);
              if (parts.length === 3) {
                const ptYear = parseInt(parts[2].length === 4 ? parts[2] : (parseInt(parts[2]) > 30 ? '19'+parts[2] : '20'+parts[2]), 10);
                const ptMonth = parseInt(parts[1], 10);
                const ptDay = parseInt(parts[0], 10);
                
                let yDiff = currentYear - ptYear;
                let mDiff = currentMonth - ptMonth;
                let dDiff = currentDay - ptDay;
                
                if (dDiff < 0) mDiff--;
                if (mDiff < 0) { yDiff--; mDiff += 12; }
                
                ptDurationYears = yDiff + (mDiff / 12);
                
                if (yDiff <= 0 && mDiff <= 0) ptDurationStr = 'Kurang Sebulan';
                else if (yDiff <= 0) ptDurationStr = `${mDiff} Bulan`;
                else if (mDiff === 0) ptDurationStr = `${yDiff} Tahun`;
                else ptDurationStr = `${yDiff} Tahun ${mDiff} Bulan`;
              }
            }

            // Tempoh Keseluruhan
            const tarikhLantikanStr = getVal(['LANTIKAN PERTAMA', 'TARIKHLANTIKAN', 'TARIKH LANTIKAN']);
            let totalYears = 0;
            let totalServiceFloat = 0;
            let tempohKeseluruhan = '-';
            if (tarikhLantikanStr && tarikhLantikanStr !== '-') {
              const parts = tarikhLantikanStr.split(/[\/\-.]/);
              if (parts.length === 3) {
                const lantikanYear = parseInt(parts[2].length === 4 ? parts[2] : (parseInt(parts[2]) > 30 ? '19'+parts[2] : '20'+parts[2]), 10);
                const lantikanMonth = parseInt(parts[1], 10);
                let yDiff = currentYear - lantikanYear;
                let mDiff = currentMonth - lantikanMonth;
                if (mDiff < 0) { yDiff--; mDiff += 12; }
                totalYears = Math.max(0, yDiff);
                totalServiceFloat = Math.max(0, yDiff + (mDiff / 12));
                if (yDiff < 0) tempohKeseluruhan = '0 Tahun';
                else if (mDiff === 0) tempohKeseluruhan = `${yDiff} Tahun`;
                else tempohKeseluruhan = `${yDiff} Tahun ${mDiff} Bulan`;
              }
            }

            // LOGIK AMARAN & BAKI TAHUN PERSARAAN
            let alertLevel = 'none';
            let alertMsgs = [];
            let bakiTahunBersara = 0;
            
            if (ptDurationYears >= 7) {
              alertLevel = 'red';
              alertMsgs.push(`Telah berkhidmat ${Math.floor(ptDurationYears)} tahun di PT yang sama (Stagnan)`);
            }
            
            const tarikhBersara = getVal('TARIKH BERSARA');
            const umurBersaraVal = parseInt(getVal('UMUR BERSARA'), 10) || 60;
            if (tarikhBersara && tarikhBersara !== '-') {
              const parts = tarikhBersara.split(/[\/\-.]/);
              if (parts.length === 3) {
                const retYear = parseInt(parts[2].length === 4 ? parts[2] : '20'+parts[2], 10);
                const retMonth = parseInt(parts[1], 10);
                const monthsToRetire = (retYear - currentYear) * 12 + (retMonth - currentMonth);
                bakiTahunBersara = Math.max(0, Number((monthsToRetire / 12).toFixed(1)));
                if (monthsToRetire > 0 && monthsToRetire <= 6) {
                  alertLevel = 'red';
                  alertMsgs.push(`Bakal bersara dalam masa ${monthsToRetire} bulan`);
                }
              }
            } else if (umurSemasa) {
              bakiTahunBersara = Math.max(0, umurBersaraVal - umurSemasa);
            }

            const rawJantina = getVal('JANTINA').trim().toUpperCase();
            let jantinaPenuh = rawJantina.startsWith('L') ? 'Lelaki' : (rawJantina.startsWith('P') ? 'Perempuan' : rawJantina);

            let pasanganNamaSheet = '-';
            let pasanganNoKpSheet = '-';
            let pasanganPtSheet = '-';

            const catatanIdx = headers.findIndex(h => h.includes('CATATAN') || h.includes('PENGESAHAN'));
            const startPartnerCol = pasanganColIdx !== -1 ? pasanganColIdx : (catatanIdx !== -1 ? catatanIdx + 1 : 20);

            for (let c = Math.max(0, startPartnerCol - 1); c < row.length; c++) {
              const cellVal = (row[c] || '').trim();
              if (!cellVal || cellVal === '-') continue;

              const digitsOnly = cellVal.replace(/[^0-9]/g, '');
              if (digitsOnly.length >= 11 && digitsOnly.length <= 12 && digitsOnly !== noKp && digitsOnly !== rawNoKp) {
                pasanganNoKpSheet = digitsOnly.padStart(12, '0');
                if (c > 0 && row[c - 1] && row[c - 1].trim() !== '' && isNaN(Number(row[c - 1].trim()))) {
                  pasanganNamaSheet = row[c - 1].trim();
                }
                if (c + 1 < row.length && row[c + 1] && row[c + 1].trim() !== '') {
                  pasanganPtSheet = row[c + 1].trim();
                }
                break;
              }
            }

            if (pasanganNamaSheet === '-' && pasanganColIdx !== -1 && row[pasanganColIdx]) {
              pasanganNamaSheet = row[pasanganColIdx].trim();
              if (row[pasanganColIdx + 2]) pasanganPtSheet = row[pasanganColIdx + 2].trim();
            }

            const hubunganJenis = getVal(['JENIS HUBUNGAN', 'HUBUNGAN']);
            const ptjValue = getVal(['TANGGUNGJAWAB', 'TANGUNGGJAWAB', 'PTJ', 'PUSAT']);

            const rawSejarah = getVal(['SEJARAH PERKHIDMATAN', 'SEJARAH PENEMPATAN', 'REKOD PENEMPATAN', 'SEJARAH']);
            const sejarahList = parseServiceHistoryList(rawSejarah, ptjValue, tarikhPTSemasa, tarikhLantikanStr);

            const rawApc = getVal(['ANUGERAH PERKHIDMATAN CEMERLANG', 'TAHUN APC', 'APC']);
            const apcYears = parseApcYearsList(rawApc);

            const rawSme = getVal(['DILANTIK SEBAGAI SME', 'PELANTIKAN SME', 'BIDANG SME', 'SME']);
            const smeInfo = parseSmeInfo(rawSme);

            return {
              id: index + 1,
              nama: nama,
              no_kp: noKp,
              no_pekerja: noPekerja,
              emel: getVal(['EMEL', 'EMAIL']),
              skim: rawSkim,
              ptj: ptjValue,
              negeri: getVal('NEGERI'),
              jantina: jantinaPenuh,
              bahagian: getVal(['BAHAGIAN', 'UNIT']),
              tarikh_lantikan: tarikhLantikanStr,
              tarikh_pt_sekarang: tarikhPTSemasa,
              tarikh_lahir: tarikhLahir,
              umur_bersara: getVal('UMUR BERSARA'),
              tarikh_bersara: tarikhBersara,
              tempoh_perkhidmatan: tempohKeseluruhan,
              tarikh_pengesahan: getVal('PENGESAHAN JAWATAN'),
              gambar: finalGambar,
              driveGambar: driveImageUrl,
              umurSemasa: umurSemasa,
              ageCohort: ageCohortStr,
              ptDurationYears: ptDurationYears,
              ptDurationStr: ptDurationStr,
              alertLevel: alertLevel,
              alertMsgs: alertMsgs,
              pasanganRef: pasanganNamaSheet,
              pasanganNoKp: pasanganNoKpSheet,
              pasanganPt: pasanganPtSheet,
              hubunganJenis: hubunganJenis,
              sejarahList,
              apcYears,
              isSme: smeInfo.isSme,
              smeBidang: smeInfo.bidang,
              totalServiceYears: Number(totalServiceFloat.toFixed(1)),
              bakiTahunBersara
            };
          }).filter(s => s.nama !== '-' && s.nama !== '');

          const normalizeName = (str) => (str || '')
            .toUpperCase()
            .replace(/\bBINTI\b|\bBT\.?\b/g, 'BT')
            .replace(/\bBIN\b|\bB\.?\b/g, 'B')
            .replace(/\bABDUL\b|\bABD\.?\b/g, 'ABD')
            .replace(/\bMOHAMAD\b|\bMUHAMMAD\b|\bMUHAMAD\b|\bMOHD\.?\b|\bMD\.?\b/g, 'MD')
            .replace(/[^A-Z0-9 ]/g, '')
            .replace(/\s+/g, ' ')
            .trim();

          const isKpMatch = (kp1, kp2) => {
            const c1 = (kp1 || '').replace(/[^0-9]/g, '');
            const c2 = (kp2 || '').replace(/[^0-9]/g, '');
            if (!c1 || !c2 || c1.length < 6 || c2.length < 6) return false;
            return c1 === c2 || c1.padStart(12, '0') === c2.padStart(12, '0') || (c1.slice(-6) === c2.slice(-6) && c1.slice(0, 6) === c2.slice(0, 6));
          };

          const isNameMatch = (n1, n2) => {
            const norm1 = normalizeName(n1);
            const norm2 = normalizeName(n2);
            if (!norm1 || !norm2 || norm1 === '-' || norm2 === '-') return false;
            return norm1 === norm2 || (norm1.length > 6 && norm2.includes(norm1)) || (norm2.length > 6 && norm1.includes(norm2));
          };

          const linkedData = mappedData.map(staff => ({
            ...staff,
            pasanganObj: null
          }));

          linkedData.forEach(staff => {
            const hasRef = (staff.pasanganNoKp && staff.pasanganNoKp !== '-') || (staff.pasanganRef && staff.pasanganRef !== '-');
            if (!hasRef) return;

            const matchedPartner = linkedData.find(other => 
              other.id !== staff.id && (
                isKpMatch(staff.pasanganNoKp, other.no_kp) ||
                isNameMatch(staff.pasanganRef, other.nama)
              )
            );

            if (matchedPartner) {
              staff.pasanganObj = matchedPartner;
              if (!matchedPartner.pasanganObj) {
                matchedPartner.pasanganObj = staff;
              }
            }
          });

          setStaffData(linkedData);
        }
        setIsLoadingCSV(false);
      } catch (error) {
        console.error("Gagal memuat turun data CSV:", error);
        setIsLoadingCSV(false);
      }
    };
    fetchGoogleSheetsData();
  }, []);

  const baseFilteredStaff = staffData.filter(s => {
    const qTrim = searchQuery.trim();
    const qLower = qTrim.toLowerCase();
    const qDigitsOnly = qTrim.replace(/[-\s]/g, '');
    const matchHiddenKp = qDigitsOnly.length > 0 && /^\d+$/.test(qDigitsOnly) && Boolean(s.no_kp && s.no_kp.includes(qDigitsOnly));
    const matchName =
      s.nama.toLowerCase().includes(qLower) ||
      s.no_pekerja.toLowerCase().includes(qLower) ||
      matchHiddenKp ||
      Boolean(s.smeBidang && s.smeBidang.toLowerCase().includes(qLower));
    const matchPtj = filterPtj === 'Semua' ? true : s.ptj === filterPtj;
    const matchSkim = filterSkim === 'Semua' ? true : s.skim.replace(/[0-9]/g, '').trim().toUpperCase() === filterSkim; 
    const matchRetiring = showRetiringOnly ? s.tarikh_bersara.includes('2027') : true;
    const minTahun = parseInt(filterTahunPT, 10);
    const matchTahunPT = filterTahunPT === '' || isNaN(minTahun) ? true : s.ptDurationYears >= minTahun;
    return matchName && matchPtj && matchSkim && matchRetiring && matchTahunPT;
  });

  const activeDataForCharts = baseFilteredStaff.filter(s => {
    return filterAgeCohort === 'Semua' ? true : s.ageCohort === filterAgeCohort;
  }).sort((a, b) => {
    const ptjA = a.ptj || '';
    const ptjB = b.ptj || '';
    const isPrnA = ptjA.toUpperCase().includes('PRN - PAHANG');
    const isPrnB = ptjB.toUpperCase().includes('PRN - PAHANG');
    
    if (isPrnA && !isPrnB) return -1;
    if (!isPrnA && isPrnB) return 1;
    if (ptjA < ptjB) return -1;
    if (ptjA > ptjB) return 1;
    
    const gredA = parseInt((a.skim || '').replace(/\D/g, ''), 10) || 0;
    const gredB = parseInt((b.skim || '').replace(/\D/g, ''), 10) || 0;
    
    if (gredA !== gredB) {
      return gredB - gredA; 
    }
    return (a.nama || '').localeCompare(b.nama || '');
  });

  const rawPtjList = [...new Set(staffData.map(s => s.ptj).filter(p => p && p !== '-'))].sort();
  const prnPtjMatch = rawPtjList.find(p => p.toUpperCase().includes('PRN - PAHANG'));
  const otherPtjList = rawPtjList.filter(p => p !== prnPtjMatch);
  
  const uniquePtj = ['Semua'];
  if (prnPtjMatch) uniquePtj.push(prnPtjMatch);
  uniquePtj.push(...otherPtjList);

  const allDetectedSkims = [...new Set(staffData.map(s => s.skim.replace(/[0-9]/g, '').trim().toUpperCase()).filter(s => s && s !== '-'))].sort();
  const uniqueSkim = ['Semua', ...allDetectedSkims];

  const totalStaff = activeDataForCharts.length;
  const maleStaff = activeDataForCharts.filter(s => s.jantina.toUpperCase().startsWith('L')).length;
  const femaleStaff = activeDataForCharts.filter(s => s.jantina.toUpperCase().startsWith('P')).length;
  const retiringSoon = activeDataForCharts.filter(s => s.tarikh_bersara.includes('2027')).length;
  const totalPtjCount = new Set(activeDataForCharts.map(s => s.ptj).filter(p => p && p !== '-')).size;

  const ptjDistribution = useMemo(() => {
    const counts = {};
    activeDataForCharts.forEach(s => {
      const ptjName = s.ptj && s.ptj !== '-' ? s.ptj.replace(/PEJABAT RISDA DAERAH|PEJABAT PRD -|PEJABAT/gi, '').trim() : 'Lain-lain';
      counts[ptjName] = (counts[ptjName] || 0) + 1;
    });
    return Object.entries(counts).map(([name, count]) => ({ name, count })).sort((a, b) => b.count - a.count);
  }, [activeDataForCharts]);

  const skimGroupDistribution = useMemo(() => {
    const counts = {};
    activeDataForCharts.forEach(s => {
      const group = (s.skim || '').replace(/[0-9]/g, '').trim().toUpperCase() || 'Lain-lain';
      if (group && group !== '-') counts[group] = (counts[group] || 0) + 1;
    });
    return Object.entries(counts).map(([group, count]) => ({ 
      group, count, percentage: totalStaff > 0 ? ((count / totalStaff) * 100).toFixed(1) : 0 
    })).sort((a, b) => b.count - a.count);
  }, [activeDataForCharts, totalStaff]);

  const ageDistribution = useMemo(() => {
    const cohorts = { 'Bawah 30 Thn': 0, '31 - 40 Thn': 0, '41 - 50 Thn': 0, '51 Thn Ke Atas': 0 };
    baseFilteredStaff.forEach(s => { if (cohorts[s.ageCohort] !== undefined) cohorts[s.ageCohort]++; });
    return cohorts;
  }, [baseFilteredStaff]);

  const handleExportCSV = () => {
    if (activeDataForCharts.length === 0) {
      setExportNotice("Tiada rekod untuk dieksport berdasarkan tapisan semasa.");
      setTimeout(() => setExportNotice(''), 3500);
      return;
    }
    const headers = ['Bil', 'Nama', 'No. Pekerja', 'Emel', 'Skim', 'Bahagian', 'Pusat Tanggungjawab', 'Tarikh Lantikan', 'Tempoh di PT Terkini', 'Tarikh Bersara', 'Sejarah Perkhidmatan', 'Tahun APC', 'Dilantik SME', 'Pasangan di RISDA', 'Amaran'];
    const rows = activeDataForCharts.map((s, idx) => {
      const namaPasangan = s.pasanganObj ? `${s.pasanganObj.nama} (${s.pasanganObj.no_pekerja})` : (s.pasanganRef !== '-' ? s.pasanganRef : '-');
      const sejarahText = s.sejarahList.map(item => `${item.tempoh}: ${item.tempat}`).join(' | ');
      const apcText = s.apcYears.length > 0 ? s.apcYears.join(', ') : '-';
      const smeText = s.isSme ? s.smeBidang : '-';
      return [
        idx + 1,
        `"${s.nama}"`,
        `="${s.no_pekerja}"`,
        `"${s.emel}"`,
        `"${s.skim}"`,
        `"${s.bahagian}"`,
        `"${s.ptj}"`,
        `"${s.tarikh_lantikan}"`,
        `"${s.ptDurationStr}"`,
        `"${s.tarikh_bersara}"`,
        `"${sejarahText}"`,
        `"${apcText}"`,
        `"${smeText}"`,
        `"${namaPasangan}"`,
        `"${s.alertMsgs.join(' | ')}"`
      ].join(',');
    });
    const csvString = [headers.join(','), ...rows].join('\n');
    const blob = new Blob(["\uFEFF" + csvString], { type: 'text/csv;charset=utf-8;' });
    const url = URL.createObjectURL(blob);
    const link = document.createElement("a");
    link.href = url;
    link.download = `Senarai_Kakitangan_RISDA_${new Date().toISOString().slice(0, 10).replace(/-/g, '')}.csv`;
    document.body.appendChild(link);
    link.click();
    document.body.removeChild(link);
  };

  const handlePrintProfile = (staff) => {
    if (!staff) return;
    const printWindow = window.open('', '_blank');
    if (!printWindow) return;
    const umurPaparan = staff.umurSemasa ? staff.umurSemasa + ' Tahun' : '-';

    const origin = window.location.origin;
    const defaultAvatarUrl = `https://ui-avatars.com/api/?name=${encodeURIComponent(staff.nama)}&background=1e3a8a&color=facc15&size=128&bold=true`;
    const modalAvatarEl = document.getElementById('modal-staff-photo');
    const currentModalSrc =
      modalAvatarEl && modalAvatarEl.src && !modalAvatarEl.src.includes('ui-avatars.com')
        ? modalAvatarEl.src
        : '';

    const fullLocalUrl = staff.gambar
      ? (staff.gambar.startsWith('/') ? `${origin}${staff.gambar}` : staff.gambar)
      : '';

    const driveIdMatch = (staff.driveGambar || '').match(/\/d\/([a-zA-Z0-9_-]+)/);
    const driveThumbUrl =
      driveIdMatch && driveIdMatch[1]
        ? `https://drive.google.com/thumbnail?id=${driveIdMatch[1]}&sz=w400`
        : '';

    const photoCandidates = [
      currentModalSrc,
      staff.driveGambar,
      driveThumbUrl,
      fullLocalUrl,
      defaultAvatarUrl
    ].filter((u, idx, arr) => Boolean(u) && arr.indexOf(u) === idx);
    
    const sejarahRowsHtml = (staff.sejarahList || []).map((item, idx) => `
      <tr>
        <td class="label">${idx + 1}. ${item.tempoh}</td>
        <td class="value">${item.tempat} ${item.isCurrent ? '<span style="color:#0d9488;">(Semasa)</span>' : ''}</td>
      </tr>
    `).join('');

    const apcText = staff.apcYears && staff.apcYears.length > 0
      ? staff.apcYears.map(y => `Tahun ${y}`).join(', ')
      : 'Tiada rekod direkodkan';

    const smeText = staff.isSme
      ? `Dilantik (${staff.smeBidang})`
      : 'Tidak Berkaitan';

    let pasanganHtml = '';
    if (staff.pasanganObj) {
      const isSamePtj = staff.ptj === staff.pasanganObj.ptj;
      pasanganHtml = `
        <div class="section-title">Maklumat Hubungan Keluarga / Pasangan (RISDA)</div>
        <table>
          <tr><td class="label">Nama Pasangan / Keluarga</td><td class="value">${staff.pasanganObj.nama} (No. Pekerja: ${staff.pasanganObj.no_pekerja})</td></tr>
          <tr><td class="label">Jawatan / Gred</td><td class="value">${staff.pasanganObj.bahagian} (${staff.pasanganObj.skim})</td></tr>
          <tr><td class="label">Pusat Tanggungjawab (PTJ)</td><td class="value" style="color: ${isSamePtj ? '#166534' : '#b45309'};">${staff.pasanganObj.ptj} (${isSamePtj ? 'Sama PTJ' : 'Berlainan PTJ'})</td></tr>
        </table>
      `;
    } else if (staff.pasanganRef && staff.pasanganRef !== '-') {
      pasanganHtml = `
        <div class="section-title">Maklumat Hubungan Keluarga / Pasangan (RISDA)</div>
        <table>
          <tr><td class="label">Rujukan Pasangan / Keluarga</td><td class="value">${staff.pasanganRef}</td></tr>
        </table>
      `;
    }
    
    const html = `
      <!DOCTYPE html>
      <html>
        <head>
          <title>Profil Kakitangan - ${staff.nama}</title>
          <style>
            body { font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif; padding: 40px; color: #333; line-height: 1.6; max-width: 800px; margin: 0 auto; -webkit-print-color-adjust: exact; print-color-adjust: exact; }
            .header { display: flex; align-items: center; border-bottom: 3px solid #1e3a8a; padding-bottom: 20px; margin-bottom: 30px; }
            .avatar { width: 120px; height: 120px; border-radius: 50%; object-fit: cover; margin-right: 25px; border: 4px solid #1e3a8a; background: #f8fafc; }
            .title h1 { margin: 0; color: #1e3a8a; font-size: 26px; text-transform: uppercase; font-weight: 900; }
            .title p { margin: 5px 0 0 0; color: #555; font-size: 14px; font-family: monospace; font-weight: bold; }
            .section-title { font-size: 15px; color: #1e3a8a; border-bottom: 2px solid #e5e7eb; padding-bottom: 5px; margin-top: 28px; margin-bottom: 12px; font-weight: 800; text-transform: uppercase; }
            table { width: 100%; border-collapse: collapse; margin-bottom: 16px; }
            td { padding: 8px 0; border-bottom: 1px dashed #e5e7eb; font-size: 13.5px; }
            .label { width: 40%; color: #6b7280; font-weight: bold; }
            .value { width: 60%; font-weight: bold; color: #111827; }
            .footer { margin-top: 50px; font-size: 11px; color: #9ca3af; text-align: center; border-top: 1px solid #f3f4f6; padding-top: 15px; font-style: italic; }
            .badge { display: inline-block; background: #e0e7ff; color: #3730a3; padding: 4px 10px; border-radius: 6px; font-size: 12px; font-weight: bold; border: 1px solid #c7d2fe; margin-top: 10px; }
          </style>
        </head>
        <body>
          <div class="header">
            <img id="print-avatar" class="avatar" referrerpolicy="no-referrer" alt="${staff.nama}" src="${photoCandidates[0]}" />
            <div class="title">
              <h1>${staff.nama}</h1>
              <p>NO. PEKERJA: ${staff.no_pekerja} &nbsp;|&nbsp; NO. KP: ${staff.no_kp}</p>
              <div class="badge">${staff.bahagian} (${staff.skim})</div>
            </div>
          </div>
          <div class="section-title">Maklumat Penempatan</div>
          <table>
            <tr><td class="label">Pusat Tanggungjawab (PTJ)</td><td class="value">${staff.ptj}</td></tr>
            <tr><td class="label">Negeri</td><td class="value">${staff.negeri}</td></tr>
            <tr><td class="label">Emel Rasmi</td><td class="value" style="color: #2563eb;">${staff.emel}</td></tr>
            <tr><td class="label">Jantina</td><td class="value">${staff.jantina}</td></tr>
          </table>
          <div class="section-title">Rekod Perkhidmatan & Persaraan</div>
          <table>
            <tr><td class="label">Tarikh Lantikan Pertama</td><td class="value">${staff.tarikh_lantikan}</td></tr>
            <tr><td class="label">Tarikh Pengesahan Jawatan</td><td class="value">${staff.tarikh_pengesahan}</td></tr>
            <tr><td class="label">Tarikh Penempatan (PT Semasa)</td><td class="value">${staff.tarikh_pt_sekarang}</td></tr>
            <tr><td class="label">Tempoh di PT Terkini</td><td class="value" style="color: #0d9488;">${staff.ptDurationStr}</td></tr>
            <tr><td class="label">Tempoh Perkhidmatan Keseluruhan</td><td className="value" style="color: #166534;">${staff.tempoh_perkhidmatan}</td></tr>
            <tr><td class="label">Tarikh Lahir / Umur Semasa</td><td class="value">${staff.tarikh_lahir} (${umurPaparan})</td></tr>
            <tr><td class="label" style="color: #991b1b;">Tarikh Kuatkuasa Bersara</td><td class="value" style="color: #991b1b;">${staff.tarikh_bersara} (${staff.umur_bersara} Tahun)</td></tr>
          </table>
          <div class="section-title">Sejarah Penempatan Perkhidmatan</div>
          <table>
            ${sejarahRowsHtml}
          </table>
          <div class="section-title">Pengiktirafan & Kepakaran (APC & SME)</div>
          <table>
            <tr><td class="label">Anugerah Perkhidmatan Cemerlang (APC)</td><td class="value" style="color: #b45309;">${apcText}</td></tr>
            <tr><td class="label">Pelantikan SME</td><td class="value" style="color: #4338ca;">${smeText}</td></tr>
          </table>
          ${pasanganHtml}
          <div class="footer">
            Dicetak melalui Portal Rasmi Pentadbiran RISDA Negeri Pahang pada ${new Date().toLocaleString('ms-MY')}. <br/>Dokumen ini dijana secara automatik.
          </div>
          <script>
            (function() {
              var candidates = ${JSON.stringify(photoCandidates)};
              var img = document.getElementById('print-avatar');
              var idx = 0;
              var printed = false;

              function triggerPrint() {
                if (printed) return;
                printed = true;
                setTimeout(function() { window.print(); }, 250);
              }

              function tryNext() {
                if (idx >= candidates.length) {
                  triggerPrint();
                  return;
                }
                img.src = candidates[idx++];
              }

              img.onload = function() {
                triggerPrint();
              };

              img.onerror = function() {
                tryNext();
              };

              setTimeout(triggerPrint, 3000);
              tryNext();
            })();
          </script>
        </body>
      </html>
    `;
    printWindow.document.open();
    printWindow.document.write(html);
    printWindow.document.close();
  };

  return (
    <div className="bg-transparent mb-12">
      <div className="mb-6 flex flex-col md:flex-row justify-between items-start md:items-center gap-4">
        <div>
          <h2 className="text-2xl font-bold text-blue-900">Dashboard Profiling Kakitangan</h2>
          <p className="text-gray-600">Analisis dan pengurusan maklumat tenaga kerja RISDA Negeri Pahang (Data Langsung).</p>
        </div>
        <button
          onClick={() => setShowAnalytics(!showAnalytics)}
          className="flex items-center px-4 py-2 bg-blue-100 hover:bg-blue-200 text-blue-900 text-sm font-semibold rounded-lg transition-colors shadow-sm"
        >
          <BarChart2 className="w-4 h-4 mr-2" />
          {showAnalytics ? 'Sembunyikan Analisis Visual' : 'Papar Analisis Visual'}
          {showAnalytics ? <ChevronUp className="w-4 h-4 ml-1.5" /> : <ChevronDown className="w-4 h-4 ml-1.5" />}
        </button>
      </div>

      {isLoadingCSV ? (
        <div className="flex flex-col items-center justify-center p-12 bg-white rounded-xl shadow-sm border border-gray-200">
           <div className="inline-block animate-spin rounded-full h-10 w-10 border-b-4 border-blue-900 mb-4"></div>
           <p className="text-gray-600 font-medium">Sedang memuat turun data kakitangan dari Google Sheets...</p>
        </div>
      ) : (
        <>
          <div className="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-4 mb-8">
            <div className="bg-white p-5 rounded-xl border-l-4 border-blue-600 shadow-sm flex items-center justify-between hover:shadow-md transition-all">
              <div>
                <p className="text-xs font-semibold text-gray-500">Jumlah Staf</p>
                <h3 className="text-3xl font-black text-gray-900 mt-0.5">{totalStaff}</h3>
              </div>
              <div className="p-3 bg-blue-50 text-blue-700 rounded-lg"><Users className="w-6 h-6" /></div>
            </div>
            <div className="bg-white p-5 rounded-xl border-l-4 border-indigo-500 shadow-sm flex items-center justify-between hover:shadow-md transition-all">
              <div>
                <p className="text-xs font-semibold text-gray-500">Lelaki / Wanita</p>
                <h3 className="text-xl font-black text-gray-900 mt-0.5">{maleStaff} <span className="text-gray-400 text-sm font-normal">/</span> {femaleStaff}</h3>
              </div>
              <div className="p-3 bg-indigo-50 text-indigo-700 rounded-lg"><User className="w-6 h-6" /></div>
            </div>
            <div 
              onClick={() => setShowRetiringOnly(!showRetiringOnly)}
              className={`p-5 rounded-xl border-l-4 border-rose-500 shadow-sm flex items-center justify-between hover:shadow-md transition-all cursor-pointer ${showRetiringOnly ? 'bg-rose-50 ring-2 ring-rose-400' : 'bg-white'}`}
            >
              <div>
                <p className="text-xs font-semibold text-gray-500">Bakal Bersara</p>
                <h3 className="text-3xl font-black text-gray-900 mt-0.5">{retiringSoon}</h3>
                <p className="text-[10px] text-rose-600 font-semibold mt-0.5">Klik tapis</p>
              </div>
              <div className="p-3 rounded-lg bg-rose-50 text-rose-600"><AlertTriangle className="w-6 h-6" /></div>
            </div>
            <div className="bg-white p-5 rounded-xl border-l-4 border-emerald-500 shadow-sm flex items-center justify-between hover:shadow-md transition-all">
              <div>
                <p className="text-xs font-semibold text-gray-500">PTJ Aktif</p>
                <h3 className="text-3xl font-black text-gray-900 mt-0.5">{totalPtjCount}</h3>
              </div>
              <div className="p-3 bg-emerald-50 text-emerald-700 rounded-lg"><Building className="w-6 h-6" /></div>
            </div>
          </div>

          {showAnalytics && (
            <div className="space-y-6 mb-8 animate-in fade-in duration-300">
              <div className="grid grid-cols-1 lg:grid-cols-3 gap-6">
                <div className="bg-white p-6 rounded-xl shadow-sm border border-gray-200 lg:col-span-2">
                  <div className="flex items-center justify-between mb-6 border-b pb-3">
                    <div className="flex items-center space-x-3">
                      <div className="p-2.5 bg-gradient-to-br from-blue-800 to-blue-600 text-white rounded-lg"><BarChart2 className="w-5 h-5" /></div>
                      <div>
                        <h3 className="font-black text-gray-900 text-lg">Bilangan Kakitangan mengikut Pusat Tanggungjawab</h3>
                        <p className="text-xs text-gray-500 font-medium mt-0.5">Kedudukan {ptjDistribution.length > 9 ? 9 : ptjDistribution.length} pusat tanggungjawab tertinggi</p>
                      </div>
                    </div>
                    <span className="text-xs font-bold bg-blue-50 text-blue-800 px-3 py-1 rounded-full border border-blue-200">{totalPtjCount} PTJ Aktif</span>
                  </div>
                  <div className="space-y-5">
                    {ptjDistribution.slice(0, 9).map((item, idx) => {
                      const percentage = ptjDistribution.length > 0 ? ((item.count / ptjDistribution[0].count) * 100).toFixed(0) : 0;
                      const globalPct = totalStaff > 0 ? ((item.count / totalStaff) * 100).toFixed(1) : 0;
                      return (
                        <div key={idx} className="relative group cursor-crosshair">
                          <div className="flex justify-between text-sm font-medium mb-1.5">
                            <span className="font-bold truncate text-gray-700 uppercase">{idx + 1}. {item.name}</span>
                            <span className="text-gray-900 font-black">{item.count} <span className="text-gray-500 text-xs font-medium">staf</span> <span className="text-gray-400 text-xs font-normal ml-1">({globalPct}%)</span></span>
                          </div>
                          <div className="w-full bg-gray-100 rounded-full h-3.5 flex items-center shadow-inner overflow-hidden">
                            <div className="h-full rounded-full bg-gradient-to-r from-blue-400 to-blue-600 transition-all duration-1000" style={{ width: `${percentage}%` }}></div>
                          </div>
                        </div>
                      );
                    })}
                  </div>
                </div>

                <div className="bg-white p-6 rounded-xl shadow-sm border border-gray-200 flex flex-col">
                  <div className="flex items-center space-x-3 mb-6 border-b pb-3">
                    <div className="p-2.5 bg-gradient-to-br from-yellow-500 to-yellow-400 text-yellow-900 rounded-lg"><PieChart className="w-5 h-5" /></div>
                    <div>
                        <h3 className="font-black text-gray-900 text-lg">Kategori Skim</h3>
                        <p className="text-xs text-gray-500 font-medium mt-0.5">Komposisi bidang tugas</p>
                    </div>
                  </div>
                  <div className="grid grid-cols-1 gap-3 mt-1 flex-grow">
                    {skimGroupDistribution.map((item, idx) => (
                      <div key={idx} className="relative overflow-hidden flex items-center justify-between p-3.5 rounded-xl border border-gray-100 bg-white shadow-sm hover:border-blue-200 transition-colors">
                        <div className="flex items-center space-x-3 z-10">
                          <div className={`w-10 h-10 rounded-full flex items-center justify-center font-black text-white shadow-sm ${idx === 0 ? 'bg-blue-600' : idx === 1 ? 'bg-indigo-500' : idx === 2 ? 'bg-yellow-500' : idx === 3 ? 'bg-emerald-500' : 'bg-purple-600'}`}>
                            {item.group.substring(0,2)}
                          </div>
                          <div>
                            <span className="font-extrabold text-sm text-gray-800 block">Skim {item.group}</span>
                            <span className="text-[10px] text-gray-400 font-bold uppercase tracking-wider">{
                                item.group === 'G' ? 'PERTANIAN' : item.group === 'N' ? 'PENTADBIRAN' : item.group === 'W' ? 'KEWANGAN' : item.group === 'H' ? 'TEKNIKAL' : 'LAIN-LAIN'
                            }</span>
                          </div>
                        </div>
                        <div className="text-right z-10 flex flex-col items-end">
                          <span className="font-black text-gray-900 text-lg">{item.count}</span>
                          <span className="text-[10px] font-bold text-gray-500">{item.percentage}%</span>
                        </div>
                      </div>
                    ))}
                  </div>
                </div>
              </div>

              <div className="bg-white p-6 rounded-xl shadow-sm border border-gray-200">
                <div className="flex items-center justify-between mb-4 border-b pb-3">
                  <div className="flex items-center space-x-2">
                    <div className="p-2 bg-green-50 text-green-700 rounded-lg"><TrendingUp className="w-5 h-5" /></div>
                    <div>
                      <h3 className="font-bold text-gray-900">Analisis Kohort Umur Tenaga Kerja</h3>
                      <p className="text-xs text-gray-500">Keseimbangan demografi generasi organisasi (Boleh diklik)</p>
                    </div>
                  </div>
                </div>

                <div className="grid grid-cols-2 md:grid-cols-4 gap-4">
                  {['Bawah 30 Thn', '31 - 40 Thn', '41 - 50 Thn', '51 Thn Ke Atas'].map((label, idx) => {
                    const count = ageDistribution[label] || 0;
                    const totalRef = baseFilteredStaff.length;
                    const pct = totalRef > 0 ? ((count / totalRef) * 100).toFixed(1) : 0;
                    const isSelected = filterAgeCohort === label;
                    return (
                      <div 
                        key={idx}
                        onClick={() => setFilterAgeCohort(isSelected ? 'Semua' : label)}
                        className={`relative p-5 rounded-xl cursor-pointer transition-all duration-300 shadow-sm border ${isSelected ? 'border-blue-400 bg-blue-50/50 ring-2 ring-blue-100 scale-[1.02]' : 'border-gray-100 bg-white hover:border-blue-200 hover:shadow-md'} flex flex-col items-center justify-center text-center`}
                      >
                        {isSelected && (
                          <div className="absolute top-2 right-2 flex items-center">
                            <span className="text-[10px] font-bold text-white bg-blue-500 px-2 py-0.5 rounded-full shadow-sm animate-pulse">Aktif</span>
                          </div>
                        )}
                        <p className={`text-xs font-bold uppercase tracking-wider mb-2 ${isSelected ? 'text-blue-700' : 'text-gray-500'}`}>{label}</p>
                        <h4 className={`text-3xl font-black mb-2 ${isSelected ? 'text-blue-900' : 'text-gray-800'}`}>{count} <span className="text-xs font-medium text-gray-500">staf</span></h4>
                        <div className="w-full bg-gray-200 rounded-full h-1.5 my-3 max-w-[80%]">
                          <div className={`h-1.5 rounded-full ${isSelected ? 'bg-blue-600' : 'bg-blue-500'}`} style={{ width: `${pct}%` }}></div>
                        </div>
                        <span className="text-xs font-bold text-gray-600">{pct}% jumlah</span>
                      </div>
                    );
                  })}
                </div>
              </div>
            </div>
          )}

          {exportNotice && (
            <div className="mb-4 p-3 bg-amber-50 border border-amber-200 text-amber-800 rounded-lg text-sm font-medium">
              {exportNotice}
            </div>
          )}

          <div className="bg-white p-4 rounded-xl shadow-sm border border-gray-200 mb-6 flex flex-col md:flex-row gap-4 items-center justify-between">
            <div className="relative w-full md:w-1/4">
              <Search className="absolute left-3 top-1/2 transform -translate-y-1/2 text-gray-400 w-5 h-5" />
              <input 
                type="text" 
                placeholder="Cari nama atau No. Pekerja..." 
                value={searchQuery}
                onChange={(e) => setSearchQuery(e.target.value)}
                className="w-full pl-10 pr-4 py-2.5 rounded-lg border border-gray-300 focus:ring-2 focus:ring-blue-900 outline-none text-sm"
              />
            </div>
            <div className="w-full md:w-3/4 flex flex-col sm:flex-row gap-3 items-center">
              <div className="w-full md:w-1/3 flex items-center">
                <Filter className="text-gray-400 w-4 h-4 mr-2 shrink-0" />
                <select value={filterPtj} onChange={(e) => setFilterPtj(e.target.value)} className="w-full py-2.5 px-3 rounded-lg border border-gray-300 focus:ring-2 focus:ring-blue-900 outline-none bg-white text-sm">
                  {uniquePtj.map(ptj => <option key={ptj} value={ptj}>{ptj === 'Semua' ? 'Semua PTJ' : ptj}</option>)}
                </select>
              </div>
              <div className="w-full md:w-1/4 flex items-center">
                <Briefcase className="text-gray-400 w-4 h-4 mr-2 shrink-0" />
                <select value={filterSkim} onChange={(e) => setFilterSkim(e.target.value)} className="w-full py-2.5 px-3 rounded-lg border border-gray-300 focus:ring-2 focus:ring-blue-900 outline-none bg-white text-sm">
                  {uniqueSkim.map(skim => <option key={skim} value={skim}>{skim === 'Semua' ? 'Semua Skim' : `Skim ${skim}`}</option>)}
                </select>
              </div>
              <div className="w-full md:w-1/4 flex items-center">
                <Clock className="text-gray-400 w-4 h-4 mr-2 shrink-0" />
                <input 
                  type="number" 
                  min="0"
                  placeholder="Min. Tahun di PT (Cth: 5)"
                  value={filterTahunPT} 
                  onChange={(e) => setFilterTahunPT(e.target.value)}
                  className="w-full py-2.5 px-3 rounded-lg border border-gray-300 focus:ring-2 focus:ring-blue-900 outline-none bg-white font-medium text-sm"
                />
              </div>
              <div className="flex gap-2 shrink-0">
                <button
                  onClick={handleExportCSV}
                  title="Eksport data ke Excel/CSV"
                  className="flex items-center justify-center px-4 py-2.5 rounded-lg text-xs font-bold border bg-green-50 text-green-700 hover:bg-green-100 border-green-200"
                >
                  <Download className="w-4 h-4 mr-1.5" /> Eksport CSV
                </button>
                <button
                  onClick={handleResetFilters}
                  className={`flex items-center justify-center px-4 py-2.5 rounded-lg text-xs font-semibold transition-all border ${isFiltered ? 'bg-red-50 text-red-600 border-red-200 hover:bg-red-100' : 'bg-gray-50 text-gray-500 border-gray-200 hover:bg-gray-100'}`}
                >
                  <RotateCcw className="w-4 h-4 mr-1.5" /> Set Semula
                </button>
              </div>
            </div>
          </div>

          <div className="bg-white rounded-xl shadow-sm border border-gray-200 overflow-hidden">
            <div className="overflow-x-auto max-h-[600px]">
              <table className="w-full text-left border-collapse">
                <thead className="sticky top-0 z-10 shadow-sm">
                  <tr className="bg-blue-50 text-blue-900 text-sm border-b border-gray-200">
                    <th className="p-4 font-semibold">Profil</th>
                    <th className="p-4 font-semibold">Nama & Pengiktirafan</th>
                    <th className="p-4 font-semibold">Jawatan / Gred</th>
                    <th className="p-4 font-semibold">Pusat Tanggungjawab</th>
                    <th className="p-4 font-semibold text-center">Tindakan</th>
                  </tr>
                </thead>
                <tbody className="divide-y divide-gray-100">
                  {activeDataForCharts.length > 0 ? activeDataForCharts.map((staff) => {
                    const isRed = staff.alertLevel === 'red';
                    const isYellow = staff.alertLevel === 'yellow';
                    const rowClass = isRed ? 'bg-red-50 hover:bg-red-100' : isYellow ? 'bg-yellow-50 hover:bg-yellow-100' : 'hover:bg-gray-50';

                    return (
                      <tr key={staff.id} className={`transition-colors ${rowClass}`}>
                        <td className="p-4 relative">
                          {staff.alertLevel !== 'none' && (
                            <div 
                              className={`absolute top-2 left-2 w-3 h-3 rounded-full animate-pulse shadow-sm border border-white ${isRed ? 'bg-red-500' : 'bg-yellow-500'}`} 
                              title={staff.alertMsgs.join(' | ')}
                            ></div>
                          )}
                          <img 
                            src={staff.gambar} 
                            alt={staff.nama} 
                            onError={(e) => {
                              if (staff.driveGambar && e.currentTarget.src !== staff.driveGambar) {
                                e.currentTarget.src = staff.driveGambar;
                              } else {
                                e.currentTarget.onerror = null;
                                e.currentTarget.src = `https://ui-avatars.com/api/?name=${encodeURIComponent(staff.nama)}&background=1e3a8a&color=facc15&size=128&bold=true`;
                              }
                            }}
                            className="w-12 h-12 rounded-full object-cover border-2 border-white shadow-sm bg-white" 
                          />
                        </td>
                        <td className="p-4">
                          <p className="font-bold text-gray-900 text-sm">{staff.nama}</p>
                          <p className="text-xs text-gray-500 font-mono mt-0.5">{staff.no_pekerja}</p>
                          <div className="flex flex-wrap items-center gap-1.5 mt-1.5">
                            {staff.apcYears.length > 0 && (
                              <span className="text-[10px] font-bold inline-flex items-center px-2 py-0.5 rounded-md bg-amber-100 text-amber-900 border border-amber-300">
                                <Award className="w-3 h-3 mr-1 text-amber-700" /> APC ({staff.apcYears.join(', ')})
                              </span>
                            )}
                            {staff.isSme && (
                              <span className="text-[10px] font-bold inline-flex items-center px-2 py-0.5 rounded-md bg-purple-100 text-purple-900 border border-purple-300">
                                <Star className="w-3 h-3 mr-1 text-purple-700" /> SME: {staff.smeBidang}
                              </span>
                            )}
                            {staff.alertLevel !== 'none' && (
                              <span className={`text-[11px] font-bold inline-block px-2.5 py-0.5 rounded shadow-sm border ${isRed ? 'bg-red-100 text-red-700 border-red-200' : 'bg-yellow-100 text-yellow-800 border-yellow-300'}`}>
                                {staff.alertMsgs[0]}
                              </span>
                            )}
                            {staff.pasanganObj ? (
                              <span 
                                onClick={() => setSelectedStaff(staff)}
                                className="text-[11px] font-bold inline-flex items-center gap-1.5 px-2.5 py-1 rounded-md shadow-sm border bg-indigo-50 hover:bg-indigo-100 text-indigo-900 border-indigo-200 cursor-pointer transition-colors" 
                                title={`Klik untuk lihat profil & pasangan (${staff.pasanganObj.nama})`}
                              >
                                <img 
                                  src={staff.pasanganObj.gambar} 
                                  alt={staff.pasanganObj.nama} 
                                  onError={(e) => {
                                    if (staff.pasanganObj.driveGambar && e.currentTarget.src !== staff.pasanganObj.driveGambar) {
                                      e.currentTarget.src = staff.pasanganObj.driveGambar;
                                    } else {
                                      e.currentTarget.onerror = null;
                                      e.currentTarget.src = `https://ui-avatars.com/api/?name=${encodeURIComponent(staff.pasanganObj.nama)}&background=581c87&color=facc15&size=64&bold=true`;
                                    }
                                  }}
                                  className="w-4 h-4 rounded-full object-cover border border-indigo-400 shrink-0"
                                />
                                <span>Pasangan RISDA: {staff.pasanganObj.nama} ({staff.pasanganObj.ptj})</span>
                              </span>
                            ) : (staff.pasanganRef && staff.pasanganRef !== '-') && (
                              <span 
                                onClick={() => setSelectedStaff(staff)}
                                className="text-[11px] font-bold inline-flex items-center gap-1.5 px-2.5 py-0.5 rounded-md shadow-sm border bg-indigo-50 hover:bg-indigo-100 text-indigo-800 border-indigo-200 cursor-pointer transition-colors"
                              >
                                <Users className="w-3.5 h-3.5 text-indigo-700 shrink-0" />
                                <span>Pasangan RISDA: {staff.pasanganRef} {staff.pasanganPt && staff.pasanganPt !== '-' ? `(${staff.pasanganPt})` : ''}</span>
                              </span>
                            )}
                          </div>
                        </td>
                        <td className="p-4">
                          <p className="text-sm text-gray-800 line-clamp-1">{staff.bahagian}</p>
                          <span className="inline-block px-2 py-0.5 mt-1 bg-blue-100 text-blue-800 text-xs font-bold rounded">{staff.skim}</span>
                        </td>
                        <td className="p-4 text-sm text-gray-600">{staff.ptj}</td>
                        <td className="p-4 text-center">
                          <button 
                            onClick={() => setSelectedStaff(staff)}
                            className="px-4 py-1.5 bg-blue-900 hover:bg-blue-800 text-white text-sm font-medium rounded-lg shadow-sm flex items-center justify-center mx-auto"
                          >
                            <Eye className="w-4 h-4 mr-1.5" /> Lihat
                          </button>
                        </td>
                      </tr>
                    );
                  }) : (
                    <tr>
                      <td colSpan="5" className="p-8 text-center text-gray-500">Tiada rekod kakitangan ditemui mengikut tapisan.</td>
                    </tr>
                  )}
                </tbody>
              </table>
            </div>
          </div>
        </>
      )}

      {selectedStaff && (
        <div className="fixed inset-0 z-50 flex items-center justify-center p-4 bg-slate-950/75 backdrop-blur-sm animate-in fade-in duration-200">
          <div className="bg-slate-50 rounded-2xl shadow-2xl w-full max-w-5xl max-h-[92vh] overflow-y-auto border border-slate-200 relative">
            <div className="sticky top-0 bg-gradient-to-r from-[#0f2354] via-[#1e3a8a] to-[#1d4ed8] text-white p-6 flex flex-col sm:flex-row justify-between items-start sm:items-center gap-4 z-20 rounded-t-2xl shadow-lg border-b-4 border-amber-400">
              <div className="flex items-center space-x-5">
                <div className="relative shrink-0">
                  <img 
                    id="modal-staff-photo"
                    referrerPolicy="no-referrer"
                    src={selectedStaff.gambar} 
                    alt={selectedStaff.nama} 
                    onError={(e) => {
                      if (selectedStaff.driveGambar && e.currentTarget.src !== selectedStaff.driveGambar) {
                        e.currentTarget.src = selectedStaff.driveGambar;
                      } else {
                        e.currentTarget.onerror = null;
                        e.currentTarget.src = `https://ui-avatars.com/api/?name=${encodeURIComponent(selectedStaff.nama)}&background=1e3a8a&color=facc15&size=128&bold=true`;
                      }
                    }}
                    className="w-20 h-20 sm:w-24 sm:h-24 rounded-2xl object-cover border-4 border-amber-400/90 shadow-xl bg-white" 
                  />
                  {selectedStaff.isSme && (
                    <span className="absolute -bottom-2 -right-2 bg-purple-700 text-amber-300 text-[10px] font-black px-2 py-0.5 rounded-full border-2 border-white shadow-md flex items-center">
                      <Star className="w-3 h-3 mr-0.5 fill-amber-300" /> SME
                    </span>
                  )}
                </div>
                <div>
                  <div className="flex flex-wrap items-center gap-2 mb-1">
                    <h2 className="text-xl sm:text-2xl font-black tracking-tight">{selectedStaff.nama}</h2>
                  </div>
                  <p className="text-blue-200 font-mono text-xs sm:text-sm mb-2.5">
                    No. Pekerja: <strong className="text-white">{selectedStaff.no_pekerja}</strong> &nbsp;•&nbsp; No. KP: <strong className="text-white">{selectedStaff.no_kp || '-'}</strong>
                  </p>
                  <div className="flex flex-wrap items-center gap-2">
                    <span className="bg-amber-400 text-blue-950 px-3 py-1 rounded-lg text-xs font-black shadow-sm">
                      {selectedStaff.bahagian} ({selectedStaff.skim})
                    </span>
                    {selectedStaff.apcYears.length > 0 && (
                      <span className="bg-white/15 backdrop-blur-sm text-amber-300 border border-amber-400/50 px-2.5 py-1 rounded-lg text-xs font-bold flex items-center">
                        <Award className="w-3.5 h-3.5 mr-1 text-amber-400" /> Penerima APC ({selectedStaff.apcYears.length}x)
                      </span>
                    )}
                  </div>
                </div>
              </div>
              <div className="flex items-center space-x-2 self-end sm:self-center">
                <button 
                  onClick={() => handlePrintProfile(selectedStaff)} 
                  className="flex items-center px-4 py-2 bg-amber-400 hover:bg-amber-300 text-blue-950 font-black rounded-xl transition-colors text-xs sm:text-sm shadow-md"
                >
                  <Printer className="w-4 h-4 mr-1.5" /> Cetak Profil
                </button>
                <button onClick={() => setSelectedStaff(null)} className="p-2 bg-blue-950/70 hover:bg-red-500 rounded-xl transition-colors text-white shadow-md">
                  <X className="w-5 h-5" />
                </button>
              </div>
            </div>

            <div className="px-6 pt-6 grid grid-cols-2 md:grid-cols-4 gap-3">
              <div className="bg-white p-3.5 rounded-xl border border-slate-200/80 shadow-sm">
                <span className="text-[10px] font-bold text-slate-400 uppercase block">Tempoh di PT Terkini</span>
                <span className="text-sm sm:text-base font-black text-teal-700 mt-0.5 block">{selectedStaff.ptDurationStr}</span>
              </div>
              <div className="bg-white p-3.5 rounded-xl border border-slate-200/80 shadow-sm">
                <span className="text-[10px] font-bold text-slate-400 uppercase block">Jumlah Perkhidmatan</span>
                <span className="text-sm sm:text-base font-black text-emerald-700 mt-0.5 block">{selectedStaff.tempoh_perkhidmatan}</span>
              </div>
              <div className="bg-white p-3.5 rounded-xl border border-slate-200/80 shadow-sm">
                <span className="text-[10px] font-bold text-slate-400 uppercase block">Umur Semasa ({new Date().getFullYear()})</span>
                <span className="text-sm sm:text-base font-black text-blue-900 mt-0.5 block">{selectedStaff.umurSemasa ? `${selectedStaff.umurSemasa} Tahun` : '-'}</span>
              </div>
              <div className="bg-white p-3.5 rounded-xl border border-slate-200/80 shadow-sm">
                <span className="text-[10px] font-bold text-slate-400 uppercase block">Kuatkuasa Bersara</span>
                <span className="text-sm sm:text-base font-black text-rose-700 mt-0.5 block">{selectedStaff.tarikh_bersara}</span>
              </div>
            </div>

            {(() => {
              const khidmatThn = selectedStaff.totalServiceYears || 0;
              const bakiThn = selectedStaff.bakiTahunBersara || 0;
              const jumlahKerjaya = Math.max(khidmatThn + bakiThn, 1);
              const pctKhidmat = Math.min(100, Math.round((khidmatThn / jumlahKerjaya) * 100));
              const ptSemasaThn = Number((selectedStaff.ptDurationYears || 0).toFixed(1));
              const ptTerdahuluThn = Math.max(0, Number((khidmatThn - ptSemasaThn).toFixed(1)));
              const pctHadPt = Math.min(100, Math.round((ptSemasaThn / 7) * 100));
              const bilPenempatan = selectedStaff.sejarahList ? selectedStaff.sejarahList.length : 1;
              const bilApc = selectedStaff.apcYears ? selectedStaff.apcYears.length : 0;

              const radius = 44;
              const circumference = 2 * Math.PI * radius;
              const strokeDashoffset = circumference - (pctKhidmat / 100) * circumference;

              const barMetrics = [
                {
                  label: 'Pengalaman Berkhidmat',
                  valueText: `${khidmatThn} Thn`,
                  pct: Math.min(100, Math.round((khidmatThn / 35) * 100)),
                  color: 'from-emerald-500 to-teal-500'
                },
                {
                  label: 'Pusingan Penempatan PT',
                  valueText: `${bilPenempatan} PTJ`,
                  pct: Math.min(100, bilPenempatan * 25),
                  color: 'from-blue-600 to-cyan-500'
                },
                {
                  label: 'Anugerah Cemerlang (APC)',
                  valueText: `${bilApc} Kali`,
                  pct: bilApc > 0 ? Math.min(100, bilApc * 35) : 6,
                  color: bilApc > 0 ? 'from-amber-500 to-yellow-400' : 'from-slate-300 to-slate-300'
                },
                {
                  label: 'Status Kepakaran SME',
                  valueText: selectedStaff.isSme ? 'Aktif (SME)' : 'Tiada',
                  pct: selectedStaff.isSme ? 100 : 8,
                  color: selectedStaff.isSme ? 'from-purple-600 to-indigo-500' : 'from-slate-300 to-slate-300'
                }
              ];

              return (
                <div className="px-6 pt-5">
                  <div className="bg-white p-5 rounded-2xl shadow-sm border border-slate-200">
                    <div className="flex flex-col sm:flex-row sm:items-center justify-between border-b border-slate-100 pb-3 mb-5 gap-2">
                      <h3 className="text-base font-black text-blue-950 flex items-center">
                        <BarChart2 className="w-5 h-5 mr-2 text-blue-700" /> Analisis Visual Kerjaya, Penempatan & Pencapaian
                      </h3>
                      <span className="text-[11px] font-bold bg-blue-50 text-blue-800 px-3 py-1 rounded-full border border-blue-200">
                        Ringkasan Graf Individu
                      </span>
                    </div>

                    <div className="grid grid-cols-1 md:grid-cols-3 gap-5">
                      <div className="bg-slate-50/80 p-4 rounded-xl border border-slate-200/80 flex flex-col items-center justify-between">
                        <div className="w-full flex items-center justify-between mb-2">
                          <span className="text-xs font-extrabold text-slate-700">Fasa Tempoh Kerjaya</span>
                          <PieChart className="w-4 h-4 text-emerald-600" />
                        </div>
                        <div className="relative w-32 h-32 flex items-center justify-center my-1">
                          <svg className="w-full h-full -rotate-90" viewBox="0 0 110 110">
                            <circle cx="55" cy="55" r={radius} stroke="#e2e8f0" strokeWidth="12" fill="none" />
                            <circle
                              cx="55"
                              cy="55"
                              r={radius}
                              stroke="#10b981"
                              strokeWidth="12"
                              strokeDasharray={circumference}
                              strokeDashoffset={strokeDashoffset}
                              strokeLinecap="round"
                              fill="none"
                              className="transition-all duration-700"
                            />
                          </svg>
                          <div className="absolute inset-0 flex flex-col items-center justify-center text-center">
                            <span className="text-xl font-black text-slate-900">{pctKhidmat}%</span>
                            <span className="text-[9px] font-bold text-slate-500 uppercase">Telah Dilalui</span>
                          </div>
                        </div>
                        <div className="w-full grid grid-cols-2 gap-2 mt-2 pt-2 border-t border-slate-200/80 text-center">
                          <div>
                            <span className="text-[10px] font-bold text-emerald-700 block">Berkhidmat</span>
                            <span className="text-xs font-black text-slate-900">{khidmatThn} Thn</span>
                          </div>
                          <div>
                            <span className="text-[10px] font-bold text-rose-600 block">Baki Bersara</span>
                            <span className="text-xs font-black text-slate-900">{bakiThn} Thn</span>
                          </div>
                        </div>
                      </div>

                      <div className="bg-slate-50/80 p-4 rounded-xl border border-slate-200/80 flex flex-col justify-between">
                        <div>
                          <div className="flex items-center justify-between mb-3">
                            <span className="text-xs font-extrabold text-slate-700">Analisis Tempoh PT</span>
                            <span className={`text-[10px] font-black px-2 py-0.5 rounded-full ${ptSemasaThn >= 7 ? 'bg-red-100 text-red-700' : ptSemasaThn >= 5 ? 'bg-amber-100 text-amber-800' : 'bg-teal-100 text-teal-800'}`}>
                              {ptSemasaThn >= 7 ? 'Melepasi 7 Thn' : 'Normal (<7 Thn)'}
                            </span>
                          </div>

                          <p className="text-[11px] font-semibold text-slate-500 mb-1.5">Nisbah PT Terkini vs PT Terdahulu</p>
                          <div className="w-full h-5 bg-slate-200 rounded-lg overflow-hidden flex shadow-inner mb-2">
                            <div
                              className="h-full bg-teal-600 flex items-center justify-center text-[10px] font-bold text-white transition-all duration-500"
                              style={{ width: `${khidmatThn > 0 ? Math.max(12, (ptSemasaThn / khidmatThn) * 100) : 100}%` }}
                              title={`PT Terkini: ${ptSemasaThn} Tahun`}
                            >
                              {ptSemasaThn}y
                            </div>
                            {ptTerdahuluThn > 0 && (
                              <div
                                className="h-full bg-indigo-500 flex items-center justify-center text-[10px] font-bold text-white transition-all duration-500"
                                style={{ width: `${(ptTerdahuluThn / khidmatThn) * 100}%` }}
                                title={`PT Terdahulu: ${ptTerdahuluThn} Tahun`}
                              >
                                {ptTerdahuluThn}y
                              </div>
                            )}
                          </div>
                          <div className="flex justify-between text-[10px] font-bold text-slate-500 mb-4">
                            <span className="flex items-center"><span className="w-2 h-2 rounded-full bg-teal-600 mr-1"></span>PT Terkini ({ptSemasaThn}y)</span>
                            <span className="flex items-center"><span className="w-2 h-2 rounded-full bg-indigo-500 mr-1"></span>Terdahulu ({ptTerdahuluThn}y)</span>
                          </div>

                          <div className="flex justify-between text-[11px] font-bold mb-1">
                            <span className="text-slate-600">Penanda Aras Stagnan (7 Thn)</span>
                            <span className={ptSemasaThn >= 7 ? 'text-red-600 font-black' : 'text-teal-700 font-black'}>{pctHadPt}%</span>
                          </div>
                          <div className="w-full h-3 bg-slate-200 rounded-full overflow-hidden">
                            <div
                              className={`h-full rounded-full transition-all duration-700 ${ptSemasaThn >= 7 ? 'bg-gradient-to-r from-red-500 to-rose-600' : ptSemasaThn >= 5 ? 'bg-gradient-to-r from-amber-400 to-orange-500' : 'bg-gradient-to-r from-teal-500 to-emerald-500'}`}
                              style={{ width: `${pctHadPt}%` }}
                            ></div>
                          </div>
                        </div>

                        <p className="text-[10px] text-slate-500 mt-3 pt-2 border-t border-slate-200/80">
                          Penempatan semasa: <strong className="text-slate-700">{selectedStaff.ptDurationStr}</strong> daripada had pemantauan 7 tahun.
                        </p>
                      </div>

                      <div className="bg-slate-50/80 p-4 rounded-xl border border-slate-200/80 flex flex-col justify-between">
                        <div className="flex items-center justify-between mb-2.5">
                          <span className="text-xs font-extrabold text-slate-700">Graf Indeks Profil & Bakat</span>
                          <TrendingUp className="w-4 h-4 text-blue-700" />
                        </div>
                        <div className="space-y-3 my-auto">
                          {barMetrics.map((m, idx) => (
                            <div key={idx}>
                              <div className="flex justify-between text-[11px] font-bold mb-1">
                                <span className="text-slate-600">{m.label}</span>
                                <span className="text-slate-900 font-black">{m.valueText}</span>
                              </div>
                              <div className="w-full h-2.5 bg-slate-200 rounded-full overflow-hidden">
                                <div
                                  className={`h-full bg-gradient-to-r ${m.color} rounded-full transition-all duration-700`}
                                  style={{ width: `${m.pct}%` }}
                                ></div>
                              </div>
                            </div>
                          ))}
                        </div>
                      </div>

                    </div>
                  </div>
                </div>
              );
            })()}

            <div className="p-6 grid grid-cols-1 lg:grid-cols-12 gap-6">
              <div className="lg:col-span-7 space-y-6">
                <div className="bg-white p-5 rounded-2xl shadow-sm border border-slate-200">
                  <h3 className="text-base font-black text-blue-950 mb-4 flex items-center border-b border-slate-100 pb-2.5">
                    <User className="w-5 h-5 mr-2 text-blue-700" /> Maklumat Penempatan Semasa
                  </h3>
                  <div className="grid grid-cols-1 sm:grid-cols-3 gap-4 text-sm">
                    <div className="bg-slate-50 p-3 rounded-xl border border-slate-100">
                      <p className="text-[11px] font-bold text-slate-400 uppercase mb-0.5">Emel Rasmi</p>
                      <p className="font-bold text-blue-700 truncate" title={selectedStaff.emel}>{selectedStaff.emel}</p>
                    </div>
                    <div className="bg-slate-50 p-3 rounded-xl border border-slate-100">
                      <p className="text-[11px] font-bold text-slate-400 uppercase mb-0.5">Jantina</p>
                      <p className="font-bold text-slate-900">{selectedStaff.jantina}</p>
                    </div>
                    <div className="bg-slate-50 p-3 rounded-xl border border-slate-100">
                      <p className="text-[11px] font-bold text-slate-400 uppercase mb-0.5">Negeri</p>
                      <p className="font-bold text-slate-900">{selectedStaff.negeri}</p>
                    </div>
                    <div className="sm:col-span-3 bg-gradient-to-r from-blue-50 to-indigo-50 p-3.5 rounded-xl border border-blue-200 flex items-center justify-between">
                      <div>
                        <p className="text-blue-700 text-[11px] font-extrabold uppercase tracking-wider">Pusat Tanggungjawab (PTJ) Terkini</p>
                        <p className="font-black text-blue-950 text-base mt-0.5">{selectedStaff.ptj}</p>
                      </div>
                      <Building className="w-7 h-7 text-blue-700/40 shrink-0" />
                    </div>
                  </div>
                </div>

                <div className="bg-white p-5 rounded-2xl shadow-sm border border-slate-200">
                  <div className="flex items-center justify-between border-b border-slate-100 pb-2.5 mb-4">
                    <h3 className="text-base font-black text-blue-950 flex items-center">
                      <History className="w-5 h-5 mr-2 text-teal-600" /> Sejarah Perkhidmatan & Penempatan
                    </h3>
                    <span className="text-[11px] font-bold bg-teal-50 text-teal-800 px-2.5 py-0.5 rounded-full border border-teal-200">
                      Sejak {selectedStaff.tarikh_lantikan}
                    </span>
                  </div>

                  {selectedStaff.sejarahList && selectedStaff.sejarahList.length > 0 ? (
                    <div className="relative pl-6 space-y-4 before:content-[''] before:absolute before:left-[9px] before:top-2 before:bottom-2 before:w-0.5 before:bg-gradient-to-b before:from-blue-400 before:via-teal-400 before:to-emerald-500">
                      {selectedStaff.sejarahList.map((item, idx) => (
                        <div key={idx} className="relative">
                          <span className={`absolute -left-6 top-1.5 w-4 h-4 rounded-full border-2 border-white shadow-sm ${item.isCurrent ? 'bg-emerald-500 ring-4 ring-emerald-100' : 'bg-blue-700'}`}></span>
                          <div className={`p-3 rounded-xl border transition-all ${item.isCurrent ? 'bg-emerald-50/70 border-emerald-200' : 'bg-slate-50 border-slate-200/70'}`}>
                            <div className="flex flex-wrap items-center justify-between gap-1">
                              <span className={`text-[11px] font-mono font-extrabold px-2 py-0.5 rounded ${item.isCurrent ? 'bg-emerald-600 text-white' : 'bg-blue-100 text-blue-900'}`}>
                                {item.tempoh}
                              </span>
                              {item.isCurrent && (
                                <span className="text-[10px] font-black text-emerald-700 uppercase tracking-wider">Penempatan Terkini</span>
                              )}
                            </div>
                            <p className="text-sm font-bold text-slate-900 mt-1.5">{item.tempat}</p>
                          </div>
                        </div>
                      ))}
                    </div>
                  ) : (
                    <p className="text-xs text-slate-500 italic bg-slate-50 p-4 rounded-xl border border-dashed border-slate-200">
                      Tiada catatan sejarah penempatan terdahulu direkodkan.
                    </p>
                  )}
                </div>

                <div className="bg-white p-5 rounded-2xl shadow-sm border border-slate-200">
                  <div className="flex flex-col sm:flex-row sm:items-center justify-between border-b border-slate-100 pb-2.5 mb-4 gap-2">
                    <h3 className="text-base font-black text-blue-950 flex items-center">
                      <Users className="w-5 h-5 mr-2 text-indigo-600" /> Maklumat Hubungan Keluarga / Pasangan
                    </h3>
                    {selectedStaff.hubunganJenis && selectedStaff.hubunganJenis !== '-' && (
                      <span className="text-xs font-bold bg-indigo-100 text-indigo-800 px-3 py-0.5 rounded-full border border-indigo-200">
                        Hubungan: {selectedStaff.hubunganJenis}
                      </span>
                    )}
                  </div>

                  {selectedStaff.pasanganObj ? (
                    <div className="bg-gradient-to-r from-indigo-50/80 to-blue-50/60 p-4 rounded-xl border border-indigo-200 flex flex-col sm:flex-row items-start sm:items-center justify-between gap-4">
                      <div className="flex items-center space-x-3.5">
                        <img 
                          src={selectedStaff.pasanganObj.gambar} 
                          alt={selectedStaff.pasanganObj.nama} 
                          onError={(e) => {
                            if (selectedStaff.pasanganObj.driveGambar && e.currentTarget.src !== selectedStaff.pasanganObj.driveGambar) {
                              e.currentTarget.src = selectedStaff.pasanganObj.driveGambar;
                            } else {
                              e.currentTarget.onerror = null;
                              e.currentTarget.src = `https://ui-avatars.com/api/?name=${encodeURIComponent(selectedStaff.pasanganObj.nama)}&background=581c87&color=facc15&size=128&bold=true`;
                            }
                          }}
                          className="w-14 h-14 rounded-full object-cover border-2 border-indigo-400 shadow-sm bg-white shrink-0" 
                        />
                        <div>
                          <h4 className="font-bold text-slate-900 text-sm">{selectedStaff.pasanganObj.nama}</h4>
                          <p className="text-xs text-slate-600 font-medium mt-0.5">
                            {selectedStaff.pasanganObj.bahagian} <span className="font-bold text-blue-800">({selectedStaff.pasanganObj.skim})</span>
                          </p>
                          <div className="flex flex-wrap items-center gap-1.5 mt-1.5">
                            <span className="text-[11px] font-bold text-blue-900 bg-white px-2 py-0.5 rounded border border-blue-200">
                              {selectedStaff.pasanganObj.ptj}
                            </span>
                            {selectedStaff.ptj === selectedStaff.pasanganObj.ptj ? (
                              <span className="text-[10px] font-bold text-green-700 bg-green-100 px-2 py-0.5 rounded border border-green-200">
                                ✓ Sama PTJ
                              </span>
                            ) : (
                              <span className="text-[10px] font-bold text-amber-800 bg-amber-100 px-2 py-0.5 rounded border border-amber-300">
                                ⚠ Berlainan PTJ
                              </span>
                            )}
                          </div>
                        </div>
                      </div>

                      <button
                        onClick={() => setSelectedStaff(selectedStaff.pasanganObj)}
                        className="px-3.5 py-2 bg-indigo-700 hover:bg-indigo-800 text-white text-xs font-bold rounded-lg shadow-sm flex items-center shrink-0 transition-colors"
                      >
                        <Eye className="w-3.5 h-3.5 mr-1.5" /> Lihat Profil
                      </button>
                    </div>
                  ) : selectedStaff.pasanganRef && selectedStaff.pasanganRef !== '-' ? (
                    <div className="bg-amber-50 p-3.5 rounded-xl border border-amber-200">
                      <p className="text-xs font-bold text-amber-800 uppercase mb-1">Rujukan Pasangan / Keluarga Direkodkan</p>
                      <p className="text-sm font-bold text-slate-900">{selectedStaff.pasanganRef}</p>
                      <div className="flex flex-wrap gap-2 mt-1.5 text-xs text-slate-700">
                        {selectedStaff.pasanganNoKp && selectedStaff.pasanganNoKp !== '-' && (
                          <span className="bg-white px-2 py-0.5 rounded border border-amber-200 font-mono">No. KP: {selectedStaff.pasanganNoKp}</span>
                        )}
                        {selectedStaff.pasanganPt && selectedStaff.pasanganPt !== '-' && (
                          <span className="bg-white px-2 py-0.5 rounded border border-amber-200 font-bold text-blue-900">PT: {selectedStaff.pasanganPt}</span>
                        )}
                      </div>
                    </div>
                  ) : (
                    <div className="bg-slate-50 p-3.5 rounded-xl border border-dashed border-slate-300 text-center">
                      <p className="text-xs text-slate-500">Tiada rekod pasangan atau ahli keluarga di RISDA didaftarkan.</p>
                    </div>
                  )}
                </div>
              </div>

              <div className="lg:col-span-5 space-y-6">
                <div className="bg-gradient-to-br from-amber-50 via-yellow-50/70 to-white p-5 rounded-2xl shadow-sm border border-amber-200">
                  <div className="flex items-center justify-between border-b border-amber-200/70 pb-2.5 mb-4">
                    <h3 className="text-base font-black text-amber-950 flex items-center">
                      <Award className="w-5 h-5 mr-2 text-amber-600" /> Anugerah Perkhidmatan Cemerlang (APC)
                    </h3>
                    {selectedStaff.apcYears.length > 0 && (
                      <span className="text-xs font-black bg-amber-500 text-white px-2.5 py-0.5 rounded-full shadow-sm">
                        {selectedStaff.apcYears.length} Kali
                      </span>
                    )}
                  </div>

                  {selectedStaff.apcYears.length > 0 ? (
                    <div className="space-y-3">
                      <p className="text-xs text-amber-900/80 font-medium">
                        Diiktiraf atas kecemerlangan prestasi perkhidmatan pada tahun berikut:
                      </p>
                      <div className="flex flex-wrap gap-2.5">
                        {selectedStaff.apcYears.map((tahun, idx) => (
                          <div
                            key={idx}
                            className="flex items-center gap-2 bg-white px-3.5 py-2 rounded-xl border-2 border-amber-400 shadow-sm"
                          >
                            <Award className="w-4 h-4 text-amber-500 shrink-0" />
                            <div>
                              <span className="text-[10px] font-bold text-amber-700 uppercase block leading-none">Penerima APC</span>
                              <span className="text-sm font-black text-slate-900">Tahun {tahun}</span>
                            </div>
                          </div>
                        ))}
                      </div>
                    </div>
                  ) : (
                    <div className="bg-white/80 p-4 rounded-xl border border-dashed border-amber-300 text-center">
                      <p className="text-xs font-semibold text-slate-600">Tiada rekod penerima APC dicatatkan.</p>
                      <p className="text-[11px] text-slate-400 mt-1">Isi tahun di lajur <strong>TAHUN APC</strong> pada Google Sheets.</p>
                    </div>
                  )}
                </div>

                <div className="bg-gradient-to-br from-purple-50 via-indigo-50/60 to-white p-5 rounded-2xl shadow-sm border border-purple-200">
                  <div className="flex items-center justify-between border-b border-purple-200/70 pb-2.5 mb-4">
                    <h3 className="text-base font-black text-purple-950 flex items-center">
                      <Star className="w-5 h-5 mr-2 text-purple-600" /> Pelantikan SME
                    </h3>
                    <span className={`text-[11px] font-black px-2.5 py-0.5 rounded-full ${selectedStaff.isSme ? 'bg-purple-700 text-amber-300' : 'bg-slate-200 text-slate-600'}`}>
                      {selectedStaff.isSme ? 'DILANTIK' : 'TIADA'}
                    </span>
                  </div>

                  {selectedStaff.isSme ? (
                    <div className="bg-white p-4 rounded-xl border border-purple-200 shadow-sm flex items-start gap-3">
                      <div className="p-2.5 bg-purple-100 text-purple-700 rounded-xl shrink-0">
                        <Sparkles className="w-5 h-5" />
                      </div>
                      <div>
                        <span className="text-[10px] font-extrabold text-purple-600 uppercase tracking-wider block">
                          Bidang Kepakaran Rujukan (Subject Matter Expert)
                        </span>
                        <p className="text-sm font-black text-slate-900 mt-1">{selectedStaff.smeBidang}</p>
                      </div>
                    </div>
                  ) : (
                    <div className="bg-white/80 p-4 rounded-xl border border-dashed border-purple-200 text-center">
                      <p className="text-xs font-semibold text-slate-600">Belum dilantik sebagai Pakar Rujuk (SME).</p>
                      <p className="text-[11px] text-slate-400 mt-1">Isi bidang kepakaran di lajur <strong>DILANTIK SEBAGAI SME</strong> pada Google Sheets.</p>
                    </div>
                  )}
                </div>

                <div className="bg-white p-5 rounded-2xl shadow-sm border border-slate-200">
                  <h3 className="text-base font-black text-blue-950 mb-4 flex items-center border-b border-slate-100 pb-2.5">
                    <Briefcase className="w-5 h-5 mr-2 text-blue-700" /> Tarikh Penting Perkhidmatan & Persaraan
                  </h3>
                  <ul className="space-y-2.5 text-sm">
                    <li className="flex justify-between border-b border-slate-100 pb-2">
                      <span className="text-slate-500">Lantikan Pertama</span>
                      <span className="font-bold text-slate-900">{selectedStaff.tarikh_lantikan}</span>
                    </li>
                    <li className="flex justify-between border-b border-slate-100 pb-2">
                      <span className="text-slate-500">Pengesahan Jawatan</span>
                      <span className="font-bold text-slate-900">{selectedStaff.tarikh_pengesahan}</span>
                    </li>
                    <li className="flex justify-between border-b border-slate-100 pb-2">
                      <span className="text-slate-500">Penempatan PT Semasa</span>
                      <span className="font-bold text-slate-900">{selectedStaff.tarikh_pt_sekarang}</span>
                    </li>
                    <li className="flex justify-between border-b border-slate-100 pb-2">
                      <span className="text-slate-500">Tarikh Lahir</span>
                      <span className="font-bold text-slate-900">{selectedStaff.tarikh_lahir}</span>
                    </li>
                    <li className="flex justify-between border-b border-slate-100 pb-2">
                      <span className="text-slate-500">Umur Pilihan Bersara</span>
                      <span className="font-bold text-slate-900">{selectedStaff.umur_bersara} Tahun</span>
                    </li>
                    <li className="flex justify-between items-center pt-1 mt-2 bg-rose-50 p-3 rounded-xl border border-rose-200">
                      <span className="text-rose-800 font-bold text-xs flex items-center"><Clock className="w-4 h-4 mr-1.5" /> Kuatkuasa Bersara</span>
                      <span className="font-black text-rose-800">{selectedStaff.tarikh_bersara}</span>
                    </li>
                  </ul>
                </div>
              </div>
            </div>
          </div>
        </div>
      )}
    </div>
  );
};

export default function App() {
  const ANNOUNCEMENT_STORAGE_KEY = 'risda_pahang_announcements_v1';
  const SUPER_ADMIN_ANNOUNCEMENT_IC = '880518115127';

  const normalizeIcId = (val) => String(val || '').replace(/[^a-zA-Z0-9]/g, '').trim();

  const defaultInitialAnnouncements = [
    {
      id: 'init-ann-1',
      title: 'Selamat Datang ke Portal Rasmi Pentadbiran RISDA Negeri Pahang',
      category: 'Makluman Rasmi',
      content: 'Portal interaktif ini memaparkan maklumat direktori, lokasi Pusat Tanggungjawab (PTJ), serta papan pemuka analitik sumber manusia secara langsung.',
      linkUrl: '',
      timestamp: Date.now(),
      author: 'Pentadbiran RISDA Pahang'
    }
  ];

  const [user, setUser] = useState(null);
  const [currentPage, setCurrentPage] = useState('home');
  const [isMobileMenuOpen, setIsMobileMenuOpen] = useState(false);
  const [homeSubTab, setHomeSubTab] = useState('info');
  const [lokasiTab, setLokasiTab] = useState('daerah');
  const [filterStesenDaerah, setFilterStesenDaerah] = useState('Semua');
  const [stesenList, setStesenList] = useState([]);
  const [isLoadingStesen, setIsLoadingStesen] = useState(true);

  useEffect(() => {
    let isMounted = true;
    const defaultPahangStesen = [
      { nama: 'PEJABAT RISDA STESEN BATU PAPAN', daerah: 'PRD BERA', alamat: 'JALAN KUALA TRIANG, KG BATU PAPAN, 28300 BERA, PAHANG', tel: '09-2554807' },
      { nama: 'PEJABAT RISDA STESEN KERAYONG', daerah: 'PRD BERA', alamat: 'NO. 21, RUMAH KEDAI, JALAN JATI, TAMAN JATI, 28200 TRIANG, PAHANG', tel: '09-2553952' },
      { nama: 'PEJABAT RISDA STESEN LANCHANG', daerah: 'PRD TEMERLOH', alamat: 'NO. 56 JALAN TENGKU AMPUAN AFZAN 1, 28500 LANCHANG PAHANG', tel: '09-2803050' },
      { nama: 'PEJABAT RISDA STESEN KUALA KRAU', daerah: 'PRD TEMERLOH', alamat: 'NO. 12, JALAN BESAR KUALA KRAU, 28050 KUALA KRAU, PAHANG', tel: '09-2862422' },
      { nama: 'PEJABAT RISDA STESEN TEMERLOH', daerah: 'PRD TEMERLOH', alamat: 'NO. 30, JALAN SUNGAI RABIT, 28000 TEMERLOH, PAHANG', tel: '09-2962100' },
      { nama: 'PEJABAT RISDA STESEN CHEROH', daerah: 'PRD RAUB', alamat: 'TAMAN BINTANG CHEROH, 27600 RAUB, PAHANG', tel: '09-3697506' },
      { nama: 'PEJABAT RISDA STESEN GALI', daerah: 'PRD RAUB', alamat: 'KAMPUNG ULU GALI, 27500 SUNGAI RUAN, RAUB, PAHANG', tel: '09-3657335' },
      { nama: 'PEJABAT RISDA STESEN SEGA', daerah: 'PRD RAUB', alamat: 'KAMPUNG JERUAS, 27620 SEGA, PAHANG', tel: '09-3657571' },
      { nama: 'PEJABAT RISDA STESEN DAMAK', daerah: 'PRD JERANTUT', alamat: 'NO. 1, PUSAT PERTUMBUHAN DESA (PPD) DAMAK 2B, 27030 JERANTUT, PAHANG', tel: '09-2691288' },
      { nama: 'PEJABAT RISDA STESEN PEDAH / TEBING TINGGI', daerah: 'PRD JERANTUT', alamat: 'KAMPUNG TEBING TINGGI, 27040 JERANTUT, PAHANG', tel: '09-2663511' },
      { nama: 'PEJABAT RISDA STESEN BENTA', daerah: 'PRD LIPIS', alamat: 'JALAN BESAR BENTA, 27300 BENTA, PAHANG', tel: '09-3238233' },
      { nama: 'PEJABAT RISDA STESEN MERAPOH', daerah: 'PRD LIPIS', alamat: 'BANDAR BARU MERAPOH, 27210 KUALA LIPIS, PAHANG', tel: '09-9121233' },
      { nama: 'PEJABAT RISDA STESEN SUNGAI KOYAN', daerah: 'PRD LIPIS', alamat: 'PUSAT PENEMPATAN SUNGAI KOYAN, 27650 RAUB, PAHANG', tel: '09-3401233' },
      { nama: 'PEJABAT RISDA STESEN CHENOR', daerah: 'PRD MARAN', alamat: 'BANDAR CHENOR, 28100 CHENOR, PAHANG', tel: '09-2991233' },
      { nama: 'PEJABAT RISDA STESEN SRI JAYA', daerah: 'PRD MARAN', alamat: 'BANDAR SRI JAYA, 26500 MARAN, PAHANG', tel: '09-4772233' },
      { nama: 'PEJABAT RISDA STESEN GAMBANG', daerah: 'PRD PAHANG TIMUR', alamat: 'BANDAR GAMBANG, 26300 KUANTAN, PAHANG', tel: '09-5491233' },
      { nama: 'PEJABAT RISDA STESEN PANCHING', daerah: 'PRD PAHANG TIMUR', alamat: 'JALAN PANCHING, 25150 KUANTAN, PAHANG', tel: '09-5391233' },
      { nama: 'PEJABAT RISDA STESEN PEKAN', daerah: 'PRD PAHANG TIMUR', alamat: 'JALAN SULTAN AHMAD, 26600 PEKAN, PAHANG', tel: '09-4221233' },
      { nama: 'PEJABAT RISDA STESEN MUADZAM SHAH', daerah: 'PRD PAHANG TIMUR', alamat: 'BANDAR MUADZAM SHAH, 26700 MUADZAM SHAH, PAHANG', tel: '09-4522233' },
      { nama: 'PEJABAT RISDA STESEN KARAK', daerah: 'PRD BENTONG', alamat: 'JALAN BESAR KARAK, 28600 KARAK, PAHANG', tel: '09-2311233' },
      { nama: 'PEJABAT RISDA MINI STESEN LURAH BILUT', daerah: 'PRD BENTONG', alamat: 'FELDA LURAH BILUT, 28800 BENTONG, PAHANG', tel: '09-2331233' },
      { nama: 'PEJABAT RISDA MINI STESEN LEPAR HILIR', daerah: 'PRD PAHANG TIMUR', alamat: 'KAMPUNG LEPAR HILIR, 26300 KUANTAN, PAHANG', tel: '09-5492233' },
      { nama: 'PEJABAT RISDA MINI STESEN PADANG PIOL', daerah: 'PRD JERANTUT', alamat: 'KAMPUNG PADANG PIOL, 27000 JERANTUT, PAHANG', tel: '09-2664233' }
    ];

    const fetchStesenData = async () => {
      setIsLoadingStesen(true);
      try {
        let parsedRows = [];
        try {
          parsedRows = await fetchSheetViaJSONP(STAFF_SHEET_ID, '1');
        } catch (e) {
          parsedRows = [];
        }

        if (!parsedRows || parsedRows.length <= 1) {
          const urlsToTry = [
            `https://docs.google.com/spreadsheets/d/${STAFF_SHEET_ID}/gviz/tq?tqx=out:csv&gid=1&t=${Date.now()}`,
            `https://docs.google.com/spreadsheets/d/${STAFF_SHEET_ID}/export?format=csv&gid=1&t=${Date.now()}`,
            `${FALLBACK_PUBLISHED_CSV_URL.replace('gid=0', 'gid=1')}&t=${Date.now()}`
          ];
          for (const url of urlsToTry) {
            try {
              const res = await fetch(url);
              if (res.ok) {
                const text = await res.text();
                if (text && !text.trim().startsWith('<!DOCTYPE')) {
                  const csvParsed = parseCSV(text);
                  if (csvParsed && csvParsed.length > 1) {
                    parsedRows = csvParsed;
                    break;
                  }
                }
              }
            } catch (err) {
              // Cuba URL seterusnya
            }
          }
        }

        if (isMounted && parsedRows && parsedRows.length > 1) {
          const headers = parsedRows[0].map(h => String(h || '').trim().toUpperCase());
          const hasStesenCols = headers.some(h => h.includes('STESEN') || h.includes('DAERAH') || h.includes('ALAMAT') || h.includes('TEL'));

          if (hasStesenCols) {
            const mappedStesen = parsedRows.slice(1).map((row) => {
              const getField = (keys) => {
                const arr = Array.isArray(keys) ? keys : [keys];
                for (const k of arr) {
                  const idx = headers.findIndex(h => h.includes(k));
                  if (idx !== -1 && row[idx]) return String(row[idx]).trim();
                }
                return '';
              };

              const nama = getField(['NAMA STESEN', 'NAMA PEJABAT', 'STESEN', 'PEJABAT', 'NAMA']);
              const daerah = getField(['DAERAH', 'PT', 'PUSAT TANGGUNGJAWAB', 'PRD']);
              const alamat = getField(['ALAMAT', 'LOKASI']);
              const tel = getField(['TEL', 'TELEFON', 'NO TEL', 'PHONE']);

              return {
                nama: nama || '',
                daerah: daerah || 'Negeri Pahang',
                alamat: alamat || '-',
                tel: tel || '-'
              };
            }).filter(item => item.nama && item.nama !== '-' && (item.nama.toUpperCase().includes('STESEN') || item.nama.toUpperCase().includes('PRS') || item.nama.toUpperCase().includes('PRMS')));

            if (mappedStesen.length > 0) {
              setStesenList(mappedStesen);
              return;
            }
          }
        }

        if (isMounted) {
          setStesenList(defaultPahangStesen);
        }
      } catch (err) {
        if (isMounted) {
          setStesenList(defaultPahangStesen);
        }
      } finally {
        if (isMounted) setIsLoadingStesen(false);
      }
    };

    fetchStesenData();
    return () => {
      isMounted = false;
    };
  }, []);
  
  const [mtrZoom, setMtrZoom] = useState(1);
  const [mtrPan, setMtrPan] = useState({ x: 0, y: 0 });
  const [isPanningMtr, setIsPanningMtr] = useState(false);
  const mtrPanStartRef = useRef({ x: 0, y: 0 });
  const mtrViewerRef = useRef(null);
  const [mtrTab, setMtrTab] = useState('teras');
  const [posterLoadError, setPosterLoadError] = useState(false);

  const posterSources = [
    '/poster-mtr-2030.jpg',
    '/poster-mtr-2030.png',
    'https://drive.google.com/thumbnail?id=1bHujA0hvyOjVm0le0gs9GZonBoYKsksY&sz=w1600'
  ];
  const [posterSourceIdx, setPosterSourceIdx] = useState(0);
  const [buildingImgIdx, setBuildingImgIdx] = useState(0);

  const buildingSources = [
    BANGUNAN_PRN_PRIMARY_URL,
    BANGUNAN_PRN_URL,
    BANGUNAN_PRN_ALT_URL,
    `https://drive.google.com/thumbnail?id=${BANGUNAN_PRN_DRIVE_ID}&sz=w1200`,
    `https://lh3.googleusercontent.com/d/${BANGUNAN_PRN_DRIVE_ID}`,
    `https://drive.usercontent.google.com/download?id=${BANGUNAN_PRN_DRIVE_ID}&export=view`
  ];
  const buildingLoadFailed = buildingImgIdx >= buildingSources.length;

  useEffect(() => {
    if (currentPage !== 'profil') return;
    const viewerEl = mtrViewerRef.current;
    if (!viewerEl) return;

    // Pasang pendengar wheel secara non-passive supaya scroll dalam gambar tidak menggerakkan halaman utama
    const handleNativeWheel = (e) => {
      if (posterLoadError) return;
      e.preventDefault();
      e.stopPropagation();

      setMtrZoom((prev) => {
        const nextZoom = e.deltaY < 0
          ? Math.min(4.0, Number((prev + 0.2).toFixed(1)))
          : Math.max(0.8, Number((prev - 0.2).toFixed(1)));
        if (nextZoom <= 1) {
          setMtrPan({ x: 0, y: 0 });
        }
        return nextZoom;
      });
    };

    viewerEl.addEventListener('wheel', handleNativeWheel, { passive: false });
    return () => {
      viewerEl.removeEventListener('wheel', handleNativeWheel);
    };
  }, [currentPage, posterLoadError]);
  const [editingAnnId, setEditingAnnId] = useState(null);
  const [announcementFeedback, setAnnouncementFeedback] = useState('');
  const [isSubmitting, setIsSubmitting] = useState(false);
  const [adminTab, setAdminTab] = useState('utama');
  const [isAdminLoggedIn, setIsAdminLoggedIn] = useState(false);
  const [loggedInUser, setLoggedInUser] = useState(null);
  const [allowedUsers, setAllowedUsers] = useState([]);
  const [icInput, setIcInput] = useState('');
  const [passwordInput, setPasswordInput] = useState('');
  const [showPassword, setShowPassword] = useState(false);
  const [loginError, setLoginError] = useState('');
  const [announcements, setAnnouncements] = useState(() => {
    try {
      const saved = localStorage.getItem(ANNOUNCEMENT_STORAGE_KEY);
      if (saved) {
        const parsed = JSON.parse(saved);
        if (Array.isArray(parsed) && parsed.length > 0) return parsed;
      }
    } catch (e) {}
    return defaultInitialAnnouncements;
  });
  const [newTitle, setNewTitle] = useState('');
  const [newCategory, setNewCategory] = useState('Makluman Rasmi');
  const [newContent, setNewContent] = useState('');
  const [newLinkUrl, setNewLinkUrl] = useState('');
  const [annSearchQuery, setAnnSearchQuery] = useState('');
  const [annPage, setAnnPage] = useState(1);
  const [selectedAnnouncement, setSelectedAnnouncement] = useState(null);
  const [isLoadingData, setIsLoadingData] = useState(true);

  const canManageAnnouncements = Boolean(
    isAdminLoggedIn &&
    loggedInUser &&
    normalizeIcId(loggedInUser.username) === SUPER_ADMIN_ANNOUNCEMENT_IC
  );

  const defaultAuthorizedUsers = [
    { username: '671109025015', password: '084561', nama: 'ABDUL AZIZ BIN AWANG' },
    { username: '880518115127', password: '123', nama: 'MOHD REDZUAN BIN ABD RASHID' },
    { username: '840803065687', password: '089668', nama: 'MUHAMAD ABBAS BIN MOHD ALI' }
  ];

  useEffect(() => {
    const fetchAllowedUsers = async () => {
      try {
        const res = await fetch(`https://docs.google.com/spreadsheets/d/1bPoG6HPjkBzuIetcwJWGFAINPOaemHXh4DmuPm-o7bk/export?format=csv`);
        const parsed = parseCSV(await res.text());
        if (parsed.length > 1) {
          const headers = parsed[0].map(h => h.trim().toUpperCase());
          const uIdx = headers.findIndex(h => h.includes('USERNAME') || h.includes('NO KP'));
          const pIdx = headers.findIndex(h => h.includes('PASSWORD'));
          const nIdx = headers.findIndex(h => h.includes('NAMA'));
          const validUsers = parsed.slice(1).map(row => ({
            username: uIdx !== -1 && row[uIdx] ? row[uIdx].trim() : '',
            password: pIdx !== -1 && row[pIdx] ? row[pIdx].trim() : '',
            nama: nIdx !== -1 && row[nIdx] ? row[nIdx].trim() : ''
          })).filter(u => u.username !== '');
          if (validUsers.length > 0) setAllowedUsers(validUsers);
          else setAllowedUsers(defaultAuthorizedUsers);
        } else setAllowedUsers(defaultAuthorizedUsers);
      } catch (err) {
        setAllowedUsers(defaultAuthorizedUsers);
      }
    };
    fetchAllowedUsers();
  }, []);

  const saveAnnouncementsToStorage = (list) => {
    setAnnouncements(list);
    try {
      localStorage.setItem(ANNOUNCEMENT_STORAGE_KEY, JSON.stringify(list));
    } catch (e) {}
  };

  useEffect(() => {
    if (!auth) return;
    const initAuth = async () => {
      try {
        await signInAnonymously(auth);
      } catch (error) {
        console.warn("Firebase Auth off:", error);
      }
    };
    initAuth();
    const unsubscribe = onAuthStateChanged(auth, (usr) => setUser(usr));
    return () => unsubscribe();
  }, []);

  useEffect(() => {
    if (!user || !db || firebaseConfig.apiKey === "demo-api-key") {
      setIsLoadingData(false);
      return;
    }
    setIsLoadingData(true);
    try {
      const announcementsRef = collection(db, 'artifacts', appId, 'public', 'data', 'announcements');
      const unsubscribe = onSnapshot(announcementsRef, (snapshot) => {
        const fetched = snapshot.docs.map(docSnap => ({ id: docSnap.id, ...docSnap.data() }));
        fetched.sort((a, b) => b.timestamp - a.timestamp);
        if (fetched.length > 0) {
          saveAnnouncementsToStorage(fetched);
        }
        setIsLoadingData(false);
      }, () => {
        setIsLoadingData(false);
      });
      return () => unsubscribe();
    } catch (err) {
      setIsLoadingData(false);
    }
  }, [user]);

  const navigateTo = (page) => {
    setCurrentPage(page);
    setIsMobileMenuOpen(false);
    window.scrollTo(0, 0);
  };

  const handleLogin = (e) => {
    e.preventDefault();
    const activeUsersList = allowedUsers.length > 0 ? allowedUsers : defaultAuthorizedUsers;
    const inputClean = normalizeIcId(icInput);
    const matchedUser = activeUsersList.find(
      u => normalizeIcId(u.username) === inputClean && String(u.password).trim() === passwordInput.trim()
    );
    if (matchedUser) {
      setIsAdminLoggedIn(true);
      setLoggedInUser(matchedUser);
      setLoginError('');
      setIcInput('');
      setPasswordInput('');
      setShowPassword(false);
    } else {
      setLoginError('ID Pengguna atau Kata Laluan tidak sah. Hanya pengguna berdaftar dibenarkan.');
    }
  };

  const handleLogout = () => {
    setIsAdminLoggedIn(false);
    setLoggedInUser(null);
    setEditingAnnId(null);
    navigateTo('home');
  };

  const handlePostAnnouncement = async (e) => {
    e.preventDefault();
    if (!canManageAnnouncements) return;
    if (!newTitle.trim() || !newContent.trim()) return;

    setIsSubmitting(true);
    const nowTs = Date.now();
    const authorName = loggedInUser?.nama || 'Pentadbir Utama Portal';

    try {
      if (editingAnnId) {
        const updatedList = announcements.map(item =>
          item.id === editingAnnId
            ? { ...item, title: newTitle.trim(), category: newCategory, content: newContent.trim(), linkUrl: newLinkUrl.trim(), timestamp: nowTs, author: authorName }
            : item
        );
        saveAnnouncementsToStorage(updatedList);
        setEditingAnnId(null);
        setAnnouncementFeedback('Pengumuman telah berjaya dikemas kini dan dipaparkan di Laman Utama!');
      } else {
        const newEntry = {
          id: 'ann-' + nowTs,
          title: newTitle.trim(),
          category: newCategory,
          content: newContent.trim(),
          linkUrl: newLinkUrl.trim(),
          timestamp: nowTs,
          author: authorName
        };
        const updatedList = [newEntry, ...announcements];
        saveAnnouncementsToStorage(updatedList);

        if (user && db && firebaseConfig.apiKey !== "demo-api-key") {
          try {
            await addDoc(collection(db, 'artifacts', appId, 'public', 'data', 'announcements'), {
              title: newEntry.title,
              category: newEntry.category,
              content: newEntry.content,
              linkUrl: newEntry.linkUrl,
              timestamp: newEntry.timestamp,
              author: newEntry.author
            });
          } catch (err) {}
        }
        setAnnouncementFeedback('Pengumuman baharu berjaya diterbitkan terus ke Laman Utama Portal!');
      }

      setNewTitle('');
      setNewContent('');
      setNewLinkUrl('');
      setNewCategory('Makluman Rasmi');
      setAnnPage(1);
      setTimeout(() => setAnnouncementFeedback(''), 4500);
    } finally {
      setIsSubmitting(false);
    }
  };

  const handleStartEditAnnouncement = (ann) => {
    if (!canManageAnnouncements) return;
    setEditingAnnId(ann.id);
    setNewTitle(ann.title || '');
    setNewCategory(ann.category || 'Makluman Rasmi');
    setNewContent(ann.content || '');
    setNewLinkUrl(ann.linkUrl || '');
  };

  const handleDeleteAnnouncement = async (annId) => {
    if (!canManageAnnouncements) return;
    const filteredList = announcements.filter(item => item.id !== annId);
    saveAnnouncementsToStorage(filteredList);
    if (editingAnnId === annId) {
      setEditingAnnId(null);
      setNewTitle('');
      setNewContent('');
      setNewLinkUrl('');
    }
    if (user && db && firebaseConfig.apiKey !== "demo-api-key") {
      try {
        await deleteDoc(doc(db, 'artifacts', appId, 'public', 'data', 'announcements', annId));
      } catch (err) {}
    }
    setAnnouncementFeedback('Pengumuman telah dipadamkan daripada Laman Utama.');
    setTimeout(() => setAnnouncementFeedback(''), 3500);
  };

  const directoryData = [
    { name: "Encik Abdul Aziz bin Awang", role: "Pengarah RISDA Negeri", extension: "111", email: "abdaziz@risda.gov.my", department: "Pejabat Pengarah" },
    { name: "Encik Muhammad Abbas bin Mohd Ali", role: "Timbalan Pengarah RISDA Negeri", extension: "113", email: "abbas@risda.gov.my", department: "Unit Tanam Semula dan Bekalan" },
    { name: "Encik Mohd Redzuan bin Abd Rashid", role: "Pegawai Tadbir Negeri", extension: "114", email: "mohdredzuan@risda.gov.my", department: "Unit Pentadbiran, Kewangan, Integriti dan Kejuteraan" },
    { name: "Puan Wan Kamariah binti Wan Muhammad", role: "Ketua Unit", extension: "140", email: "wkamariah@risda.gov.my", department: "Unit Pengembangan, Produktiviti dan Pemasaran" },
    { name: "Puan Syuhaida binti Syukor", role: "Ketua Unit", extension: "145", email: "syuhaida@risda.gov.my", department: "Unit Perancangan, Pembangunan Usahawan, Agromakanan dan Program Khas" }
  ];

  const formatDate = (timestamp) => new Date(timestamp).toLocaleDateString('ms-MY', { year: 'numeric', month: 'long', day: 'numeric', hour: '2-digit', minute: '2-digit' });

  const formatShortMalayDate = (timestamp) => {
    const monthsShort = ['Jan', 'Feb', 'Mac', 'Apr', 'Mei', 'Jun', 'Jul', 'Ogo', 'Sep', 'Okt', 'Nov', 'Dis'];
    const d = new Date(timestamp);
    if (isNaN(d.getTime())) return '-';
    const day = String(d.getDate()).padStart(2, '0');
    return `${day} ${monthsShort[d.getMonth()]} ${d.getFullYear()}`;
  };

  const mtrData = [
    {
      id: 1, teras: "TERAS 1", tajuk: "Pemerkasaan Pengeluaran Getah Negara", warna: "from-blue-900 to-blue-700", borderWarna: "border-blue-500", impak: "Pengeluaran Getah Capai 1 Juta Tan Metrik",
      fokus: ["Pengeluaran Getah Negara", "Tanam Semula Getah", "Prasarana Asas"],
      strategi: ["Meningkatkan Pengeluaran Getah Negara", "Pembangunan Kawasan Tanam Getah", "Penyediaan Kemudahan Asas Tanaman Getah", "Peningkatan Keupayaan Pasukan Kerja"]
    },
    {
      id: 2, teras: "TERAS 2", tajuk: "Kemakmuran Pekebun Kecil", warna: "from-amber-700 to-amber-600", borderWarna: "border-amber-500", impak: "Purata Pendapatan RM4,500 Sebulan",
      fokus: ["Pendapatan Pekebun Kecil", "Kemahiran Modal Insan", "Kesejahteraan Sosial"],
      strategi: ["Pengukuhan Teknik Berkelompok", "Pemerkasaan Aktiviti Agromakanan", "Peningkatan Projek Pembangunan", "Akses Pendidikan Berkualiti", "Pengupayaan Modal Insan", "Perlindungan Takaful Maksimum"]
    },
    {
      id: 3, teras: "TERAS 3", tajuk: "Pengukuhan Keterlihatan Dan Sinergi", warna: "from-yellow-600 to-yellow-500", borderWarna: "border-yellow-400", impak: "Keterlihatan Kumpulan RISDA Dalam Industri",
      fokus: ["Persepsi Umum", "Kerjasama Strategik"],
      strategi: ["Kepelbagaian Liputan Media RISDA", "Memartabatkan Maslahah Ummah Melalui Pelbagai Agensi"]
    },
    {
      id: 4, teras: "TERAS 4", tajuk: "Penguasaan Rantaian Bekalan", warna: "from-emerald-800 to-emerald-700", borderWarna: "border-emerald-500", impak: "Keuntungan KRH Mencapai RM500 Juta",
      fokus: ["Pendapatan Kumpulan", "Perniagaan Getah Kumpulan"],
      strategi: ["Meneroka Pasaran Baharu & Mengembangkan Perniagaan Getah", "Pendedahan Dalam Pembuatan Getah"]
    },
    {
      id: 5, teras: "TERAS 5", tajuk: "Organisasi Berprestasi Tinggi", warna: "from-amber-600 to-amber-500", borderWarna: "border-amber-400", impak: "RISDA Agensi Berprestasi Tinggi",
      fokus: ["Tataskelola dan Akauntabiliti", "Budaya Kerja Berprestasi", "Reformasi Prosedur", "Transformasi Digital"],
      strategi: ["Amalan Pembudayaan Nilai Tatakelola Baik", "Pelaksanaan Penilaian Prestasi", "Laksana Reformasi Prosedur", "Menyokong Pemerkasaan Data", "Mengoptimumkan Modal Insan", "Transformasi Digital"]
    }
  ];

  const renderHome = () => {
    const ANN_PER_PAGE = 10;
    const qAnn = annSearchQuery.trim().toLowerCase();
    const filteredAnnouncements = announcements.filter((ann) => {
      if (!qAnn) return true;
      return (
        (ann.title || '').toLowerCase().includes(qAnn) ||
        (ann.content || '').toLowerCase().includes(qAnn) ||
        (ann.category || '').toLowerCase().includes(qAnn) ||
        formatShortMalayDate(ann.timestamp).toLowerCase().includes(qAnn)
      );
    });

    const totalArticles = filteredAnnouncements.length;
    const totalPages = Math.max(1, Math.ceil(totalArticles / ANN_PER_PAGE));
    const currentSafePage = Math.min(annPage, totalPages);
    const startIndex = (currentSafePage - 1) * ANN_PER_PAGE;
    const paginatedAnnouncements = filteredAnnouncements.slice(startIndex, startIndex + ANN_PER_PAGE);
    const showingFrom = totalArticles === 0 ? 0 : startIndex + 1;
    const showingTo = Math.min(startIndex + ANN_PER_PAGE, totalArticles);

    const getPageNumbers = () => {
      const pages = [];
      if (totalPages <= 6) {
        for (let i = 1; i <= totalPages; i++) pages.push(i);
      } else {
        pages.push(1, 2, 3, 4, 5, '...', totalPages);
      }
      return pages;
    };

    return (
      <div className="flex flex-col md:flex-row min-h-[calc(100vh-80px)] w-full animate-in fade-in duration-500">
        <aside className="w-full md:w-64 lg:w-72 bg-white border-b md:border-b-0 md:border-r border-gray-200 shrink-0 flex flex-col">
          <div className="p-5 border-b border-gray-100 bg-slate-50/80">
            <span className="text-[11px] font-black uppercase tracking-widest text-blue-900 block">
              Menu Laman Utama
            </span>
            <p className="text-xs text-gray-500 mt-1">
              Pilih paparan informasi atau analisis awam
            </p>
          </div>
          <div className="p-3 space-y-2">
            <button
              type="button"
              onClick={() => setHomeSubTab('info')}
              className={`w-full flex items-center px-4 py-3 rounded-xl font-bold text-sm transition-all text-left ${
                homeSubTab === 'info'
                  ? 'bg-blue-900 text-yellow-400 shadow-md'
                  : 'text-gray-700 hover:bg-blue-50 hover:text-blue-900'
              }`}
            >
              <Home className="w-5 h-5 mr-3 shrink-0" />
              <span>Informasi & Pengumuman</span>
            </button>
            <button
              type="button"
              onClick={() => setHomeSubTab('statistik')}
              className={`w-full flex items-center px-4 py-3 rounded-xl font-bold text-sm transition-all text-left ${
                homeSubTab === 'statistik'
                  ? 'bg-blue-900 text-yellow-400 shadow-md'
                  : 'text-gray-700 hover:bg-blue-50 hover:text-blue-900'
              }`}
            >
              <BarChart2 className="w-5 h-5 mr-3 shrink-0" />
              <span>Statistik & Analisis Awam</span>
            </button>
          </div>
        </aside>

        <div className="flex-1 min-w-0 p-4 sm:p-6 lg:p-8">
          {homeSubTab === 'info' ? (
            <div className="space-y-8 animate-in fade-in duration-300">
              <div className="relative bg-blue-900 text-white overflow-hidden rounded-xl shadow-2xl">
                <div className="absolute inset-0 opacity-20 bg-[url('https://www.transparenttextures.com/patterns/cubes.png')]"></div>
                <div className="relative z-10 px-8 py-14 md:py-20 flex flex-col items-center text-center">
                  <div className="flex items-center justify-center gap-6 md:gap-10 mb-6 flex-wrap">
                    <RisdaDriveLogo className="h-28 md:h-36 max-w-[160px] md:max-w-[200px] hover:scale-105" showGlow={false} isSecond={true} />
                    <div className="hidden sm:block h-20 w-px bg-blue-700/60"></div>
                    <RisdaDriveLogo className="h-28 md:h-36 max-w-[240px] md:max-w-[300px] hover:scale-105" showGlow={true} isSecond={false} />
                  </div>
                  <h1 className="text-3xl md:text-5xl font-bold mb-4 tracking-tight">PENTADBIRAN RISDA PAHANG</h1>
                  <p className="text-lg md:text-xl max-w-2xl text-blue-100 mb-8">Memacu kemajuan pekebun kecil getah ke arah kehidupan yang lebih sejahtera dan berpendapatan tinggi.</p>
                  <button 
                    onClick={() => navigateTo('lokasi')}
                    className="bg-yellow-500 hover:bg-yellow-400 text-blue-900 font-semibold py-3 px-8 rounded-full shadow-lg transition-transform transform hover:scale-105 flex items-center"
                  >
                    Kenali Kami <ChevronRight className="ml-2 w-5 h-5" />
                  </button>
                </div>
              </div>

              <div className="grid grid-cols-1 md:grid-cols-3 gap-6">
                <div className="bg-white p-6 rounded-xl shadow-sm border border-gray-100 flex flex-col items-center text-center">
                  <div className="bg-blue-100 p-4 rounded-full mb-4 text-blue-700"><Users className="w-8 h-8" /></div>
                  <h3 className="text-xl font-semibold mb-2">Pekebun Kecil</h3>
                  <p className="text-gray-600">Menyokong 47,464 pekebun kecil di seluruh negeri Pahang.</p>
                </div>
                <div className="bg-white p-6 rounded-xl shadow-sm border border-gray-100 flex flex-col items-center text-center">
                  <div className="bg-blue-100 p-4 rounded-full mb-4 text-blue-700"><Building className="w-8 h-8" /></div>
                  <h3 className="text-xl font-semibold mb-2">Pusat Tanggungjawab</h3>
                  <p className="text-gray-600">8 Pejabat RISDA Daerah, 20 Pejabat RISDA Stesen & 3 Pejabat Mini Stesen sedia membantu.</p>
                </div>
                <div className="bg-white p-6 rounded-xl shadow-sm border border-gray-100 flex flex-col items-center text-center">
                  <div className="bg-blue-100 p-4 rounded-full mb-4 text-blue-700"><Bell className="w-8 h-8" /></div>
                  <h3 className="text-xl font-semibold mb-2">Bantuan & Subsidi</h3>
                  <p className="text-gray-600">Menyalurkan pelbagai inisiatif, bantuan tanam semula dan input pertanian terkini.</p>
                </div>
              </div>

              <style>
                {'@keyframes risdaTickerMove { 0% { transform: translateX(0%); } 100% { transform: translateX(-50%); } } .risda-ticker-track { display: flex; width: max-content; animation: risdaTickerMove 30s linear infinite; } .risda-ticker-wrap:hover .risda-ticker-track { animation-play-state: paused; }'}
              </style>

              <div className="bg-white rounded-xl shadow-md border border-gray-200 overflow-hidden">
                {announcements.length > 0 && (
                  <div className="bg-gradient-to-r from-blue-950 via-blue-900 to-blue-950 text-white flex items-center border-b border-amber-400/60 overflow-hidden">
                    <div className="bg-amber-400 text-blue-950 px-4 py-2 font-black text-[11px] uppercase tracking-wider flex items-center shrink-0 z-10 shadow-sm">
                      <span className="w-2 h-2 rounded-full bg-rose-600 animate-ping mr-2"></span>
                      <Volume2 className="w-3.5 h-3.5 mr-1.5" />
                      Terkini
                    </div>
                    <div className="risda-ticker-wrap flex-1 overflow-hidden py-2 relative">
                      <div className="risda-ticker-track items-center">
                        {[0, 1].map((dupIdx) => (
                          <div key={dupIdx} className="flex items-center shrink-0">
                            {announcements.map((ann, idx) => (
                              <button
                                key={`${dupIdx}-${ann.id}-${idx}`}
                                type="button"
                                onClick={() => setSelectedAnnouncement(ann)}
                                className="inline-flex items-center mx-8 text-xs font-semibold text-blue-50 hover:text-amber-300 hover:underline transition-colors cursor-pointer"
                              >
                                <span className="px-1.5 py-0.5 rounded bg-amber-400/20 text-amber-300 border border-amber-400/40 text-[10px] font-bold mr-2">
                                  {formatShortMalayDate(ann.timestamp)}
                                </span>
                                <span>{ann.title}</span>
                              </button>
                            ))}
                          </div>
                        ))}
                      </div>
                    </div>
                  </div>
                )}

                <div className="bg-gray-100/80 border-b border-gray-200 px-6 py-2.5 flex items-center text-xs font-medium text-blue-700">
                  <Home className="w-3.5 h-3.5 text-blue-800 mr-2" />
                  <ChevronRight className="w-3.5 h-3.5 text-gray-400 mx-1" />
                  <span className="text-blue-700">Pemberitahuan</span>
                  <ChevronRight className="w-3.5 h-3.5 text-gray-400 mx-1" />
                  <span className="text-blue-900 font-semibold">Pengumuman</span>
                </div>

                <div className="p-6 md:p-8">
                  <div className="flex flex-col sm:flex-row sm:items-center justify-between gap-4 mb-6">
                    <h2 className="text-2xl font-bold text-gray-900 tracking-tight">Pengumuman</h2>

                    <div className="flex items-center gap-2.5 self-end sm:self-auto w-full sm:w-auto justify-end">
                      <label className="text-sm font-medium text-gray-700 shrink-0">Carian</label>
                      <div className="relative w-full sm:w-64">
                        <input
                          type="text"
                          value={annSearchQuery}
                          onChange={(e) => {
                            setAnnSearchQuery(e.target.value);
                            setAnnPage(1);
                          }}
                          placeholder="Kata kunci tajuk..."
                          className="w-full px-3.5 py-2 rounded-md border border-gray-300 focus:border-blue-700 focus:ring-1 focus:ring-blue-700 outline-none text-sm text-gray-800 bg-white"
                        />
                        {annSearchQuery && (
                          <button
                            type="button"
                            onClick={() => { setAnnSearchQuery(''); setAnnPage(1); }}
                            className="absolute right-2.5 top-1/2 -translate-y-1/2 text-gray-400 hover:text-gray-600"
                            title="Kosongkan carian"
                          >
                            <X className="w-4 h-4" />
                          </button>
                        )}
                      </div>
                    </div>
                  </div>

                  <div className="overflow-x-auto border-t border-b border-gray-200">
                    <table className="w-full text-left border-collapse">
                      <thead>
                        <tr className="border-b border-gray-200 bg-gray-50/60">
                          <th className="py-3.5 px-4 text-sm font-semibold text-gray-800 border-r border-gray-200/80">
                            Tajuk
                          </th>
                          <th className="py-3.5 px-4 text-sm font-semibold text-gray-800 w-36 sm:w-44 shrink-0">
                            Tarikh
                          </th>
                        </tr>
                      </thead>
                      <tbody className="divide-y divide-gray-100">
                        {isLoadingData ? (
                          <tr>
                            <td colSpan="2" className="py-8 px-4 text-center text-sm text-gray-500 animate-pulse">
                              Memuatkan senarai pengumuman...
                            </td>
                          </tr>
                        ) : paginatedAnnouncements.length === 0 ? (
                          <tr>
                            <td colSpan="2" className="py-10 px-4 text-center text-sm text-gray-500">
                              Tiada pengumuman ditemui{annSearchQuery ? ` bagi carian "${annSearchQuery}"` : ''}.
                            </td>
                          </tr>
                        ) : (
                          paginatedAnnouncements.map((ann, idx) => {
                            const isUrgent = ann.category === 'Segera / Penting';
                            const isRecent = Date.now() - Number(ann.timestamp || 0) < 7 * 24 * 60 * 60 * 1000;
                            return (
                              <tr
                                key={ann.id}
                                className={`transition-colors hover:bg-blue-50/50 ${idx % 2 === 1 ? 'bg-gray-50/30' : 'bg-white'}`}
                              >
                                <td className="py-3.5 px-4 border-r border-gray-200/80 align-top">
                                  <button
                                    type="button"
                                    onClick={() => setSelectedAnnouncement(ann)}
                                    className="text-left group focus:outline-none"
                                  >
                                    <span className="text-sm sm:text-[15px] text-[#2b579a] group-hover:text-blue-900 group-hover:underline font-medium leading-relaxed">
                                      {ann.title}
                                    </span>
                                    {isUrgent && (
                                      <span className="ml-2 inline-flex items-center px-2 py-0.5 rounded text-[10px] font-bold bg-rose-100 text-rose-700 border border-rose-200 align-middle">
                                        PENTING
                                      </span>
                                    )}
                                    {!isUrgent && isRecent && idx === 0 && currentSafePage === 1 && (
                                      <span className="ml-2 inline-flex items-center px-2 py-0.5 rounded text-[10px] font-bold bg-amber-100 text-amber-800 border border-amber-300 align-middle">
                                        BARU
                                      </span>
                                    )}
                                    {ann.linkUrl && (
                                      <ExternalLink className="w-3.5 h-3.5 inline-block ml-1.5 text-blue-500 align-middle" />
                                    )}
                                  </button>
                                </td>
                                <td className="py-3.5 px-4 text-sm text-gray-800 whitespace-nowrap align-top font-normal">
                                  {formatShortMalayDate(ann.timestamp)}
                                </td>
                              </tr>
                            );
                          })
                        )}
                      </tbody>
                    </table>
                  </div>

                  <div className="mt-6 flex flex-col sm:flex-row items-center justify-between gap-4 text-sm text-gray-700">
                    <div>
                      Memaparkan {showingFrom} sehingga {showingTo} dari {totalArticles} artikel
                    </div>

                    <div className="inline-flex items-center rounded-md border border-gray-300 bg-white overflow-hidden shadow-sm">
                      <button
                        type="button"
                        disabled={currentSafePage <= 1}
                        onClick={() => setAnnPage((p) => Math.max(1, p - 1))}
                        className="px-3.5 py-2 text-sm border-r border-gray-300 text-gray-700 hover:bg-gray-100 disabled:text-gray-300 disabled:hover:bg-white transition-colors"
                      >
                        Sebelumnya
                      </button>

                      {getPageNumbers().map((pNum, i) =>
                        pNum === '...' ? (
                          <span key={`dots-${i}`} className="px-3 py-2 text-sm text-gray-400 border-r border-gray-300">
                            ...
                          </span>
                        ) : (
                          <button
                            key={pNum}
                            type="button"
                            onClick={() => setAnnPage(Number(pNum))}
                            className={`px-3.5 py-2 text-sm border-r border-gray-300 font-medium transition-colors ${
                              currentSafePage === pNum
                                ? 'bg-gray-200/90 text-gray-900 font-bold'
                                : 'text-gray-700 hover:bg-gray-100'
                            }`}
                          >
                            {pNum}
                          </button>
                        )
                      )}

                      <button
                        type="button"
                        disabled={currentSafePage >= totalPages}
                        onClick={() => setAnnPage((p) => Math.min(totalPages, p + 1))}
                        className="px-3.5 py-2 text-sm text-gray-700 hover:bg-gray-100 disabled:text-gray-300 disabled:hover:bg-white transition-colors"
                      >
                        Seterusnya
                      </button>
                    </div>
                  </div>
                </div>
              </div>

              {selectedAnnouncement && (
                <div className="fixed inset-0 z-50 flex items-center justify-center p-4 bg-slate-950/70 backdrop-blur-sm animate-in fade-in duration-200">
                  <div className="bg-white rounded-2xl shadow-2xl w-full max-w-2xl max-h-[88vh] flex flex-col overflow-hidden border border-gray-200">
                    <div className="bg-gradient-to-r from-[#0f2354] to-[#1e3a8a] text-white px-6 py-5 flex items-start justify-between gap-4 border-b-4 border-amber-400">
                      <div>
                        <div className="flex flex-wrap items-center gap-2 mb-2">
                          <span className="px-2.5 py-0.5 rounded-full text-[11px] font-black bg-amber-400 text-blue-950 uppercase">
                            {selectedAnnouncement.category || 'Makluman Rasmi'}
                          </span>
                          <span className="text-xs text-blue-200 flex items-center">
                            <Calendar className="w-3.5 h-3.5 mr-1 text-amber-300" />
                            {formatDate(selectedAnnouncement.timestamp)}
                          </span>
                        </div>
                        <h3 className="text-lg sm:text-xl font-bold leading-snug">
                          {selectedAnnouncement.title}
                        </h3>
                      </div>
                      <button
                        type="button"
                        onClick={() => setSelectedAnnouncement(null)}
                        className="p-1.5 rounded-lg bg-white/10 hover:bg-red-500 text-white transition-colors shrink-0"
                        title="Tutup"
                      >
                        <X className="w-5 h-5" />
                      </button>
                    </div>

                    <div className="p-6 overflow-y-auto space-y-5 text-gray-800 text-sm sm:text-base leading-relaxed">
                      <div className="whitespace-pre-line bg-slate-50 p-5 rounded-xl border border-slate-200/80">
                        {selectedAnnouncement.content}
                      </div>

                      {selectedAnnouncement.linkUrl && (
                        <div className="p-4 rounded-xl bg-blue-50 border border-blue-200 flex flex-col sm:flex-row sm:items-center justify-between gap-3">
                          <div className="text-xs sm:text-sm text-blue-900 font-semibold">
                            Lampiran / Dokumen Berkaitan Disediakan:
                          </div>
                          <a
                            href={selectedAnnouncement.linkUrl}
                            target="_blank"
                            rel="noopener noreferrer"
                            className="inline-flex items-center justify-center px-4 py-2 bg-blue-900 hover:bg-blue-800 text-white text-xs font-bold rounded-lg shadow-sm transition-colors shrink-0"
                          >
                            Buka Pautan / Dokumen <ExternalLink className="w-3.5 h-3.5 ml-1.5" />
                          </a>
                        </div>
                      )}
                    </div>

                    <div className="px-6 py-4 bg-gray-50 border-t border-gray-200 flex flex-wrap items-center justify-between gap-3 text-xs text-gray-500">
                      <span>
                        Diterbitkan oleh: <strong className="text-gray-800">{selectedAnnouncement.author || 'Pentadbiran RISDA Pahang'}</strong>
                      </span>
                      <button
                        type="button"
                        onClick={() => setSelectedAnnouncement(null)}
                        className="px-5 py-2 bg-blue-900 hover:bg-blue-800 text-white font-bold rounded-lg text-xs transition-colors"
                      >
                        Tutup Paparan
                      </button>
                    </div>
                  </div>
                </div>
              )}
            </div>
          ) : (
            <div className="animate-in fade-in duration-300">
              <PublicDashboard />
            </div>
          )}
        </div>
      </div>
    );
  };

  const renderProfil = () => (
    <div className="animate-in fade-in duration-500 max-w-5xl mx-auto space-y-8">
      <div className="bg-white rounded-2xl shadow-md border border-gray-100 overflow-hidden">
        <div className="p-6 bg-gradient-to-r from-blue-900 to-blue-800 border-b border-blue-900 text-center md:text-left">
          <h1 className="text-2xl md:text-3xl font-black text-white uppercase tracking-wider">Model Transformasi RISDA 2026-2030</h1>
          <p className="text-blue-200 mt-1 font-medium text-sm md:text-base">Lakaran Masa Depan Industri Getah Negara</p>
        </div>
        <div
          ref={mtrViewerRef}
          onMouseDown={(e) => {
            if (posterLoadError || mtrZoom <= 1 || e.button !== 0) return;
            e.preventDefault();
            setIsPanningMtr(true);
            mtrPanStartRef.current = {
              x: e.clientX - mtrPan.x,
              y: e.clientY - mtrPan.y
            };
          }}
          onMouseMove={(e) => {
            if (!isPanningMtr) return;
            setMtrPan({
              x: e.clientX - mtrPanStartRef.current.x,
              y: e.clientY - mtrPanStartRef.current.y
            });
          }}
          onMouseUp={() => setIsPanningMtr(false)}
          onMouseLeave={() => setIsPanningMtr(false)}
          className={`relative w-full h-[540px] sm:h-[620px] bg-gray-100 p-4 md:p-8 border-b border-gray-200 overflow-hidden select-none ${
            !posterLoadError && mtrZoom > 1
              ? (isPanningMtr ? 'cursor-grabbing' : 'cursor-grab')
              : 'cursor-default'
          }`}
        >
          <div className="w-full h-full flex justify-center items-center">
            <div
              style={{
                transform: `translate(${mtrPan.x}px, ${mtrPan.y}px) scale(${mtrZoom})`,
                transformOrigin: 'center center',
                transition: isPanningMtr ? 'none' : 'transform 0.2s ease-out'
              }}
              className="inline-block w-full max-w-4xl"
            >
              {!posterLoadError ? (
                <img
                  src={posterSources[posterSourceIdx]}
                  alt="Poster Rasmi Model Transformasi RISDA 2026-2030"
                  referrerPolicy="no-referrer"
                  draggable={false}
                  onError={() => {
                    if (posterSourceIdx + 1 < posterSources.length) {
                      setPosterSourceIdx((prev) => prev + 1);
                    } else {
                      setPosterLoadError(true);
                    }
                  }}
                  className="w-full h-auto max-h-[540px] object-contain rounded-xl shadow-xl border border-gray-300 bg-white pointer-events-none"
                />
              ) : (
                <div className="bg-gradient-to-br from-blue-950 via-blue-900 to-indigo-900 text-white rounded-2xl p-6 md:p-10 shadow-xl border-2 border-amber-400/70">
                  <div className="flex flex-col sm:flex-row sm:items-center justify-between gap-3 border-b border-blue-700/70 pb-4 mb-6">
                    <div>
                      <span className="text-[11px] font-black uppercase tracking-widest bg-amber-400 text-blue-950 px-3 py-1 rounded-full">
                        Rangka Strategik Korporat
                      </span>
                      <h3 className="text-xl md:text-2xl font-black mt-2">
                        Model Transformasi RISDA (MTR) 2026 – 2030
                      </h3>
                    </div>
                    <a
                      href="https://drive.google.com/file/d/1bHujA0hvyOjVm0le0gs9GZonBoYKsksY/view"
                      target="_blank"
                      rel="noopener noreferrer"
                      className="inline-flex items-center px-4 py-2 bg-amber-400 hover:bg-amber-300 text-blue-950 font-bold text-xs rounded-xl shadow transition-colors shrink-0"
                    >
                      Buka Poster Asal <ExternalLink className="w-3.5 h-3.5 ml-1.5" />
                    </a>
                  </div>
                  <div className="grid grid-cols-1 md:grid-cols-3 gap-4 mb-6 text-left">
                    <div className="bg-blue-950/60 p-4 rounded-xl border border-blue-700/60">
                      <p className="text-xs font-black text-amber-300 uppercase mb-1">Sasaran Pengeluaran</p>
                      <p className="text-lg font-bold text-white">1 Juta Tan Metrik / Tahun</p>
                    </div>
                    <div className="bg-blue-950/60 p-4 rounded-xl border border-blue-700/60">
                      <p className="text-xs font-black text-amber-300 uppercase mb-1">Sasaran Pendapatan</p>
                      <p className="text-lg font-bold text-white">Purata RM4,500 Sebulan</p>
                    </div>
                    <div className="bg-blue-950/60 p-4 rounded-xl border border-blue-700/60">
                      <p className="text-xs font-black text-amber-300 uppercase mb-1">Kerangka Utama</p>
                      <p className="text-lg font-bold text-white">5 Teras • 16 Fokus • 20 Strategi</p>
                    </div>
                  </div>
                  <p className="text-xs text-blue-200">
                    Tip *localhost*: Jika ingin memaparkan fail imej poster secara terus di komputer tempatan, simpan fail poster sebagai <code className="text-amber-300 font-mono">public/poster-mtr-2030.jpg</code>.
                  </p>
                </div>
              )}
            </div>
          </div>

          {!posterLoadError && (
            <div className="absolute bottom-4 right-4 z-20 flex flex-col items-center bg-neutral-900/90 backdrop-blur-sm rounded-lg border border-white/15 shadow-xl overflow-hidden divide-y divide-white/15">
              <button
                type="button"
                onClick={() => setMtrZoom((prev) => Math.min(4.0, Number((prev + 0.2).toFixed(1))))}
                disabled={mtrZoom >= 4.0}
                aria-label="Zoom In"
                title="Zoom In"
                className="w-11 h-9 flex items-center justify-center text-white hover:bg-white/15 active:bg-white/25 disabled:opacity-35 transition-colors"
              >
                <Plus className="w-4 h-4 stroke-[2.5]" />
              </button>
              <div
                title="Peratus Zoom Semasa"
                className="w-11 py-1 px-1 flex items-center justify-center text-[11px] font-mono font-bold text-amber-300 tabular-nums select-none"
              >
                {Math.round(mtrZoom * 100)}%
              </div>
              <button
                type="button"
                onClick={() =>
                  setMtrZoom((prev) => {
                    const nextZoom = Math.max(0.8, Number((prev - 0.2).toFixed(1)));
                    if (nextZoom <= 1) {
                      setMtrPan({ x: 0, y: 0 });
                    }
                    return nextZoom;
                  })
                }
                disabled={mtrZoom <= 0.8}
                aria-label="Zoom Out"
                title="Zoom Out"
                className="w-11 h-9 flex items-center justify-center text-white hover:bg-white/15 active:bg-white/25 disabled:opacity-35 transition-colors"
              >
                <span className="w-3.5 h-[2.5px] bg-current rounded-full block"></span>
              </button>
              <button
                type="button"
                onClick={() => {
                  setMtrZoom(1);
                  setMtrPan({ x: 0, y: 0 });
                }}
                aria-label="Kembalikan Saiz Asal"
                title="Saiz Asal (100%)"
                className="w-11 h-9 flex items-center justify-center text-slate-200 hover:bg-white/15 active:bg-white/25 transition-colors"
              >
                <RotateCcw className="w-3.5 h-3.5 stroke-[2.2]" />
              </button>
            </div>
          )}
        </div>
      </div>

      <div className="grid grid-cols-1 md:grid-cols-3 gap-6">
        <div className="bg-white p-8 rounded-2xl shadow-sm border-t-4 border-yellow-500 hover:shadow-md transition-shadow">
          <div className="bg-yellow-100 w-14 h-14 rounded-full flex items-center justify-center mb-6"><Eye className="w-7 h-7 text-yellow-600" /></div>
          <h2 className="text-xl font-bold text-gray-900 mb-4">VISI</h2>
          <p className="text-gray-700 leading-relaxed font-medium">Sebagai Peneraju Utama Yang Berprestasi Tinggi Dalam Memperkasa Sosio-ekonomi Pekebun Kecil.</p>
        </div>
        <div className="bg-white p-8 rounded-2xl shadow-sm border-t-4 border-blue-600 hover:shadow-md transition-shadow">
          <div className="bg-blue-100 w-14 h-14 rounded-full flex items-center justify-center mb-6"><Target className="w-7 h-7 text-blue-700" /></div>
          <h2 className="text-xl font-bold text-gray-900 mb-4">MISI</h2>
          <p className="text-gray-700 leading-relaxed font-medium">Menguasai Industri Getah Di Sepanjang Rantaian Bekalan Berasaskan Transformasi Digital.</p>
        </div>
        <div className="bg-white p-8 rounded-2xl shadow-sm border-t-4 border-green-500 hover:shadow-md transition-shadow">
          <div className="bg-green-100 w-14 h-14 rounded-full flex items-center justify-center mb-6"><Flag className="w-7 h-7 text-green-700" /></div>
          <h2 className="text-xl font-bold text-gray-900 mb-4">OBJEKTIF</h2>
          <p className="text-gray-700 leading-relaxed font-medium">Memastikan Pengeluaran Getah Negara Mencapai 1 Juta Tan Metrik Setahun Pada Akhir Tahun 2030.</p>
        </div>
      </div>

      <div className="bg-blue-900 rounded-2xl shadow-lg p-6 md:p-10 text-white relative overflow-hidden">
        <div className="absolute top-0 right-0 opacity-10 pointer-events-none"><Layers className="w-64 h-64 -mt-10 -mr-10" /></div>
        <div className="relative z-10">
          <div className="flex flex-wrap items-center justify-center gap-4 mb-8 text-center">
            <button onClick={() => setMtrTab('teras')} className={`px-7 py-3 rounded-full font-black text-lg transition-all ${mtrTab === 'teras' ? 'bg-yellow-500 text-blue-900' : 'bg-blue-800/80 text-blue-100'}`}>5 TERAS</button>
            <button onClick={() => setMtrTab('fokus')} className={`px-7 py-3 rounded-full font-black text-lg transition-all ${mtrTab === 'fokus' ? 'bg-white text-blue-900' : 'bg-blue-800/80 text-blue-100'}`}>16 FOKUS</button>
            <button onClick={() => setMtrTab('strategi')} className={`px-7 py-3 rounded-full font-black text-lg transition-all ${mtrTab === 'strategi' ? 'bg-yellow-500 text-blue-900' : 'bg-blue-800/80 text-blue-100'}`}>20 STRATEGI</button>
          </div>
          <div className="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6">
            {mtrData.map((item) => (
              <div key={item.id} className={`bg-blue-800/60 p-6 rounded-2xl border-2 ${item.borderWarna} shadow-lg`}>
                <div className="flex items-center justify-between mb-3">
                  <span className="text-yellow-400 font-black text-sm tracking-wider bg-blue-950/60 px-3 py-1 rounded-full border border-blue-700">{item.teras}</span>
                </div>
                <h4 className="font-bold text-white text-lg mb-3 leading-snug">{item.tajuk}</h4>
                <ul className="space-y-2.5">
                   {mtrTab === 'teras' ? (
                     <li className="flex items-start text-sm bg-blue-950/40 p-2 rounded-xl border border-blue-800/80">
                       <CheckCircle2 className="w-4 h-4 text-yellow-400 mr-2 mt-0.5 shrink-0" />
                       <span><strong>Impak:</strong> {item.impak}</span>
                     </li>
                   ) : null}
                   {mtrTab === 'fokus' ? item.fokus.map((f, idx) => <li key={idx} className="flex items-start text-sm bg-blue-950/40 p-2 rounded-xl"><CheckCircle2 className="w-4 h-4 text-emerald-400 mr-2 mt-0.5 shrink-0" />{f}</li>) : null}
                   {mtrTab === 'strategi' ? item.strategi.map((s, idx) => <li key={idx} className="flex items-start text-sm bg-blue-950/40 p-2 rounded-xl border border-blue-800/80"><span className="text-yellow-400 mr-2">{idx+1}.</span>{s}</li>) : null}
                </ul>
              </div>
            ))}
          </div>
        </div>
      </div>
    </div>
  );

  const renderDirektori = () => (
    <div className="animate-in fade-in duration-500 max-w-6xl mx-auto">
      <div className="flex items-center space-x-4 mb-8">
        <div className="p-3 bg-blue-100 text-blue-700 rounded-lg"><Users className="w-6 h-6" /></div>
        <div><h1 className="text-3xl font-bold text-gray-900">Direktori Pegawai</h1></div>
      </div>
      <div className="bg-white rounded-xl shadow-sm border border-gray-200 overflow-hidden">
        <div className="overflow-x-auto">
          <table className="w-full text-left border-collapse">
            <thead>
              <tr className="bg-blue-900 text-white text-sm">
                <th className="p-4 font-semibold">Nama</th>
                <th className="p-4 font-semibold">Jawatan</th>
                <th className="p-4 font-semibold">Sambungan</th>
                <th className="p-4 font-semibold">E-mel</th>
                <th className="p-4 font-semibold">Bahagian</th>
              </tr>
            </thead>
            <tbody className="divide-y divide-gray-100">
              {directoryData.map((person, index) => (
                <tr key={index} className="hover:bg-blue-50 transition-colors">
                  <td className="p-4 font-bold text-gray-900">{person.name}</td>
                  <td className="p-4 text-gray-700">{person.role}</td>
                  <td className="p-4 text-gray-700 font-medium">{person.extension}</td>
                  <td className="p-4"><a href={`mailto:${person.email}`} className="text-blue-600 hover:text-yellow-600">{person.email}</a></td>
                  <td className="p-4 text-gray-700">{person.department}</td>
                </tr>
              ))}
            </tbody>
          </table>
        </div>
      </div>
    </div>
  );

  const renderLokasi = () => {
    const daerahList = [
      { nama: "Pejabat RISDA Daerah Bentong", tel: "09-2221155", alamat: "Tingkat 1, Bangunan Persekutuan, 28700 Bentong, Pahang" },
      { nama: "Pejabat RISDA Daerah Bera", tel: "09-2506899", alamat: "No. 15 & 16, Jalan 2, Pusat Komersial Bandar Bera, 28200 Bera, Pahang" },
      { nama: "Pejabat RISDA Daerah Jerantut", tel: "09-2662283", alamat: "Tingkat 2, Bangunan Persekutuan, 27000 Jerantut, Pahang" },
      { nama: "Pejabat RISDA Daerah Lipis", tel: "09-3121288", alamat: "Tingkat 1, Bangunan Persekutuan, 27200 Kuala Lipis, Pahang" },
      { nama: "Pejabat RISDA Daerah Maran", tel: "09-4771233", alamat: "Pusat Jengka, 26400 Bandar Jengka, Pahang" },
      { nama: "Pejabat RISDA Daerah Pahang Timur", tel: "09-5141911", alamat: "Bangunan RISDA, Lot 7876, Jalan Haji Junid, 25200 Kuantan, Pahang" },
      { nama: "Pejabat RISDA Daerah Raub", tel: "09-3551221", alamat: "KM 2, Jalan Lipis, 27600 Raub, Pahang" },
      { nama: "Pejabat RISDA Daerah Temerloh", tel: "09-2961233", alamat: "Tingkat 2, Bangunan Persekutuan, 28000 Temerloh, Pahang" }
    ];

    return (
      <div className="animate-in fade-in duration-500 max-w-6xl mx-auto">
        <div className="flex items-center space-x-4 mb-8">
          <div className="p-3 bg-blue-100 text-blue-700 rounded-lg"><MapPin className="w-6 h-6" /></div>
          <div><h1 className="text-3xl font-bold text-gray-900">Lokasi Pusat Tanggungjawab</h1></div>
        </div>

        <div className="bg-white border border-gray-200 rounded-xl shadow-sm overflow-hidden mb-12">
          <div className="grid grid-cols-1 md:grid-cols-3 divide-y md:divide-y-0 md:divide-x divide-gray-200">
            <div className="p-6 bg-gray-50 flex flex-col justify-center">
              {buildingLoadFailed ? (
                <div className="rounded-lg border-4 border-white shadow-md bg-gradient-to-br from-blue-950 via-blue-900 to-blue-800 text-white p-5 min-h-[200px] flex flex-col justify-between">
                  <div>
                    <span className="inline-block text-[10px] font-black uppercase tracking-wider bg-amber-400 text-blue-950 px-2.5 py-0.5 rounded-full mb-2">
                      Ibu Pejabat Negeri
                    </span>
                    <h4 className="font-bold text-base leading-snug">
                      Bangunan RISDA Negeri Pahang
                    </h4>
                    <p className="text-xs text-blue-200 mt-1 leading-relaxed">
                      Lot 7876, Jalan Haji Junid, 25200 Kuantan, Pahang.
                    </p>
                  </div>
                  <p className="text-[11px] text-amber-200/90 mt-3 pt-2 border-t border-blue-700/70">
                    Letakkan <code className="font-mono text-amber-300">public/prn-pahang.jpg</code> untuk imej lokal.
                  </p>
                </div>
              ) : (
                <div className="rounded-lg overflow-hidden border-4 border-white shadow-md bg-white">
                  <img
                    src={buildingSources[buildingImgIdx]}
                    alt="Bangunan RISDA Pahang"
                    referrerPolicy="no-referrer"
                    onError={() => setBuildingImgIdx((prev) => prev + 1)}
                    className="w-full h-auto object-cover min-h-[200px]"
                  />
                </div>
              )}
            </div>
            
            <div className="p-0 h-64 md:h-auto bg-gray-200 relative">
              <iframe width="100%" height="100%" frameBorder="0" scrolling="no" marginHeight={0} marginWidth={0} src="https://maps.google.com/maps?q=Pejabat%20RISDA%20Negeri%20Pahang&t=&z=15&ie=UTF8&iwloc=&output=embed" className="absolute inset-0 w-full h-full"></iframe>
            </div>
            
            <div className="p-6 flex flex-col">
              <p className="text-gray-700 text-sm mb-4 leading-relaxed">
                Tingkat 1, Blok A, Bangunan RISDA, Lot 7876, Jalan Haji Junid,<br/>25200 Kuantan, Pahang.
              </p>
              <div className="text-gray-700 text-sm space-y-1 mb-8">
                <p><span className="font-bold text-gray-900">Tel :</span> 09-5141911 / 09-5141912</p>
              </div>
              
              <div className="mt-auto space-y-3 w-full">
                <button onClick={() => setLokasiTab(lokasiTab === 'daerah' ? '' : 'daerah')} className={`w-full flex items-center px-4 py-2 border rounded-lg font-bold transition-colors ${lokasiTab === 'daerah' ? 'border-blue-900 bg-blue-900 text-white shadow-md' : 'border-blue-900 text-blue-900 hover:bg-blue-50'}`}>
                  <MapPin className="w-5 h-5 mr-3" /> Pejabat Daerah (8 PT)
                </button>
                <button onClick={() => setLokasiTab(lokasiTab === 'stesen' ? '' : 'stesen')} className={`w-full flex items-center px-4 py-2 border rounded-lg font-bold transition-colors ${lokasiTab === 'stesen' ? 'border-teal-700 bg-teal-700 text-white shadow-md' : 'border-teal-700 text-teal-700 hover:bg-teal-50'}`}>
                  <List className="w-5 h-5 mr-3" /> Pejabat Stesen (20 PRS)
                </button>
                <button onClick={() => setLokasiTab(lokasiTab === 'mini' ? '' : 'mini')} className={`w-full flex items-center px-4 py-2 border rounded-lg font-bold transition-colors ${lokasiTab === 'mini' ? 'border-orange-500 bg-orange-500 text-white shadow-md' : 'border-orange-500 text-orange-600 hover:bg-orange-50'}`}>
                  <Layers className="w-5 h-5 mr-3" /> Pejabat Mini Stesen (3 PRMS)
                </button>
              </div>
            </div>
          </div>
        </div>

        {lokasiTab === 'daerah' && (
          <div className="animate-in slide-in-from-top-4 duration-300">
            <h3 className="text-2xl font-bold text-blue-900 mb-6 border-b-2 border-yellow-400 pb-2 inline-block">Senarai Pejabat Daerah (8 PT)</h3>
            <div className="grid grid-cols-1 lg:grid-cols-2 gap-6">
              {daerahList.map((daerah, idx) => (
                <div key={idx} className="bg-white border border-gray-200 rounded-xl p-4 flex flex-col sm:flex-row gap-4 shadow-sm relative overflow-hidden hover:border-blue-300 transition-colors">
                  <div className="w-full sm:w-1/3 h-40 sm:h-auto relative rounded-lg overflow-hidden border border-gray-200 shrink-0 bg-gray-100">
                    <iframe width="100%" height="100%" frameBorder="0" scrolling="no" marginHeight={0} marginWidth={0} src={`https://maps.google.com/maps?q=${encodeURIComponent(daerah.nama + ', Pahang')}&t=&z=14&ie=UTF8&iwloc=&output=embed`} className="absolute inset-0 w-full h-full"></iframe>
                    <a href={`https://maps.google.com/maps?q=${encodeURIComponent(daerah.nama + ' ' + daerah.alamat)}`} target="_blank" rel="noopener noreferrer" className="absolute top-2 left-2 bg-white px-2 py-1 text-xs font-bold text-blue-600 rounded shadow-md border border-gray-100 hover:bg-blue-50 flex items-center z-10">
                      Maps <span className="ml-1">↗</span>
                    </a>
                  </div>
                  <div className="w-full sm:w-2/3 flex flex-col justify-center mt-2 sm:mt-0">
                    <h4 className="font-bold text-gray-900 text-md mb-2">{daerah.nama}</h4>
                    <p className="text-sm text-gray-600 mb-3 leading-relaxed">{daerah.alamat}</p>
                    <div className="mt-auto">
                      <p className="text-sm font-medium text-blue-800 bg-blue-50 border border-blue-100 inline-block px-3 py-1 rounded"><Phone className="w-3 h-3 inline mr-1" /> {daerah.tel}</p>
                    </div>
                  </div>
                </div>
              ))}
            </div>
          </div>
        )}

        {(lokasiTab === 'stesen' || lokasiTab === 'mini') && (
          <div className="animate-in slide-in-from-top-4 duration-300">
            {(() => {
              const currentList = stesenList.filter(s => {
                const isMini = s.nama.toLowerCase().includes('mini') || s.nama.toLowerCase().includes('prms');
                return lokasiTab === 'mini' ? isMini : !isMini;
              });
              return (
                <div className="flex flex-col sm:flex-row justify-between items-start sm:items-center gap-4 mb-6">
                  <h3 className={`text-2xl font-bold border-b-2 pb-1 inline-block ${lokasiTab === 'mini' ? 'text-orange-900 border-orange-400' : 'text-blue-900 border-yellow-400'}`}>
                    {lokasiTab === 'mini' ? `Senarai Pejabat RISDA Mini Stesen (${currentList.length} PRMS)` : `Senarai Pejabat RISDA Stesen (${currentList.length} PRS)`}
                  </h3>
                  <div className="flex items-center space-x-2 bg-white px-3 py-1.5 rounded-lg border border-gray-200 shadow-sm">
                    <Filter className="w-4 h-4 text-blue-900" />
                    <span className="text-xs font-semibold text-gray-700">Tapis Daerah:</span>
                    <select value={filterStesenDaerah} onChange={(e) => setFilterStesenDaerah(e.target.value)} className="text-xs font-bold text-blue-900 bg-transparent outline-none cursor-pointer">
                      <option value="Semua">Semua Daerah</option>
                      {[...new Set(currentList.map(s => s.daerah).filter(Boolean))].sort().map(d => <option key={d} value={d}>{d}</option>)}
                    </select>
                  </div>
                </div>
              );
            })()}

            {isLoadingStesen ? (
              <div className="bg-white border border-gray-200 rounded-xl p-8 text-center shadow-sm">
                <div className="inline-block animate-spin rounded-full h-8 w-8 border-b-2 border-teal-600 mb-2"></div>
              </div>
            ) : (
              <div className="grid grid-cols-1 lg:grid-cols-2 gap-6">
                {stesenList
                  .filter(s => filterStesenDaerah === 'Semua' ? true : s.daerah === filterStesenDaerah)
                  .filter(s => {
                    const isMini = s.nama.toLowerCase().includes('mini') || s.nama.toLowerCase().includes('prms');
                    return lokasiTab === 'mini' ? isMini : !isMini;
                  })
                  .map((stesen, idx) => {
                    const isMini = stesen.nama.toLowerCase().includes('mini') || stesen.nama.toLowerCase().includes('prms');
                    return (
                      <div key={idx} className="bg-white border border-gray-200 rounded-xl p-4 flex flex-col sm:flex-row gap-4 shadow-sm relative overflow-hidden hover:border-teal-300 transition-colors">
                        <div className="w-full sm:w-1/3 h-40 sm:h-auto relative rounded-lg overflow-hidden border border-gray-200 shrink-0 bg-gray-100">
                           <iframe width="100%" height="100%" frameBorder="0" scrolling="no" marginHeight={0} marginWidth={0} src={`https://maps.google.com/maps?q=${encodeURIComponent(stesen.nama + ', Pahang')}&t=&z=14&ie=UTF8&iwloc=&output=embed`} className="absolute inset-0 w-full h-full"></iframe>
                           <a href={`https://maps.google.com/maps?q=${encodeURIComponent(stesen.nama + ' ' + stesen.alamat)}`} target="_blank" rel="noopener noreferrer" className="absolute top-2 left-2 bg-white px-2 py-1 text-xs font-bold text-blue-600 rounded shadow-md border border-gray-100 hover:bg-blue-50 flex items-center z-10">
                             Maps <span className="ml-1">↗</span>
                           </a>
                        </div>
                        <div className={`absolute top-0 right-0 px-3 py-1 rounded-bl-lg text-[10px] font-bold text-white shadow-sm z-10 ${isMini ? 'bg-orange-500' : 'bg-teal-600'}`}>{isMini ? 'MINI STESEN (PRMS)' : 'STESEN (PRS)'}</div>
                        
                        <div className="w-full sm:w-2/3 flex flex-col justify-center mt-4 sm:mt-0">
                          <span className="text-[10px] font-bold px-2 py-0.5 rounded bg-gray-100 text-gray-600 border border-gray-200 self-start mb-2 uppercase tracking-wide">{stesen.daerah}</span>
                          <h4 className="font-bold text-gray-900 text-md mb-2 pr-2">{stesen.nama}</h4>
                          <p className="text-sm text-gray-600 mb-3 leading-relaxed">{stesen.alamat}</p>
                          <div className="mt-auto">
                            <p className="text-sm font-medium text-teal-800 bg-teal-50 border border-teal-100 inline-block px-3 py-1 rounded"><Phone className="w-3 h-3 inline mr-1" /> {stesen.tel}</p>
                          </div>
                        </div>
                      </div>
                    );
                })}
              </div>
            )}
          </div>
        )}
      </div>
    );
  };

  const renderAdmin = () => {
    if (!isAdminLoggedIn) {
      return (
        <div className="animate-in fade-in duration-500 flex justify-center items-center min-h-[60vh]">
          <div className="bg-white p-8 rounded-2xl shadow-lg border border-gray-100 max-w-md w-full">
            <div className="text-center mb-8">
              <div className="inline-flex p-4 bg-blue-50 text-blue-800 rounded-full mb-4"><LogIn className="w-8 h-8" /></div>
              <h2 className="text-2xl font-bold text-gray-900">Log Masuk Kakitangan</h2>
              <p className="text-gray-500 text-sm mt-2">Sila masukkan ID Log Masuk (IC/Username) untuk mengakses sistem.</p>
            </div>
            <form onSubmit={handleLogin} className="space-y-5">
              <div>
                <label className="block text-sm font-medium text-gray-700 mb-1">ID Log Masuk (Username)</label>
                <input type="text" value={icInput} onChange={(e) => setIcInput(e.target.value)} className="w-full px-4 py-3 rounded-lg border border-gray-300 focus:ring-2 focus:ring-blue-900 outline-none" placeholder="Contoh: No. KP tanpa (-)" required />
              </div>
              <div>
                <label className="block text-sm font-medium text-gray-700 mb-1">Kata Laluan (Password)</label>
                <div className="relative">
                  <input type={showPassword ? "text" : "password"} value={passwordInput} onChange={(e) => setPasswordInput(e.target.value)} className="w-full pl-4 pr-12 py-3 rounded-lg border border-gray-300 focus:ring-2 focus:ring-blue-900 outline-none" placeholder="Masukkan kata laluan..." required />
                  <button type="button" onClick={() => setShowPassword(!showPassword)} className="absolute right-3 top-1/2 -translate-y-1/2 p-1.5 text-gray-500 hover:text-blue-900 rounded-lg">{showPassword ? <EyeOff className="w-5 h-5 text-blue-900" /> : <Eye className="w-5 h-5" />}</button>
                </div>
              </div>
              {loginError && <p className="text-red-500 text-sm font-medium bg-red-50 p-3 rounded-lg border border-red-100">{loginError}</p>}
              <button type="submit" className="w-full bg-blue-900 hover:bg-blue-800 text-white font-semibold py-3 px-4 rounded-lg shadow-md">Log Masuk Dashboard</button>
            </form>
          </div>
        </div>
      );
    }

    return (
      <div className="animate-in fade-in duration-500 max-w-6xl mx-auto">
        <div className="flex flex-col md:flex-row justify-between items-center mb-6 gap-4 bg-white p-6 rounded-xl shadow-sm border border-gray-200">
          <div className="flex items-center space-x-4">
            <div className="p-3 bg-blue-100 text-blue-900 rounded-lg"><Users className="w-8 h-8" /></div>
            <div>
              <h1 className="text-2xl md:text-3xl font-bold text-gray-900">Dashboard Pentadbir</h1>
              <p className="text-gray-600 text-sm">
                Log masuk sebagai: <strong className="text-blue-900">{loggedInUser?.nama || 'Pentadbir'}</strong>
              </p>
            </div>
          </div>
          <button onClick={handleLogout} className="flex items-center px-5 py-2.5 bg-red-50 hover:bg-red-100 text-red-600 rounded-lg font-bold transition-colors border border-red-100"><LogOut className="w-4 h-4 mr-2" /> Log Keluar</button>
        </div>

        <div className="flex flex-nowrap overflow-x-auto space-x-2 bg-white p-2 rounded-xl shadow-sm border border-gray-200 mb-8 w-full hide-scrollbar">
          <button onClick={() => setAdminTab('utama')} className={`flex items-center px-6 py-3 rounded-lg font-bold transition-all whitespace-nowrap ${adminTab === 'utama' ? 'bg-blue-900 text-yellow-400 shadow-md' : 'text-gray-600 hover:bg-blue-50 hover:text-blue-900'}`}><Home className="w-5 h-5 mr-2" /> Utama</button>
          <button onClick={() => setAdminTab('pentadbiran')} className={`flex items-center px-6 py-3 rounded-lg font-bold transition-all whitespace-nowrap ${adminTab === 'pentadbiran' ? 'bg-blue-900 text-yellow-400 shadow-md' : 'text-gray-600 hover:bg-blue-50 hover:text-blue-900'}`}><Briefcase className="w-5 h-5 mr-2" /> Pentadbiran</button>
          <button onClick={() => setAdminTab('kewangan')} className={`flex items-center px-6 py-3 rounded-lg font-bold transition-all whitespace-nowrap ${adminTab === 'kewangan' ? 'bg-blue-900 text-yellow-400 shadow-md' : 'text-gray-600 hover:bg-blue-50 hover:text-blue-900'}`}><DollarSign className="w-5 h-5 mr-2" /> Kewangan</button>
          <button onClick={() => setAdminTab('kejuruteraan')} className={`flex items-center px-6 py-3 rounded-lg font-bold transition-all whitespace-nowrap ${adminTab === 'kejuruteraan' ? 'bg-blue-900 text-yellow-400 shadow-md' : 'text-gray-600 hover:bg-blue-50 hover:text-blue-900'}`}><Wrench className="w-5 h-5 mr-2" /> Kejuruteraan</button>
        </div>

        {adminTab === 'utama' && (
          <div className="space-y-8 animate-in fade-in">
            <DashboardHR />
            <div className="pt-8 mt-4 border-t-2 border-dashed border-gray-200">
              {canManageAnnouncements ? (
                <div className="bg-white rounded-2xl shadow-sm border border-gray-200 p-6 md:p-8">
                  <div className="flex flex-col sm:flex-row sm:items-center justify-between gap-3 mb-6 pb-4 border-b border-gray-100">
                    <h2 className="text-xl font-black text-blue-900 flex items-center">
                      <Plus className="w-6 h-6 mr-2 text-yellow-500" />
                      {editingAnnId ? 'Kemas Kini Pengumuman' : 'Tambah Pengumuman Baru'}
                    </h2>
                    <span className="text-xs font-bold bg-emerald-50 text-emerald-800 px-3 py-1 rounded-full border border-emerald-200 flex items-center self-start sm:self-auto">
                      <ShieldCheck className="w-4 h-4 mr-1.5 text-emerald-600" /> Akses Khas Pentadbir
                    </span>
                  </div>

                  {announcementFeedback && (
                    <div className="mb-6 p-4 bg-emerald-50 border border-emerald-200 text-emerald-900 rounded-xl text-sm font-bold flex items-center justify-between shadow-sm">
                      <span className="flex items-center">
                        <CheckCircle2 className="w-5 h-5 mr-2 text-emerald-600 shrink-0" />
                        {announcementFeedback}
                      </span>
                      <button
                        type="button"
                        onClick={() => { setHomeSubTab('info'); navigateTo('home'); }}
                        className="text-xs bg-emerald-700 hover:bg-emerald-800 text-white px-3 py-1.5 rounded-lg font-bold shrink-0 ml-3"
                      >
                        Lihat di Laman Utama
                      </button>
                    </div>
                  )}

                  <form onSubmit={handlePostAnnouncement} className="space-y-5">
                    <div className="grid grid-cols-1 md:grid-cols-3 gap-4">
                      <div className="md:col-span-2">
                        <label className="block text-sm font-bold text-gray-700 mb-2">Tajuk Pengumuman</label>
                        <input
                          type="text"
                          value={newTitle}
                          onChange={(e) => setNewTitle(e.target.value)}
                          placeholder="Masukkan tajuk hebahan atau makluman..."
                          className="w-full px-4 py-3 rounded-xl border border-gray-300 focus:ring-2 focus:ring-blue-900 outline-none"
                          required
                        />
                      </div>
                      <div>
                        <label className="block text-sm font-bold text-gray-700 mb-2">Kategori Hebahan</label>
                        <select
                          value={newCategory}
                          onChange={(e) => setNewCategory(e.target.value)}
                          className="w-full px-4 py-3 rounded-xl border border-gray-300 focus:ring-2 focus:ring-blue-900 outline-none bg-white font-semibold text-gray-800"
                        >
                          <option value="Makluman Rasmi">Makluman Rasmi</option>
                          <option value="Pentadbiran">Pentadbiran</option>
                          <option value="Mesyuarat / Taklimat">Mesyuarat / Taklimat</option>
                          <option value="Segera / Penting">Segera / Penting</option>
                        </select>
                      </div>
                    </div>

                    <div>
                      <label className="block text-sm font-bold text-gray-700 mb-2">Kandungan Pengumuman</label>
                      <textarea
                        value={newContent}
                        onChange={(e) => setNewContent(e.target.value)}
                        rows={5}
                        placeholder="Tulis butiran penuh pengumuman yang akan dipaparkan apabila pengguna klik pada tajuk..."
                        className="w-full px-4 py-3 rounded-xl border border-gray-300 focus:ring-2 focus:ring-blue-900 outline-none resize-none"
                        required
                      ></textarea>
                    </div>

                    <div>
                      <label className="block text-sm font-bold text-gray-700 mb-2">
                        Pautan Dokumen / Lampiran <span className="text-xs font-normal text-gray-400">(Pilihan - URL Google Drive / PDF / Borang)</span>
                      </label>
                      <input
                        type="url"
                        value={newLinkUrl}
                        onChange={(e) => setNewLinkUrl(e.target.value)}
                        placeholder="Contoh: https://drive.google.com/..."
                        className="w-full px-4 py-3 rounded-xl border border-gray-300 focus:ring-2 focus:ring-blue-900 outline-none text-sm"
                      />
                    </div>

                    <div className="flex items-center justify-end gap-3">
                      {editingAnnId && (
                        <button
                          type="button"
                          onClick={() => { setEditingAnnId(null); setNewTitle(''); setNewContent(''); setNewLinkUrl(''); setNewCategory('Makluman Rasmi'); }}
                          className="px-5 py-3 bg-gray-100 hover:bg-gray-200 text-gray-700 font-bold rounded-xl transition-colors text-sm"
                        >
                          Batal Suntingan
                        </button>
                      )}
                      <button
                        type="submit"
                        disabled={isSubmitting}
                        className={`flex items-center px-6 py-3 bg-blue-900 text-white font-bold rounded-xl shadow-md transition-all ${isSubmitting ? 'opacity-70' : 'hover:bg-blue-800'}`}
                      >
                        <Send className="w-4 h-4 mr-2 text-yellow-400" />
                        {isSubmitting ? 'Menghantar...' : editingAnnId ? 'Simpan Perubahan' : 'Terbitkan Pengumuman'}
                      </button>
                    </div>
                  </form>

                  <div className="mt-8 pt-6 border-t border-gray-200">
                    <h3 className="text-sm font-black text-gray-800 uppercase tracking-wider mb-4">
                      Senarai Pengumuman Diterbitkan ({announcements.length})
                    </h3>
                    {announcements.length === 0 ? (
                      <p className="text-xs text-gray-500 italic">Belum ada pengumuman diterbitkan.</p>
                    ) : (
                      <div className="space-y-3 max-h-[320px] overflow-y-auto pr-1">
                        {announcements.map((ann) => (
                          <div key={ann.id} className="p-4 rounded-xl bg-slate-50 border border-slate-200 flex flex-col sm:flex-row sm:items-center justify-between gap-3">
                            <div className="pr-2">
                              <div className="flex items-center gap-2 mb-1">
                                <span className="text-[10px] font-black bg-blue-100 text-blue-900 px-2 py-0.5 rounded-full">
                                  {ann.category || 'Makluman Rasmi'}
                                </span>
                                <span className="text-[11px] text-gray-400">{formatDate(ann.timestamp)}</span>
                              </div>
                              <h4 className="font-bold text-gray-900 text-sm">{ann.title}</h4>
                              <p className="text-xs text-gray-600 line-clamp-2 mt-0.5">{ann.content}</p>
                            </div>
                            <div className="flex items-center gap-2 shrink-0 self-end sm:self-center">
                              <button
                                type="button"
                                onClick={() => handleStartEditAnnouncement(ann)}
                                className="px-3 py-1.5 bg-amber-50 hover:bg-amber-100 text-amber-800 border border-amber-200 rounded-lg text-xs font-bold flex items-center"
                              >
                                <Edit3 className="w-3.5 h-3.5 mr-1" /> Edit
                              </button>
                              <button
                                type="button"
                                onClick={() => handleDeleteAnnouncement(ann.id)}
                                className="px-3 py-1.5 bg-red-50 hover:bg-red-100 text-red-600 border border-red-200 rounded-lg text-xs font-bold flex items-center"
                              >
                                <Trash2 className="w-3.5 h-3.5 mr-1" /> Padam
                              </button>
                            </div>
                          </div>
                        ))}
                      </div>
                    )}
                  </div>
                </div>
              ) : (
                <div className="bg-slate-50 rounded-2xl border border-slate-200 p-6 flex items-center justify-between gap-4">
                  <div className="flex items-center space-x-3.5">
                    <div className="p-3 bg-slate-200 text-slate-600 rounded-xl shrink-0">
                      <Lock className="w-5 h-5" />
                    </div>
                    <div>
                      <h3 className="text-sm font-black text-slate-800">Pengurusan Pengumuman Laman Utama (Akses Terhad)</h3>
                      <p className="text-xs text-slate-500 mt-0.5">
                        Fungsi menerbitkan dan menyunting pengumuman portal dikhaskan kepada Pentadbir Utama Portal sahaja.
                      </p>
                    </div>
                  </div>
                </div>
              )}
            </div>
          </div>
        )}
        {adminTab === 'pentadbiran' && (<div className="animate-in fade-in"><h2 className="text-2xl font-bold text-blue-900">Modul Pentadbiran (Sedang Dibangunkan)</h2></div>)}
        {adminTab === 'kewangan' && (<div className="animate-in fade-in"><h2 className="text-2xl font-bold text-blue-900">Modul Kewangan (Sedang Dibangunkan)</h2></div>)}
        {adminTab === 'kejuruteraan' && (<div className="animate-in fade-in"><h2 className="text-2xl font-bold text-blue-900">Modul Kejuruteraan (Sedang Dibangunkan)</h2></div>)}
      </div>
    );
  };

  const navItems = [
    { id: 'home', label: 'Laman Utama' },
    { id: 'profil', label: 'MTR 2030' },
    { id: 'direktori', label: 'Direktori' },
    { id: 'lokasi', label: 'Lokasi Pusat Tanggungjawab' }
  ];

  return (
    <div className="min-h-screen bg-gray-50 flex flex-col font-sans text-gray-800 selection:bg-yellow-200 selection:text-blue-900">
      <header className="bg-blue-900 text-white shadow-lg sticky top-0 z-50">
        <div className="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
          <div className="flex justify-between items-center h-20">
            <div className="flex items-center cursor-pointer group space-x-3" onClick={() => navigateTo('home')}>
              <RisdaDriveLogo className="h-11 md:h-13 w-auto opacity-95 group-hover:opacity-100 group-hover:scale-105" showGlow={false} isSecond={true} />
              <RisdaDriveLogo className="h-10 md:h-12 w-auto hidden sm:block group-hover:scale-105" showGlow={true} isSecond={false} />
              <div className="flex flex-col pl-2 border-l border-blue-700">
                <span className="font-bold text-xl tracking-wide">RISDA PAHANG</span>
                <span className="text-xs text-blue-200 font-medium">Portal Rasmi Pentadbiran</span>
              </div>
            </div>
            <nav className="hidden md:flex space-x-1 items-center">
              {navItems.map((item) => (
                <button key={item.id} onClick={() => navigateTo(item.id)} className={`px-4 py-2 rounded-lg text-sm font-medium transition-colors ${currentPage === item.id ? 'bg-blue-800 text-yellow-400' : 'hover:bg-blue-800 hover:text-white text-blue-50'}`}>{item.label}</button>
              ))}
              <div className="w-px h-6 bg-blue-700 mx-2"></div>
              <button onClick={() => navigateTo('admin')} className={`px-4 py-2 rounded-lg text-sm font-medium flex items-center transition-colors ${currentPage === 'admin' ? 'bg-yellow-500 text-blue-900 font-bold' : 'bg-blue-800 hover:bg-yellow-500 hover:text-blue-900 border border-blue-700'}`}>{isAdminLoggedIn ? 'Dashboard' : 'Log Masuk Dashboard'}</button>
            </nav>
            <div className="md:hidden flex items-center">
              <button onClick={() => setIsMobileMenuOpen(!isMobileMenuOpen)} className="p-2 rounded-md text-blue-100 hover:text-white hover:bg-blue-800">{isMobileMenuOpen ? <X className="h-6 w-6" /> : <Menu className="h-6 w-6" />}</button>
            </div>
          </div>
        </div>
        {isMobileMenuOpen && (
          <div className="md:hidden bg-blue-800 border-t border-blue-700">
            <div className="px-2 pt-2 pb-3 space-y-1">
              {navItems.map((item) => <button key={item.id} onClick={() => navigateTo(item.id)} className="block w-full text-left px-3 py-3 rounded-md text-base font-medium text-blue-100">{item.label}</button>)}
              <button onClick={() => navigateTo('admin')} className="block w-full text-left px-3 py-3 mt-4 border-t border-blue-700 rounded-md text-base font-bold text-yellow-400">{isAdminLoggedIn ? 'Dashboard' : 'Log Masuk Dashboard'}</button>
            </div>
          </div>
        )}
      </header>

      <main className="flex-grow w-full">
        {currentPage === 'home' && renderHome()}
        {currentPage !== 'home' && (
          <div className="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-8 md:py-12">
            {currentPage === 'profil' && renderProfil()}
            {currentPage === 'direktori' && renderDirektori()}
            {currentPage === 'lokasi' && renderLokasi()}
            {currentPage === 'admin' && renderAdmin()}
          </div>
        )}
      </main>

      <footer className="bg-gray-900 text-gray-300 py-12 border-t-4 border-yellow-500">
        <div className="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
          <div className="grid grid-cols-1 md:grid-cols-3 gap-8">
            <div>
              <div className="flex items-center space-x-3 mb-4">
                <RisdaDriveLogo className="h-10 w-auto" showGlow={false} isSecond={true} />
                <RisdaDriveLogo className="h-9 w-auto" showGlow={true} isSecond={false} />
                <span className="font-bold text-lg text-white pl-2 border-l border-gray-700">RISDA PAHANG</span>
              </div>
              <p className="text-sm text-gray-400 leading-relaxed mb-4">Pihak Berkuasa Kemajuan Pekebun Kecil Perusahaan Getah Negeri Pahang. Menjulang martabat pekebun kecil melalui transformasi pertanian digital dan mampan.</p>
            </div>
            <div>
              <h3 className="text-white font-semibold mb-4 text-lg">Hubungi Kami</h3>
              <ul className="space-y-3 text-sm">
                <li className="flex items-start"><Building className="w-5 h-5 mr-3 text-gray-500 shrink-0" /><span>Tingkat 1, Blok A, Bangunan RISDA,<br/>Lot 7876, Jalan Haji Junid,<br/>25200 Kuantan, Pahang</span></li>
                <li className="flex items-center"><Phone className="w-5 h-5 mr-3 text-gray-500 shrink-0" /><span>09-514 1911 / 514 1912</span></li>
                <li className="flex items-center"><Mail className="w-5 h-5 mr-3 text-gray-500 shrink-0" /><span>risphg@risda.gov.my</span></li>
              </ul>
            </div>
          </div>
          <div className="border-t border-gray-800 mt-8 pt-8 text-sm text-center text-gray-500 flex flex-col md:flex-row justify-between items-center">
            <p>&copy; {new Date().getFullYear()} Pentadbiran RISDA Pahang. Hak Cipta Terpelihara.</p>
            <p className="mt-2 md:mt-0">Sistem Portal Korporat</p>
          </div>
        </div>
      </footer>
      
      {isAdminLoggedIn && (
        <a
          href="https://sites.google.com/risda.gov.my/pentadbiranrisdapahang/home"
          target="_blank"
          rel="noopener noreferrer"
          title="Buka Portal Pentadbiran RISDA Pahang"
          className="fixed bottom-6 left-6 z-50 flex items-center gap-2.5 bg-blue-900 hover:bg-blue-800 text-white px-4 py-2.5 rounded-full shadow-xl hover:shadow-2xl border-2 border-amber-400 group cursor-pointer transition-all duration-300"
        >
          <Globe className="w-5 h-5 text-amber-400 group-hover:rotate-12 transition-transform duration-300" />
          <span className="text-xs font-bold tracking-wide text-white">Portal Pentadbiran</span>
          <ExternalLink className="w-3.5 h-3.5 text-blue-200 group-hover:text-amber-300 transition-colors" />
        </a>
      )}
    </div>
  );
}
