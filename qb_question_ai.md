I could train a language model to write QB questions
	LLaMA
		Probably cheapter than Da Vinci if I did it on vast.ai
	GPT3 Da Vinci
	Just Chat GPT w/ a couple examples
		Probably would give me bad results?
		First attempt with few shot training: not very good
			It could do it if I prodded it to, but it was not very pyramidial and didn't give
3/9/23 Attempt 1:
	llama can be a pain to get working
	I need to learn pytorch so that I can properly train it
		Copying chatllama doesn't work well
	bitsandbytes
		make sure to add cudart & other libs to the last -L directory when linking
	Llama Options:
		llama
		llama-int8
		pyllama
3/14/23 Status:
	Options:
		GPT-4 Few Shot training with questions
			Works okay -- the questions are right, they generally get easier as it goes along, but they just seem wrong
				Not canon?
			This event was sparked by tensions between workers and police after a strike at the McCormick Harvesting Machine Company turned deadly. The rally at which it occurred was in support of the eight-hour workday movement. Anarchist August Spies delivered a speech moments before an (\*) unknown individual threw a bomb into the crowd, resulting in numerous deaths. The aftermath saw eight anarchist leaders arrested and four executed, despite a lack of evidence tying them to the bombing. For 10 points, name this 1886 labor-related riot that took place in a Chicago square. (after telling it its problems a few times)
		GPT-4 Few Shot training with old clues
			Next thing to try
			Maybe write a plugin to do it?
		GPT-4 Few Shot training with old questions of the same answer that I ask it to write
			Works better, but still messes up the difficulty ordering
				This leader, who once commanded at Fort Harrison, played a crucial role in ending the Second Seminole War by defeating the Seminoles at the Battle of Lake Okeechobee. This president's administration was marked by the Galphin Affair and the signing of the Clayton-Bulwer Treaty, which addressed the construction of a canal in Nicaragua. Prior to his presidency, he led the American forces to victory at the Battle of Palo Alto, relieving the Siege of Fort Texas, and (\*) Buena Vista during the Mexican-American War. He ran as a Whig candidate in the 1848 presidential election and defeated Lewis Cass and Martin van Buren. Known for his "Flying Artillery" tactic, he was given the nickname "Old Rough and Ready." For 10 points, name this 12th president of the United States, who died in office and was succeeded by Millard Fillmore.
		GPT-4 Few shot training after asking it to order the clues
			Works better, but still kind of oddly places new clues, and otherwise just copies old questions mostly
			The “Two Whatevers” [0] supported the leader of this event after it had taken place [1]. One central figure of this event was a Defense Secretary [2] who died in a plane crash [3] while trying to flee to the Soviet Union [4]. This event led to the destruction of many historical relics and monuments [5]. The Down to the Countryside Movement [6] and the use of big character posters [7] were initiated during this period, while the Red Guard [8] engaged in wanton destruction and targeted academics [9]. This event, which followed the Great Leap Forward [10], ended with the arrest of Jiang Qing [11] and the rest of the Gang of Four [12]. For 10 points, identify this period of extreme anti-traditionalism in China [13] which occurred under Mao Zedong.
		Instruct GPT fine-tuned AI with old clues
			that is: provide answer and clues and write a question
		Instruct GPT fine-tuned AI with old questions
		LLaMA fine-tuning / and others
			Hard to embed in app
		Maybe I can chuck it on a website if gpt-4 api access exists as a curisioty
Providing example of questions on the topic ideas:
	Ask it for a theme and ask it to find questions on that theme
			