Work on this? https://www.reddit.com/r/Compilers/comments/13d1ifv/otterkit_open_source_cobol_2023_compiler_isoiec/
Find conferences and programs that I like and apply
Scheme -> Desmos compiler
Chinese CLI w/ noncurses written in Rust
Proper YT Music CLI
Using ML Text to Speech, QB question reader
	Taking a break until I manage t
	Allow transcribing TUs with TorToiSe online?
		I could also crowdsource it on people's computers, but would people really wait 2 minutes per qb tossup they want to hear?
		Ask pace or naqt for sponsorship?
	Also allow submitting of your own read tossups
	Could build my own website for this
		Cloudflare stack:
			R2 + Pages + functions
		Front-end: 11ty + webc & HTML + CSS + minimal JS + HTMX + Hyperscript
		Back-end: Cloudflare Functions (+ something else?)
		For TorToiSe: https://replicate.com/afiaka87/tortoise-tts
	Actually, seems quite complex -- probably best to integrate with QB Reader
Using openai's Whisper, QB Reader PR with audio answer recognition
Using LLaMA or GPT 3 Da Vinci or few short Chat GPT to write quizbowl questions [[qb_question_ai]]
	Have another AI to review questions and optimize first AI?
		Actual RELF (or whatever it's called)
Student Vue+ emulator Extension
	Also as an extension for IOS Safari?
live QB match app
nushell autoformater and syntax highlighter
Something for congressional app challenge?
Automatically do quizlet learn bookmarklet
A library for react or similar that automatically generates a backend for certain functions
	see: https://hackclub.slack.com/archives/C0EA9S0A0/p1678750362524679
	also look at [Remix](https://remix.run)
		my idea is like a light weight version of it
Chinese Mneomnic maker with Chat GPT
(HARD) Holy Grail AI Waifu Assistant:
	Just emulate with uncensored chatgpt?
	Aspects:
		Mostly Uncensored Chat GPT for the response
		Coqui TTS / Tortorise TTS for Speaking
		Some manually implemented in built functionalities
		Either AI Video Generation or hand rigged 3d animation for the movement?
Vim Regexr
AI QB Moderator (SaaS?)
	Current status: Just as useful as any of my hobby projects
		Without being able to identify who gives the answer, it doesn't simplify the workflow for in person tournament enough
		I don't think there's enough interest for it for purely buzzin.live or for discord
		If I want a random project though, it's plenty interesting
		Maybe ask Rahul or somebody else if they would pay $20 for a kit to detect the mod or just use it with only answer recognitio
	Ways to do:
		Integrated with wasm:
			Use JS bindings w/ whisper.cpp and JS or a transipled language
			Write front-end with Remix
			Host it on Cloudflare pages w/ their stack
		seperate backend or frontend:
			backend:
				if school project: write all in modern Java w/ bindings to wisper.cpp
					Use Lombok and perhaps Guava (and perhaps others, ofc)
					Use that easy native java library I can't remember the name of
				else:
					rust library
			frontend:
				either GUI written in backend library or web frontend (w/ electron/similar or localhost website) with rest API written in backend language
	Seperate out backend library and front-end
	Two frontends: desktop app for 1 reader in-person and discord bot for 0 reader online
	Big issue is identifying who gives the answer, options:
		Manual input
		Require recognition
		buzzin.live
(selling, probably) anki deck with tortoise generated chinese audio
	or another TTS with audio better than google translate
CLI QB Reader client
Easy one time RSS Feed to Epub
Refactor QBreader code into react components for npm
	Seperately: QB Reader NPM package as react component
	Or just write my own
NPM module for qbreader querying?
	pretty simple already though
	just get this removed or replace it? https://www.npmjs.com/package/quizbowl
Qbreader PR to not take into account diacritics when searching
diy buzzer set
auto identify clues from wikipedia
	qanta people apparently did this but iirc thelink is dead
chatgpt conversation search extension (or userscript or something)
qb: weird format online tournament
qb pronunciation guide maker
Write hack club workshop???
	eh,  takes too much time
apply?: https://www.atlasfellowship.org/
Help out with Paradigm conference?
Compare how good Chat GPT is with QANTA
Something with Chat GPT plugins?
Extension which is hard to get rid of and charges you x amonunt of money every time you go to a website?
	Could warn you before (or, **dangerous** mode which doesn't warn you)
	Is this easy to implement?
			Maybe easier to implement with Brave and BATs?
				Or something similar with crypto
Fix QB Reader FF Mobile Question dropdown!
Add drag to difficulties in QB Reader
Post qb flashcards on discord by request
	Split it into sm notes, real raw sm collection, and sm cards (in anki format)
Small drawing tablet-esque (e-paper?) pad to be attached to the right of the trackpad
	Used to write chinese characters
	Needs to be activated with finger pressure
		Or a stylus ig, but it would significantly increase the complexity
Submit PRA (like FOIA) request to PUSD to figure out what RBHS ASB is doing with its money
	Or maybe just ask Charlotte for records?
		Or for info on the budget?
	Maybe ask for all meeting minutes, or, if it exists, a budget?
super mario world tas arbritary code execution bad apple
	Bonus points if I arbritary code execute a chiptune