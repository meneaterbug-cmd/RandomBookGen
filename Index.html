<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Random Book</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <script src="https://unpkg.com/react@18/umd/react.production.min.js"></script>
    <script src="https://unpkg.com/react-dom@18/umd/react-dom.production.min.js"></script>
    <script src="https://unpkg.com/@babel/standalone/babel.min.js"></script>
    <style>
        /* Prevents pull-to-refresh on mobile devices */
        body { overscroll-behavior-y: none; background-color: #f3f4f6; }
        .hide-scrollbar::-webkit-scrollbar { display: none; }
        .hide-scrollbar { -ms-overflow-style: none; scrollbar-width: none; }
    </style>
</head>
<body>
    <div id="root"></div>

    <script type="text/babel">
        const { useState } = React;

        // Icons as simple SVG components
        const BookIcon = () => <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" strokeWidth="2" strokeLinecap="round" strokeLinejoin="round"><path d="M4 19.5v-15A2.5 2.5 0 0 1 6.5 2H20v20H6.5a2.5 2.5 0 0 1 0-5H20"/></svg>;
        const SettingsIcon = () => <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" strokeWidth="2" strokeLinecap="round" strokeLinejoin="round"><circle cx="12" cy="12" r="3"/><path d="M19.4 15a1.65 1.65 0 0 0 .33 1.82l.06.06a2 2 0 0 1 0 2.83 2 2 0 0 1-2.83 0l-.06-.06a1.65 1.65 0 0 0-1.82-.33 1.65 1.65 0 0 0-1 1.51V21a2 2 0 0 1-2 2 2 2 0 0 1-2-2v-.09A1.65 1.65 0 0 0 9 19.4a1.65 1.65 0 0 0-1.82.33l-.06.06a2 2 0 0 1-2.83 0 2 2 0 0 1 0-2.83l.06-.06a1.65 1.65 0 0 0 .33-1.82 1.65 1.65 0 0 0-1.51-1H3a2 2 0 0 1-2-2 2 2 0 0 1 2-2h.09A1.65 1.65 0 0 0 4.6 9a1.65 1.65 0 0 0-.33-1.82l-.06-.06a2 2 0 0 1 0-2.83 2 2 0 0 1 2.83 0l.06.06a1.65 1.65 0 0 0 1.82.33H9a1.65 1.65 0 0 0 1-1.51V3a2 2 0 0 1 2-2 2 2 0 0 1 2 2v.09a1.65 1.65 0 0 0 1 1.51 1.65 1.65 0 0 0 1.82-.33l.06-.06a2 2 0 0 1 2.83 0 2 2 0 0 1 0 2.83l-.06.06a1.65 1.65 0 0 0-.33 1.82V9a1.65 1.65 0 0 0 1.51 1H21a2 2 0 0 1 2 2 2 2 0 0 1-2 2h-.09a1.65 1.65 0 0 0-1.51 1z"/></svg>;
        const DicesIcon = () => <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" strokeWidth="2" strokeLinecap="round" strokeLinejoin="round"><rect width="12" height="12" x="2" y="10" rx="2" ry="2"/><path d="m17.92 14 3.5-3.5a2.24 2.24 0 0 0 0-3l-5-4.92a2.24 2.24 0 0 0-3 0L10 6"/><path d="M6 18h.01"/><path d="M10 14h.01"/><path d="M15 6h.01"/><path d="M18 9h.01"/></svg>;
        const AlertCircleIcon = () => <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" strokeWidth="2" strokeLinecap="round" strokeLinejoin="round"><circle cx="12" cy="12" r="10"/><line x1="12" y1="8" x2="12" y2="12"/><line x1="12" y1="16" x2="12.01" y2="16"/></svg>;
        const CheckIcon = () => <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" strokeWidth="3" strokeLinecap="round" strokeLinejoin="round"><polyline points="20 6 9 17 4 12"/></svg>;
        const XIcon = () => <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" strokeWidth="3" strokeLinecap="round" strokeLinejoin="round"><line x1="18" y1="6" x2="6" y2="18"/><line x1="6" y1="6" x2="18" y2="18"/></svg>;

        const GENRES = [
            // Original 8
            { id: 'fantasy', label: 'Fantasy' },
            { id: 'science_fiction', label: 'Sci-Fi' },
            { id: 'thriller', label: 'Thriller' },
            { id: 'romance', label: 'Romance' },
            { id: 'horror', label: 'Horror' },
            { id: 'mystery', label: 'Mystery' },
            { id: 'historical_fiction', label: 'Historical' },
            { id: 'biography', label: 'Biography' },
            // New 20
            { id: 'adventure', label: 'Adventure' },
            { id: 'young_adult', label: 'Young Adult' },
            { id: 'children', label: 'Children' },
            { id: 'poetry', label: 'Poetry' },
            { id: 'humor', label: 'Humor' },
            { id: 'true_crime', label: 'True Crime' },
            { id: 'dystopia', label: 'Dystopia' },
            { id: 'travel', label: 'Travel' },
            { id: 'cooking', label: 'Cooking' },
            { id: 'art', label: 'Art' },
            { id: 'philosophy', label: 'Philosophy' },
            { id: 'psychology', label: 'Psychology' },
            { id: 'business', label: 'Business' },
            { id: 'history', label: 'History' },
            { id: 'religion', label: 'Religion' },
            { id: 'science', label: 'Science' },
            { id: 'sports', label: 'Sports' },
            { id: 'music', label: 'Music' },
            { id: 'nature', label: 'Nature' },
            { id: 'self_help', label: 'Self-Help' }
        ];

        function App() {
            const [includedGenres, setIncludedGenres] = useState(['fantasy', 'science_fiction']);
            const [excludedGenres, setExcludedGenres] = useState(['romance']);
            const [language, setLanguage] = useState('eng'); // 'ger', 'eng', 'both'
            
            const [book, setBook] = useState(null);
            const [loading, setLoading] = useState(false);
            const [error, setError] = useState(null);
            const [showConfig, setShowConfig] = useState(true);
            const [imageError, setImageError] = useState(false);
            
            // Cache to avoid refetching on every click
            const [cachedBooks, setCachedBooks] = useState([]);

            const toggleGenre = (genreId, listType) => {
                if (listType === 'include') {
                    setIncludedGenres(prev => 
                        prev.includes(genreId) ? prev.filter(id => id !== genreId) : [...prev, genreId]
                    );
                    setExcludedGenres(prev => prev.filter(id => id !== genreId));
                } else {
                    setExcludedGenres(prev => 
                        prev.includes(genreId) ? prev.filter(id => id !== genreId) : [...prev, genreId]
                    );
                    setIncludedGenres(prev => prev.filter(id => id !== genreId));
                }
                setCachedBooks([]);
            };

            const buildQuery = () => {
                let parts = [];
                
                if (includedGenres.length > 0) {
                    const inc = includedGenres.map(g => `subject:${g}`).join(' OR ');
                    parts.push(`(${inc})`);
                } else {
                    parts.push('subject:book');
                }

                if (excludedGenres.length > 0) {
                    const exc = excludedGenres.map(g => `-subject:${g}`).join(' AND ');
                    parts.push(`(${exc})`);
                }

                if (language === 'ger') {
                    parts.push('language:ger');
                } else if (language === 'eng') {
                    parts.push('language:eng');
                } else {
                    parts.push('(language:ger OR language:eng)');
                }

                return parts.join(' AND ');
            };

            const fetchBooks = async () => {
                setLoading(true);
                setError(null);
                
                try {
                    const query = buildQuery();
                    const randomPage = Math.floor(Math.random() * 3) + 1;
                    const url = `https://openlibrary.org/search.json?q=${encodeURIComponent(query)}&limit=50&page=${randomPage}`;
                    
                    const response = await fetch(url);
                    if (!response.ok) throw new Error('Network error during API fetch.');
                    
                    const data = await response.json();
                    
                    if (!data.docs || data.docs.length === 0) {
                        if (randomPage > 1) {
                            const fallbackUrl = `https://openlibrary.org/search.json?q=${encodeURIComponent(query)}&limit=50&page=1`;
                            const fallbackResp = await fetch(fallbackUrl);
                            if (!fallbackResp.ok) throw new Error('Network error during fallback API fetch.');
                            const fallbackData = await fallbackResp.json();
                            if (!fallbackData.docs || fallbackData.docs.length === 0) {
                                throw new Error('No books found. Please adjust your filters.');
                            }
                            return fallbackData.docs;
                        }
                        throw new Error('No books found. Please adjust your filters.');
                    }
                    
                    return data.docs;
                } catch (err) {
                    setError(err.message);
                    return null;
                } finally {
                    setLoading(false);
                }
            };

            const generateRandomBook = async () => {
                setShowConfig(false);
                let availableBooks = [...cachedBooks];

                if (availableBooks.length === 0) {
                    const fetched = await fetchBooks();
                    if (!fetched) return;
                    
                    // Shuffle the fetched books
                    for (let i = fetched.length - 1; i > 0; i--) {
                        const j = Math.floor(Math.random() * (i + 1));
                        [fetched[i], fetched[j]] = [fetched[j], fetched[i]];
                    }
                    availableBooks = fetched;
                }

                if (availableBooks.length > 0) {
                    const selectedBook = availableBooks.pop();
                    setImageError(false);
                    setBook(selectedBook);
                    setCachedBooks(availableBooks);
                }
            };

            return (
                <div className="min-h-screen flex flex-col max-w-md mx-auto bg-white shadow-xl overflow-hidden relative">
                    
                    {/* Header */}
                    <header className="bg-indigo-600 text-white p-4 flex justify-between items-center shadow-md z-10 relative">
                        <div className="flex items-center gap-2">
                            <BookIcon />
                            <h1 className="font-bold text-xl tracking-tight">BookRandomizer</h1>
                        </div>
                        <button 
                            onClick={() => setShowConfig(!showConfig)}
                            className="p-2 rounded-full hover:bg-indigo-700 transition"
                            aria-label="Settings"
                        >
                            <SettingsIcon />
                        </button>
                    </header>

                    {/* Content Area */}
                    <main className="flex-1 overflow-y-auto hide-scrollbar pb-24 bg-gray-50">
                        
                        {/* Config Panel */}
                        {showConfig && (
                            <div className="p-5 bg-white border-b border-gray-200 shadow-sm transition-all duration-300">
                                
                                {/* Language */}
                                <div className="mb-6">
                                    <h2 className="text-sm font-semibold text-gray-700 mb-3 uppercase tracking-wider">Language</h2>
                                    <div className="flex bg-gray-100 p-1 rounded-lg">
                                        {['ger', 'eng', 'both'].map(l => (
                                            <button
                                                key={l}
                                                onClick={() => { setLanguage(l); setCachedBooks([]); }}
                                                className={`flex-1 py-2 text-sm font-medium rounded-md transition ${language === l ? 'bg-white shadow-sm text-indigo-600' : 'text-gray-500 hover:text-gray-700'}`}
                                            >
                                                {l === 'ger' ? 'German' : l === 'eng' ? 'English' : 'Both'}
                                            </button>
                                        ))}
                                    </div>
                                </div>

                                {/* Genres Include/Exclude */}
                                <div>
                                    <h2 className="text-sm font-semibold text-gray-700 mb-3 uppercase tracking-wider">Genres</h2>
                                    <p className="text-xs text-gray-500 mb-3">Tap once for "Must include" <span className="text-green-600 font-bold">(+)</span>, twice for "Exclude" <span className="text-red-600 font-bold">(-)</span>.</p>
                                    
                                    {/* The container wraps the numerous buttons automatically using flex-wrap */}
                                    <div className="flex flex-wrap gap-2 max-h-60 overflow-y-auto hide-scrollbar pb-2">
                                        {GENRES.map(genre => {
                                            const isIncluded = includedGenres.includes(genre.id);
                                            const isExcluded = excludedGenres.includes(genre.id);
                                            
                                            let btnClass = "bg-gray-100 text-gray-600 border border-transparent";
                                            let Icon = null;

                                            if (isIncluded) {
                                                btnClass = "bg-green-50 text-green-700 border-green-200 shadow-sm";
                                                Icon = CheckIcon;
                                            } else if (isExcluded) {
                                                btnClass = "bg-red-50 text-red-700 border-red-200 shadow-sm";
                                                Icon = XIcon;
                                            }

                                            return (
                                                <button
                                                    key={genre.id}
                                                    onClick={() => {
                                                        if (!isIncluded && !isExcluded) toggleGenre(genre.id, 'include');
                                                        else if (isIncluded) toggleGenre(genre.id, 'exclude');
                                                        else {
                                                            setExcludedGenres(prev => prev.filter(id => id !== genre.id));
                                                            setCachedBooks([]);
                                                        }
                                                    }}
                                                    className={`px-3 py-2 rounded-full text-sm font-medium flex items-center gap-1 transition-all active:scale-95 ${btnClass}`}
                                                >
                                                    {Icon && <Icon />}
                                                    {genre.label}
                                                </button>
                                            )
                                        })}
                                    </div>
                                    {includedGenres.length === 0 && (
                                        <p className="text-xs text-amber-600 mt-3 flex items-center gap-1">
                                            <AlertCircleIcon /> Please select at least one genre.
                                        </p>
                                    )}
                                </div>
                            </div>
                        )}

                        {/* Display Book */}
                        <div className="p-5 flex flex-col items-center justify-center min-h-[50vh]">
                            {loading ? (
                                <div className="flex flex-col items-center text-indigo-600 animate-pulse">
                                    <DicesIcon className="w-12 h-12 mb-4 animate-spin" style={{ animationDuration: '3s' }}/>
                                    <p className="font-medium">Searching the library...</p>
                                </div>
                            ) : error ? (
                                <div className="text-center p-6 bg-red-50 rounded-2xl border border-red-100">
                                    <AlertCircleIcon className="w-10 h-10 text-red-500 mx-auto mb-3" />
                                    <p className="text-red-700 font-medium">{error}</p>
                                </div>
                            ) : book ? (
                                <div className="w-full bg-white rounded-3xl shadow-lg border border-gray-100 overflow-hidden transform transition-all">
                                    {/* Cover Image Area */}
                                    <div className="bg-gray-100 w-full aspect-[2/3] relative flex items-center justify-center">
                                        {book.cover_i && !imageError ? (
                                            <img 
                                                src={`https://covers.openlibrary.org/b/id/${book.cover_i}-L.jpg`} 
                                                alt={`Cover of ${book.title}`}
                                                className="w-full h-full object-cover"
                                                onError={() => setImageError(true)}
                                            />
                                        ) : null}
                                        <div className={`absolute inset-0 flex flex-col items-center justify-center text-gray-400 p-6 text-center ${(!book.cover_i || imageError) ? 'flex' : 'hidden'}`}>
                                            <BookIcon className="w-16 h-16 mb-2 opacity-50" />
                                            <span className="text-sm">No cover found in Open Library</span>
                                        </div>
                                    </div>
                                    
                                    {/* Book Details */}
                                    <div className="p-6 text-center">
                                        <h2 className="text-2xl font-bold text-gray-900 mb-2 leading-tight">
                                            {book.title}
                                        </h2>
                                        <p className="text-lg text-indigo-600 font-medium mb-4">
                                            {book.author_name ? [].concat(book.author_name).join(', ') : 'Unknown Author'}
                                        </p>
                                        
                                        <div className="flex flex-wrap justify-center gap-2 mb-4">
                                            {book.first_publish_year && (
                                                <span className="bg-gray-100 text-gray-600 text-xs px-2 py-1 rounded">
                                                    First published: {book.first_publish_year}
                                                </span>
                                            )}
                                            {Array.isArray(book.language) && book.language.includes('eng') && (
                                                <span className="bg-gray-100 text-gray-600 text-xs px-2 py-1 rounded">EN</span>
                                            )}
                                            {Array.isArray(book.language) && book.language.includes('ger') && (
                                                <span className="bg-gray-100 text-gray-600 text-xs px-2 py-1 rounded">DE</span>
                                            )}
                                        </div>
                                        
                                        <a 
                                            href={`https://openlibrary.org${book.key}`} 
                                            target="_blank" 
                                            rel="noopener noreferrer"
                                            className="text-sm text-gray-500 underline decoration-gray-300 hover:text-indigo-600"
                                        >
                                            View on Open Library
                                        </a>
                                    </div>
                                </div>
                            ) : (
                                !showConfig && (
                                    <div className="text-center text-gray-400">
                                        <BookIcon className="w-16 h-16 mx-auto mb-4 opacity-20" />
                                        <p>Tap below to generate your first book!</p>
                                    </div>
                                )
                            )}
                        </div>
                    </main>

                    {/* Bottom Action Area (Sticky) */}
                    <div className="absolute bottom-0 w-full p-4 bg-gradient-to-t from-white via-white to-transparent pb-[calc(1rem+env(safe-area-inset-bottom))]">
                        <button 
                            onClick={generateRandomBook}
                            disabled={loading || includedGenres.length === 0}
                            className="w-full bg-indigo-600 text-white font-bold text-lg py-4 px-6 rounded-2xl shadow-lg shadow-indigo-200 active:scale-95 transition-all flex items-center justify-center gap-2 disabled:opacity-50 disabled:active:scale-100"
                        >
                            <DicesIcon />
                            {book ? 'Another book!' : 'Find a random book'}
                        </button>
                    </div>

                </div>
            );
        }

        const root = ReactDOM.createRoot(document.getElementById('root'));
        root.render(<App />);
    </script>
</body>
</html>
