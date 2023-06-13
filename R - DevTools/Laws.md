## Software
- [Zawinski’s Law](https://en.wikipedia.org/wiki/Jamie_Zawinski#Zawinski's_Law) - Every program attempts to expand until it can read [mail](https://en.wikipedia.org/wiki/E-mail "E-mail"). Those programs which cannot so expand are replaced by ones which can. Some have interpreted this as commenting on the phenomenon of [software bloating](https://en.wikipedia.org/wiki/Software_bloat "Software bloat") with popular features
- [Polanyi’s Paradox](https://en.wikipedia.org/wiki/Polanyi%E2%80%99s_paradox) - “We can know more than we can tell”
    - applicable in AI - we find it hard to describe common sense
    - design - clients that don’t know what they want but definitely don’t want what you show them
    - related to [Moravec’s Paradox](https://en.wikipedia.org/wiki/Moravec%27s_paradox): “It’s easy to give computers adult level intelligence, but hard to give them child level perception and motor skills.”
        - “To Err is Human; To Really Foul Things Up Requires a Computer” - Bill Vaughan
- [Postel’s Law](https://en.wikipedia.org/wiki/Robustness_principle) aka Robustness principle: “be conservative in what you do, liberal in what you accept”
- [Parkinson’s Law](https://en.wikipedia.org/wiki/Parkinson%27s_law) is well known, but has several interesting corollaries: the Stock-Sanford Corollary states that “If you wait until the last minute, it only takes a minute to do.”
- [Cargill’s Law](https://thenewstack.io/code-n00b-ol-ninety-ninety/): “The first 90 percent of the code accounts for the first 90 percent of the development time. The remaining 10 percent of the code accounts for the other 90 percent of the development time.”
- [Hyrum’s Law](https://www.hyrumslaw.com/): “With a sufficient number of users of an API, it does not matter what you promise in the contract - all observable behaviors of your system will be depended on by somebody.” - [Even bugs will be relied on!](https://twitter.com/acemarke/status/1261761355712954368?s=20).
    - [Relevant XKCD](https://xkcd.com/1172/)
    - example - Python Ordered Dicts!
    - [https://shoptalkshow.com/407/](https://shoptalkshow.com/407/)
        - ~28 mins in: `window.event` was a nonstandard api but every browser except firefox implemented it. Then firefox implemented it, and JIRA broke.
        - 30 mins in: JS Objects aren’t supposed to have stable order. But every browser basically implemented them with stable order. Now browser that wants to do a performance optimization wants to use unstable order, but cannot, because apps now rely on it
- [Law of Demeter](https://en.wikipedia.org/wiki/Law_of_Demeter) - a given object should assume as little as possible about anything else - its neighbors and subcomponents
    - how to square this against “be liberal in what you accept, conservative in what you output”?
    - what happens to Unix Philosophy when you defensively code everything?

Some people combine laws:

- Zawinski-Greenspun-Atwood-Murphy’s Law - [“Anything that _can_ expand to read email with lisp in javascript, _will_ go wrong.”](https://twitter.com/secretGeek/status/1116217143933063169)
- Pareto-Hofstadter-Parkinson’s Law: [“80% of the work expands so as to fill the time available for its completion and still take 20% longer than expected.”](https://twitter.com/swyx/status/1231292352544808960)

More lists:

- [https://haacked.com/archive/2007/07/17/the-eponymous-laws-of-software-development.aspx/](https://haacked.com/archive/2007/07/17/the-eponymous-laws-of-software-development.aspx/)
- [https://www.timsommer.be/famous-laws-of-software-development/](https://www.timsommer.be/famous-laws-of-software-development/)

## Hardware

- [Moore’s Law vs Wright’s Law](https://www.forbes.com/sites/jimhandy/2013/03/25/moores-law-vs-wrights-law/#162188f277d2): _each percent increase in cumulative production in a given industry results in a fixed percentage improvement in production efficiency_
- [Dennard Scaling](https://en.wikipedia.org/wiki/Dennard_scaling): as transistors get smaller, their power density stays constant, so that the power use stays in proportion with area; both voltage and current scale (downward) with length
- [Wirth’s Law](https://en.wikipedia.org/wiki/Wirth%27s_law) - this is a special case of [Jevons paradox](https://en.wikipedia.org/wiki/Jevons_paradox): _software is getting slower more rapidly than hardware is becoming faster_
    - Spolsky wrote a great counterargument to this [on Bloatware](https://www.joelonsoftware.com/2001/03/23/strategy-letter-iv-bloatware-and-the-8020-myth/)
- [Amdahl’s law](https://en.wikipedia.org/wiki/Amdahl%27s_law): the theoretical speedup in latency of the execution of a task at fixed workload that can be expected of a system whose resources are improved (the “mythical man month” law). another statement - you can never make a system faster than its slowest part.
    - Also applied on Software and People [https://codahale.com//work-is-work/](https://codahale.com//work-is-work/)
    - adding manpower to a late sofrware project makes it later - Brooks’ Law

## Business of Tech

- Commoditize your compliments - [Gwern](https://www.gwern.net/Complement), [Spolsky](https://www.joelonsoftware.com/2002/06/12/strategy-letter-v/)
- Rules for how Networks Scale (from [pmarca](https://a16z.com/2019/12/16/starting-greatness-0-to-1-mosaic-netscape-marc-andreessen/))
    - O(N): Sarnoff’s Law - the value of a broadcast network increases in direct proportion with the number of users
    - O(N^2): Metcalfe’s Law - email is p2p - value is number of connections between two nodes
    - O(2^N): Reed’s Law - no of groups and subgroups inside the network - what people do inside social networks and games

## Socio-Psychological

- The [Gell-Mann amnesia effect](https://www.epsilontheory.com/gell-mann-amnesia/): you ascribe credibility to news on which you are not an expert, despite knowing how badly reported the news can be on things you ARE an expert. The ultimate troll, given that the name of Gell-Mann was given by Crichton to demonstrate this exact phenomena.
- Poe’s Law - sufficiently advanced satire is indistinguishable from extremism
    - _“Without a winking smiley or other blatant display of humor, it is utterly impossible to parody a Creationist in such a way that someone won’t mistake for the genuine article.”_
- [Shirky Principle](https://kk.org/thetechnium/the-shirky-prin/): Institutions will try to preserve the problem to which they are the solution
- [Cromwell’s Rule](https://en.wikipedia.org/wiki/Cromwell's_rule) - the use of prior probabilities of 1 (“the event will definitely occur”) or 0 (“the event will definitely not occur”) should be avoided, except when applied to statements that are logically true or false, such as 2+2 equaling 4 or 5.
    - _“I beseech you, in the bowels of Christ, think it possible that you may be mistaken.”_
- [Chesterton’s Fence](https://florentcrivello.com/index.php/2019/09/04/the-efficiency-destroying-magic-of-tidying-up/) - you should never take down a fence before knowing why it was put up
- [Ebbinghaus Effect](https://www.psychestudy.com/cognitive/memory/ebbinghaus-forgetting-curve) - mathematical model of how we forget - aka [forgetting curve](https://en.wikipedia.org/wiki/Forgetting_curve)
    - also notable for the visual [Ebbinghaus Illusion (relative size of circles)](https://en.wikipedia.org/wiki/Ebbinghaus_illusion)
- [Ringelmann effect](https://en.wikipedia.org/wiki/Ringelmann_effect) - work less when group is larger
- [Stigler’s Law](https://en.wikipedia.org/wiki/Stigler's_law_of_eponymy) - no scientific discovery is named after its original discoverer. Maximum meta!
    - Mark Twain: ”_“It takes a thousand men to invent a telegraph, or a steam engine, or a phonograph, or a photograph, or a telephone or any other important thing — and the last man gets the credit and we forget the others. He added his little mite — that is all he did. These object lessons should teach us that ninety-nine parts of all things that proceed from the intellect are plagiarisms, pure and simple; and the lesson ought to make us modest. But nothing can do that._”
- [Berkson’s Paradox](https://twitter.com/MWStory/status/1205486677369786369?s=20) - positive correlations become negative because of filters that trade factors off.
- [1% Rule](https://en.wikipedia.org/wiki/1%25_rule_(Internet_culture)) - 90% of the participants of a community only view content, 9% of the participants edit content, and 1% of the participants actively create new content.
    - application of [Zipf’s Law](https://en.wikipedia.org/wiki/Zipf%27s_law)
- [Goodhart’s Law](https://medium.com/@coffeeandjunk/campbells-law-goodhart-s-law-when-you-are-measuring-to-fail-c6c64923ad7) - “When a measure becomes a target, it ceases to be a good measure.”
    - Related HN: [https://news.ycombinator.com/item?id=17320640](https://news.ycombinator.com/item?id=17320640)
    - What’s Immeasurably Important? [https://www.collaborativefund.com/blog/immeasurably-important/](https://www.collaborativefund.com/blog/immeasurably-important/)
- Joseph effects and Noah effects
    - [https://www.perell.com/blog/news-in-the-age-of-abundance](https://www.perell.com/blog/news-in-the-age-of-abundance)
    - _“Joseph effects – seven fat years here, seven lean years there – occurred when markets were evolving gradually and continuously. Noah effects were cataclysms – the Flood, or the week of September 11 2001, when the New York Stock Exchange closed for five days and dropped 7.5 per cent on re-opening.”_