import React, { useState, useEffect } from 'react';
import { 
  Truck, MapPin, Navigation, Clock, User, Bell, 
  CheckCircle, LogOut, Fuel, Gauge, ChevronRight, 
  Phone, MessageSquare, AlertTriangle, Menu, X,
  LayoutDashboard // <-- Ditambahkan ke import
} from 'lucide-react';

// --- MOCK DATA (Simulasi Koneksi ke Database MyTrading) ---
const DRIVER_PROFILE = {
  id: 1,
  name: "Ujang Caniago",
  truck: "BA 9021 QU",
  type: "Hino 500 (Dump Truck)",
  phone: "0812-3456-7890",
  photo: "https://i.pravatar.cc/150?u=a042581f4e29026024d"
};

const ACTIVE_ORDER = {
  id: "TM-2401001",
  status: "Hauling", // Scheduled, Loading, Hauling, Unloading, Completed
  origin: "Pit Tambang Sijunjung",
  destination: "Stockpile IKPP Perawang",
  item: "Batubara Cal 5800",
  weight: "28.000 Kg",
  distance: "45 km",
  eta: "13:30 WIB",
  timeline: [
    { time: "08:00", status: "Tiket Dibuat", done: true },
    { time: "08:30", status: "Loading Selesai", done: true },
    { time: "09:00", status: "Keluar Tambang", done: true },
    { time: "-", status: "Tiba di Pabrik", done: false },
  ]
};

const NOTIFICATIONS = [
  { id: 1, title: "Panggilan Dispatcher", msg: "Ujang, tolong update posisi sekarang.", time: "10 mnt lalu", read: false },
  { id: 2, title: "Info Rute", msg: "Hati-hati ada perbaikan jalan di KM 50.", time: "1 jam lalu", read: true },
];

