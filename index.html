<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Rasheed: COE Academic Assistant</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <script src="https://unpkg.com/react@18/umd/react.production.min.js" crossorigin></script>
    <script src="https://unpkg.com/react-dom@18/umd/react-dom.production.min.js" crossorigin></script>
    <script src="https://unpkg.com/@babel/standalone/babel.min.js"></script>
    <script src="https://unpkg.com/lucide@latest"></script>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Inter:wght@400;600;800;900&display=swap');
        body { font-family: 'Inter', sans-serif; background-color: #f8fafc; }
        .checklist-scroll::-webkit-scrollbar { width: 6px; }
        .checklist-scroll::-webkit-scrollbar-thumb { background: #D71920; border-radius: 10px; }
        [v-cloak] { display: none; }
    </style>
</head>
<body>
    <div id="root">
        <div class="flex items-center justify-center min-h-screen">
            <div class="text-center">
                <div class="w-12 h-12 border-4 border-[#D71920] border-t-transparent rounded-full animate-spin mx-auto mb-4"></div>
                <p class="text-slate-400 font-bold uppercase tracking-widest text-xs">Initializing Rasheed...</p>
            </div>
        </div>
    </div>

    <script type="text/babel">
        const { useState, useMemo, useEffect } = React;

        const COE_DATA = {
            majors: [
                {
                    id: "ece",
                    name: "Early Childhood Education",
                    cohorts: ["2025-2026"],
                    plans: {
                        "2025-2026": [
                            { term: 1, courses: [
                                { code: "GEIT113", name: "Intro to AI", ch: 3, type: "GenEd" },
                                { code: "GESU121", name: "Sustainability", ch: 3, type: "GenEd" },
                                { code: "GEEM110", name: "Contemporary Emirati Studies", ch: 3, type: "GenEd" },
                                { code: "GEAE101", name: "Academic English", ch: 3, type: "GenEd" }
                            ]},
                            { term: 2, courses: [
                                { code: "SPED101", name: "Education of Exceptional Children", ch: 3, type: "Core" },
                                { code: "CURR101", name: "Technology in Education", ch: 3, type: "Core" },
                                { code: "FOED102", name: "Professional Ethics", ch: 3, type: "Core" },
                                { code: "CURR233", name: "Classroom Management", ch: 3, type: "Core" }
                            ]}
                        ]
                    }
                },
                {
                    id: "hpe",
                    name: "Health and Physical Education",
                    cohorts: ["2025-2026"],
                    plans: {
                        "2025-2026": [
                            { term: 1, courses: [
                                { code: "GEEM110", name: "Emirati Studies", ch: 3, type: "GenEd" },
                                { code: "GEAE101", name: "Academic English", ch: 3, type: "GenEd" }
                            ]}
                        ]
                    }
                }
            ]
        };

        function App() {
            const [major, setMajor] = useState(null);
            const [cohort, setCohort] = useState("");
            const [completed, setCompleted] = useState({});
            const [showSummer, setShowSummer] = useState(false);
            const [showNext, setShowNext] = useState(false);
            const [showLong, setShowLong] = useState(false);

            useEffect(() => {
                if (window.lucide) {
                    window.lucide.createIcons();
                }
            });

            const plan = useMemo(() => {
                if (!major || !cohort) return [];
                return major.plans[cohort] || [];
            }, [major, cohort]);

            const allCourses = useMemo(() => plan.flatMap(p => p.courses), [plan]);
            const earnedCH = useMemo(() => allCourses.filter(c => completed[c.code]).reduce((sum, c) => sum + 3, 0), [allCourses, completed]);

            const registrationWindows = useMemo(() => {
                let summer = "April 09, 2026";
                let fall = "April 20 - 21, 2026";
                if (earnedCH >= 99) summer = "April 06, 2026";
                else if (earnedCH >= 81) summer = "April 07, 2026";
                if (earnedCH >= 84) fall = "April 13 - 14, 2026";
                else if (earnedCH >= 45) fall = "April 14 - 15, 2026";
                return { summer, fall };
            }, [earnedCH]);

            const remainingCourses = allCourses.filter(c => !completed[c.code]);

            return (
                <div className="min-h-screen">
                    <header className="bg-[#D71920] text-white p-6 shadow-lg sticky top-0 z-50 flex justify-between items-center">
                        <div className="flex items-center gap-3">
                            <i data-lucide="graduation-cap" className="w-8 h-8"></i>
                            <div>
                                <h1 className="text-2xl font-black tracking-tight leading-none">Rasheed</h1>
                                <p className="text-[10px] uppercase font-bold opacity-80 mt-1">COE Academic Assistant</p>
                            </div>
                        </div>
                    </header>

                    <main className="max-w-4xl mx-auto p-6 space-y-6">
                        <section className="bg-white rounded-3xl p-8 shadow-sm border-2 border-slate-100">
                            <div className="flex items-start gap-5">
                                <div className="bg-[#D71920]/10 p-4 rounded-2xl shrink-0">
                                    <i data-lucide="sparkles" className="text-[#D71920] w-8 h-8"></i>
                                </div>
                                <div className="space-y-3">
                                    <h2 className="text-2xl font-black text-slate-900 tracking-tight">Welcome, Future Educator!</h2>
                                    <p className="text-slate-600 leading-relaxed italic">
                                        "I am Rasheed, your dedicated AI Academic Advisor. Let's optimize your path to graduation."
                                    </p>
                                </div>
                            </div>
                        </section>

                        <div className="bg-white rounded-3xl p-6 border-2 border-slate-100 grid grid-cols-1 md:grid-cols-2 gap-4">
                            <select onChange={(e) => {
                                setMajor(COE_DATA.majors.find(x => x.id === e.target.value));
                                setCohort(""); setCompleted({});
                            }} className="p-4 bg-slate-50 border-2 rounded-2xl font-bold outline-none">
                                <option value="">Select Major...</option>
                                {COE_DATA.majors.map(m => <option key={m.id} value={m.id}>{m.name}</option>)}
                            </select>
                            <select disabled={!major} onChange={(e) => setCohort(e.target.value)} value={cohort} className="p-4 bg-slate-50 border-2 rounded-2xl font-bold outline-none disabled:opacity-50">
                                <option value="">Select Cohort...</option>
                                {major?.cohorts.map(c => <option key={c} value={c}>{c}</option>)}
                            </select>
                        </div>

                        {major && cohort && (
                            <div className="space-y-6">
                                <section className="bg-white rounded-3xl border-2 border-slate-100 overflow-hidden shadow-sm">
                                    <div className="bg-slate-50 p-6 border-b flex justify-between items-center">
                                        <h3 className="font-black text-slate-800">Check Progress</h3>
                                        <div className="bg-[#D71920] text-white px-5 py-2 rounded-2xl text-sm font-black">{earnedCH} Credits</div>
                                    </div>
                                    <div className="p-4 max-h-[300px] overflow-y-auto space-y-2 checklist-scroll">
                                        {allCourses.map(c => (
                                            <div key={c.code} onClick={() => setCompleted(prev => ({...prev, [c.code]: !prev[c.code]}))} className={`p-4 rounded-xl cursor-pointer border-2 flex items-center gap-4 ${completed[c.code] ? 'bg-green-50 border-green-200' : 'bg-white border-slate-50'}`}>
                                                <i data-lucide="check" className={completed[c.code] ? 'text-green-500' : 'text-transparent'}></i>
                                                <div className="flex-1">
                                                    <span className="text-sm font-bold block">{c.name}</span>
                                                    <span className="text-[10px] font-black text-slate-400 uppercase">{c.code}</span>
                                                </div>
                                            </div>
                                        ))}
                                    </div>
                                </section>

                                <button onClick={() => setShowSummer(!showSummer)} className="w-full p-5 bg-white rounded-2xl border-2 font-black text-slate-700 flex justify-between items-center">
                                    <span>Summer 2026 Suggestions</span> <i data-lucide="sun" className="text-orange-400"></i>
                                </button>
                                {showSummer && (
                                    <div className="p-6 bg-white rounded-3xl border-2 border-orange-100 grid grid-cols-1 sm:grid-cols-2 gap-3">
                                        {remainingCourses.slice(0, 2).map(c => (
                                            <div key={c.code} className="bg-orange-50/50 p-3 rounded-xl border text-xs font-bold text-slate-700 uppercase">• {c.name}</div>
                                        ))}
                                    </div>
                                )}

                                <button onClick={() => setShowNext(!showNext)} className="w-full p-5 bg-white rounded-2xl border-2 font-black text-slate-700 flex justify-between items-center">
                                    <span>Next Term Plan (Fall 2026)</span> <i data-lucide="calendar" className="text-blue-400"></i>
                                </button>
                                {showNext && (
                                    <div className="p-6 bg-white rounded-3xl border-2 border-blue-100 space-y-2">
                                        {remainingCourses.slice(0, 5).map(c => (
                                            <div key={c.code} className="p-4 bg-blue-50/50 rounded-xl flex justify-between text-xs font-bold"><span>{c.name}</span><span className="text-blue-400">{c.code}</span></div>
                                        ))}
                                    </div>
                                )}

                                <div className="bg-slate-900 rounded-[2.5rem] p-8 text-white space-y-6 shadow-xl relative overflow-hidden border-4 border-white">
                                    <h3 className="text-xl font-black text-[#D71920] flex items-center gap-2">
                                        <i data-lucide="clock"></i> Registration Window
                                    </h3>
                                    <div className="grid grid-cols-1 md:grid-cols-2 gap-6">
                                        <div className="p-6 bg-white/5 rounded-3xl border border-white/10">
                                            <p className="text-[10px] uppercase font-black tracking-widest text-orange-400 mb-2">Summer 2026</p>
                                            <p className="text-3xl font-black text-white">{registrationWindows.summer}</p>
                                        </div>
                                        <div className="p-6 bg-white/5 rounded-3xl border border-white/10">
                                            <p className="text-[10px] uppercase font-black tracking-widest text-blue-400 mb-2">Fall 2026</p>
                                            <p className="text-3xl font-black text-white">{registrationWindows.fall}</p>
                                        </div>
                                    </div>
                                </div>
                            </div>
                        )}
                    </main>
                </div>
            );
        }

        const root = ReactDOM.createRoot(document.getElementById('root'));
        root.render(<App />);
    </script>
</body>
</html>