export default function DriverApp() {
  const [activeTab, setActiveTab] = useState('home'); // home, order, inbox, profile
  const [orderStatus, setOrderStatus] = useState(ACTIVE_ORDER.status);
  const [showSOS, setShowSOS] = useState(false);

  // Fungsi Simulasi Update Status
  const handleUpdateStatus = () => {
    if (orderStatus === 'Hauling') setOrderStatus('Unloading');
    else if (orderStatus === 'Unloading') setOrderStatus('Completed');
    else setOrderStatus('Hauling');
  };

  return (
    <div className="flex flex-col h-screen bg-gray-50 font-sans max-w-md mx-auto shadow-2xl overflow-hidden border-x border-gray-200">
      
      {/* --- HEADER MOBILE --- */}
      <header className="bg-blue-600 text-white p-4 pt-6 shadow-md z-10 flex justify-between items-center">
        <div>
          <h1 className="text-lg font-bold tracking-tight">MyTrading <span className="font-light opacity-80">Driver</span></h1>
          <p className="text-xs text-blue-100 flex items-center gap-1">
            <span className="w-2 h-2 bg-green-400 rounded-full animate-pulse"></span> Online • {DRIVER_PROFILE.truck}
          </p>
        </div>
        <div className="flex gap-3">
           <button 
             onClick={() => setShowSOS(!showSOS)}
             className="bg-red-500 hover:bg-red-600 p-2 rounded-full shadow-lg transition-transform active:scale-95"
           >
             <AlertTriangle size={20} fill="white" className="text-white" />
           </button>
           <div className="relative">
             <Bell size={24} />
             {NOTIFICATIONS.some(n => !n.read) && <span className="absolute top-0 right-0 w-2.5 h-2.5 bg-red-500 border-2 border-blue-600 rounded-full"></span>}
           </div>
        </div>
      </header>

      {/* --- SOS MODAL --- */}
      {showSOS && (
        <div className="absolute inset-0 bg-black/80 z-50 flex items-center justify-center p-6 backdrop-blur-sm animate-in fade-in zoom-in">
          <div className="bg-white rounded-2xl p-6 w-full text-center space-y-4 shadow-2xl">
            <div className="bg-red-100 w-20 h-20 rounded-full flex items-center justify-center mx-auto mb-4 animate-pulse">
              <AlertTriangle size={40} className="text-red-600" />
            </div>
            <h2 className="text-2xl font-bold text-gray-900">DARURAT?</h2>
            <p className="text-gray-500">Tombol ini akan mengirim sinyal bahaya & lokasi terkini ke Dispatcher Pusat.</p>
            <div className="grid grid-cols-2 gap-3 pt-4">
              <button onClick={() => setShowSOS(false)} className="py-3 px-4 border border-gray-300 rounded-xl font-bold text-gray-600">Batal</button>
              <button className="py-3 px-4 bg-red-600 text-white rounded-xl font-bold shadow-lg shadow-red-200">KIRIM SOS</button>
            </div>
          </div>
        </div>
      )}

      {/* --- MAIN CONTENT SCROLLABLE --- */}
      <main className="flex-1 overflow-y-auto pb-20 custom-scrollbar">
        
        {/* VIEW: HOME */}
        {activeTab === 'home' && (
          <div className="p-4 space-y-4">
            {/* Status Card */}
            <div className="bg-white p-4 rounded-2xl shadow-sm border border-gray-100">
              <div className="flex items-center gap-4">
                <img src={DRIVER_PROFILE.photo} alt="Driver" className="w-14 h-14 rounded-full border-2 border-blue-100" />
                <div className="flex-1">
                  <h2 className="font-bold text-gray-800 text-lg">Halo, {DRIVER_PROFILE.name.split(' ')[0]}!</h2>
                  <p className="text-xs text-gray-500">Shift Pagi • 07:00 - 15:00</p>
                </div>
              </div>
              <div className="mt-4 grid grid-cols-2 gap-3">
                <div className="bg-blue-50 p-3 rounded-xl flex flex-col items-center">
                  <span className="text-xs text-blue-600 font-bold uppercase">Ritase Hari Ini</span>
                  <span className="text-2xl font-black text-blue-800">2</span>
                </div>
                <div className="bg-green-50 p-3 rounded-xl flex flex-col items-center">
                  <span className="text-xs text-green-600 font-bold uppercase">Performa</span>
                  <span className="text-2xl font-black text-green-800">98%</span>
                </div>
              </div>
            </div>

            {/* Quick Actions (Telematika) */}
            <div className="grid grid-cols-2 gap-3">
               <button className="bg-white p-3 rounded-xl border border-gray-200 shadow-sm flex items-center gap-3 active:bg-gray-50">
                  <div className="bg-orange-100 p-2 rounded-lg text-orange-600"><Fuel size={20}/></div>
                  <div className="text-left">
                    <p className="text-[10px] text-gray-400 font-bold uppercase">Input BBM</p>
                    <p className="text-sm font-bold text-gray-700">Update</p>
                  </div>
               </button>
               <button className="bg-white p-3 rounded-xl border border-gray-200 shadow-sm flex items-center gap-3 active:bg-gray-50">
                  <div className="bg-purple-100 p-2 rounded-lg text-purple-600"><Gauge size={20}/></div>
                  <div className="text-left">
                    <p className="text-[10px] text-gray-400 font-bold uppercase">Odometer</p>
                    <p className="text-sm font-bold text-gray-700">Update</p>
                  </div>
               </button>
            </div>

            {/* Active Order Banner */}
            <div className="bg-slate-800 text-white p-5 rounded-2xl shadow-lg relative overflow-hidden group cursor-pointer" onClick={() => setActiveTab('order')}>
              <div className="absolute right-0 top-0 w-32 h-32 bg-white/5 rounded-full -mr-10 -mt-10 blur-xl"></div>
              <div className="flex justify-between items-start mb-4 relative z-10">
                <div>
                  <p className="text-xs text-slate-400 font-bold uppercase mb-1">Tugas Sekarang</p>
                  <h3 className="font-bold text-xl">Hauling Batubara</h3>
                </div>
                <span className="bg-green-500 text-slate-900 text-[10px] font-bold px-2 py-1 rounded">ON GOING</span>
              </div>
              <div className="space-y-3 relative z-10">
                <div className="flex items-center gap-3">
                  <div className="w-2 h-2 bg-white rounded-full"></div>
                  <p className="text-sm font-medium opacity-90">{ACTIVE_ORDER.origin}</p>
                </div>
                <div className="h-4 border-l border-dashed border-slate-600 ml-1"></div>
                <div className="flex items-center gap-3">
                  <div className="w-2 h-2 border-2 border-white rounded-full"></div>
                  <p className="text-sm font-medium opacity-90">{ACTIVE_ORDER.destination}</p>
                </div>
              </div>
              <div className="mt-4 pt-3 border-t border-slate-700 flex justify-between items-center relative z-10">
                 <p className="text-xs text-slate-400">Jarak: {ACTIVE_ORDER.distance}</p>
                 <ChevronRight size={16} className="text-white"/>
              </div>
            </div>
          </div>
        )}

        {/* VIEW: ACTIVE ORDER DETAILS */}
        {activeTab === 'order' && (
          <div className="p-4 space-y-5">
            <div className="bg-white rounded-2xl shadow-sm border border-gray-200 overflow-hidden">
              {/* Map Placeholder */}
              <div className="h-40 bg-slate-200 relative w-full group">
                 <div className="absolute inset-0 flex items-center justify-center text-slate-400">
                    <MapPin size={48} className="opacity-20"/>
                 </div>
                 {/* Fake Route Line */}
                 <svg className="absolute inset-0 w-full h-full pointer-events-none">
                    <path d="M 50 120 Q 150 80 300 50" fill="none" stroke="#3b82f6" strokeWidth="4" strokeDasharray="8 4" className="animate-pulse"/>
                    <circle cx="50" cy="120" r="6" fill="#10b981" />
                    <circle cx="300" cy="50" r="6" fill="#ef4444" />
                 </svg>
                 <button className="absolute bottom-3 right-3 bg-white p-2 rounded-lg shadow-md text-blue-600 font-bold text-xs flex items-center gap-1">
                    <Navigation size={14}/> Buka Maps
                 </button>
              </div>
              
              <div className="p-5">
                <div className="flex justify-between items-end mb-4">
                   <div>
                      <p className="text-xs text-gray-500 font-bold uppercase">No. Tiket</p>
                      <h2 className="text-2xl font-black text-gray-800">{ACTIVE_ORDER.id}</h2>
                   </div>
                   <div className="text-right">
                      <p className="text-xs text-gray-500">Estimasi Tiba</p>
                      <p className="text-lg font-bold text-green-600">{ACTIVE_ORDER.eta}</p>
                   </div>
                </div>

                <div className="space-y-4">
                   <div className="bg-gray-50 p-3 rounded-xl border border-gray-100">
                      <div className="flex items-start gap-3">
                         <Truck className="text-gray-400 mt-1" size={18}/>
                         <div>
                            <p className="text-xs text-gray-400 font-bold uppercase">Muatan</p>
                            <p className="text-sm font-bold text-gray-700">{ACTIVE_ORDER.item}</p>
                            <p className="text-xs text-gray-500">Netto: {ACTIVE_ORDER.weight}</p>
                         </div>
                      </div>
                   </div>

                   {/* Timeline */}
                   <div className="relative pl-2 space-y-4 pt-2">
                      <div className="absolute left-2.5 top-2 bottom-2 w-0.5 bg-gray-200"></div>
                      {ACTIVE_ORDER.timeline.map((log, idx) => (
                        <div key={idx} className="flex gap-4 relative">
                           <div className={`w-3 h-3 rounded-full mt-1.5 z-10 ${log.done ? 'bg-blue-600 ring-4 ring-blue-50' : 'bg-gray-300'}`}></div>
                           <div className="flex-1 flex justify-between items-center">
                              <p className={`text-sm ${log.done ? 'font-bold text-gray-800' : 'text-gray-400'}`}>{log.status}</p>
                              <p className="text-xs text-gray-400">{log.time}</p>
                           </div>
                        </div>
                      ))}
                   </div>
                </div>
              </div>
            </div>

            {/* Action Slider Button */}
            <div className="pb-4">
               <button 
                 onClick={handleUpdateStatus}
                 className={`w-full py-4 rounded-xl shadow-lg shadow-blue-200 text-white font-bold text-lg flex items-center justify-center gap-3 transition-all active:scale-95 ${
                   orderStatus === 'Hauling' ? 'bg-blue-600 hover:bg-blue-700' : 
                   orderStatus === 'Unloading' ? 'bg-orange-500 hover:bg-orange-600' : 'bg-green-600 hover:bg-green-700'
                 }`}
               >
                 {orderStatus === 'Hauling' && <><Navigation/> Tiba di Lokasi</>}
                 {orderStatus === 'Unloading' && <><Truck/> Selesai Bongkar</>}
                 {orderStatus === 'Completed' && <><CheckCircle/> Tugas Selesai</>}
               </button>
               <p className="text-center text-xs text-gray-400 mt-3">Tekan tombol saat status operasional berubah</p>
            </div>
          </div>
        )}

        {/* VIEW: INBOX */}
        {activeTab === 'inbox' && (
          <div className="p-4 space-y-3">
            <h2 className="font-bold text-lg text-gray-800 mb-2">Pesan Masuk</h2>
            {NOTIFICATIONS.map(notif => (
              <div key={notif.id} className={`bg-white p-4 rounded-xl border shadow-sm flex gap-4 ${notif.read ? 'border-gray-100 opacity-80' : 'border-blue-100 bg-blue-50/30'}`}>
                 <div className={`p-3 rounded-full h-fit ${notif.read ? 'bg-gray-100 text-gray-400' : 'bg-blue-100 text-blue-600'}`}>
                    <MessageSquare size={20} />
                 </div>
                 <div className="flex-1">
                    <div className="flex justify-between items-start mb-1">
                       <h4 className={`text-sm ${notif.read ? 'font-semibold text-gray-700' : 'font-bold text-blue-800'}`}>{notif.title}</h4>
                       <span className="text-[10px] text-gray-400">{notif.time}</span>
                    </div>
                    <p className="text-xs text-gray-600 leading-relaxed">{notif.msg}</p>
                 </div>
              </div>
            ))}
            <div className="text-center pt-8">
               <p className="text-xs text-gray-400">Tidak ada pesan lainnya.</p>
            </div>
          </div>
        )}

      </main>

      {/* --- BOTTOM NAVIGATION --- */}
      <nav className="bg-white border-t border-gray-200 px-6 py-3 flex justify-between items-center z-20 pb-safe">
        <NavButton icon={<LayoutDashboard size={22}/>} label="Home" active={activeTab === 'home'} onClick={() => setActiveTab('home')} />
        <NavButton icon={<Navigation size={22}/>} label="Jalan" active={activeTab === 'order'} onClick={() => setActiveTab('order')} />
        <div className="relative">
           <NavButton icon={<MessageSquare size={22}/>} label="Pesan" active={activeTab === 'inbox'} onClick={() => setActiveTab('inbox')} />
           {NOTIFICATIONS.some(n => !n.read) && <span className="absolute top-0 right-3 w-2 h-2 bg-red-500 rounded-full"></span>}
        </div>
        <NavButton icon={<User size={22}/>} label="Profil" active={activeTab === 'profile'} onClick={() => setActiveTab('profile')} />
      </nav>

      {/* Global Styles for Mobile */}
      <style>{`
        .pb-safe { padding-bottom: env(safe-area-inset-bottom); }
        .custom-scrollbar::-webkit-scrollbar { width: 0px; background: transparent; }
      `}</style>
    </div>
  );
}

// --- SUB COMPONENTS ---

function NavButton({ icon, label, active, onClick }) {
  return (
    <button 
      onClick={onClick}
      className={`flex flex-col items-center gap-1 transition-colors ${active ? 'text-blue-600' : 'text-gray-400 hover:text-gray-600'}`}
    >
      {React.cloneElement(icon, { fill: active ? "currentColor" : "none", className: active ? "transform scale-110 transition" : "" })}
      <span className="text-[10px] font-medium">{label}</span>
    </button>
  );
}
