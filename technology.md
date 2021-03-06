Technology
----------

* Eric Seufert. Freemium Economics
    - Chapter 4 Freemium Metrics
        - Minimal viable metrics
            - Four high-level categories: retention, engagement, monetization, viralty
        - Working with metrics in the freemium model
            - Analytics in a freemium context is contingent on the existence of very large data sets accessible only programmatically
            - Data analysts' focus shift from product feature optimization and towards product prioritization and management insight.
            - Report efforts, build dashboards, circulates KPI reports.
        - The retention profile
            - Area under the retention curve = total likely lifetime
            - Retention is best calculated retrospectively (= affect user cohort)
            - Defining churn = the point past which 80% of users do not return
        - Monetization
             - Conversion rate = the percentage of users who convert to revenue
             - One strategy: don't show users ads until you are sure they don't convert
             - Viewing ads shouldn't be considered as conversion
        - Revenue metrics
            - ARPU - average revenue per user; ARPPU - average revenue per paying user
            - Daily ARPU = ARPDAU (average revenue per daily active users)
            - Product catalogue distribution, first purchase distribution
        - Onboarding funnel
        - Session metrics
            - Average/median session length
            - Daily number of sessions
        - Net promoter scores
            - 9, 10 = promoters, 7, 8 = neutral, 1-6 = distractors
            - Percentage or promoters minus percentage of distractors
        - Viralty
            - Viralty hooks, the k-factor
        - For freemium products, team should work in small iterations at a swift pace
        - Dashboard design
            - Balance between scientific and artistic
        - Analytics as a driver for product development
    - Chapter 5 Lifetime Customer Value
        - Lifetime customer value and the freemium model
        - LTV = total amount of money a user is expected to spend, adjusted for inflation
        - Gupta et al. 2006 http://journals.sagepub.com/doi/abs/10.1177/1094670506293810
        - Customer equity (CE) = aggregate sum of the LTV metrics for all current and future users (mainly for company valuation)
        - Making use of LTV
            - LTV provides return on marketing efforts (helps decisions on marketing budget, product development riorities)
            - Cross-promotion: shift users from one product to another based on their LTV estimates
            - LTV has two primary components: retention and monetization.
        - LTV in, LTV out
            - A user can be evaluated on their way in AND out (actual LTV)
            - Retaining an existing user is far cheaper than acquiring a new user, and a user with LTV=0 has more value to a new user
        - Discounting LTV
             - by a risk-free rate (return on risk-free government bond)
        - Calculating lifetime customer value
             - Any LTV calculation = expected lifetime of a user * user's expected revenue per period
             - Spreadsheet method
             - Analytics method
    - Chapter 6 - Freemium monetization
        - Product catalogue should be composed of not only static, predefined items but also with dynamic items
        - Continuous monetization curve (plot of LTV over percent of users)
        - More personalization, meeting the idiosyncratic needs -> higher revenue
        - Monetization curve is not really continuous (because money is discrete), but should approach continuous form
        - Non-paying users
            - NPUs are essential core component of any freemium product's user base
            - Value of NPUs: data, viral and critical mass (network effects), or 'nightclub effect'
        - Revenue-based user segments
            - Whale / dolphin / minnow classification, blue/orca/beluga whales
            - Can be easily plotted by stacked bar graphs
            - Wild fluctuations in segments are the sign that monetization curve hasn't reached an optimal level of continuity
        - Data products
            - Recommendation engine (suggests new friends)
            - Dynamic selection of most appropriate products from the product catalog
        - Downstream marketing
            - Upstream marketing for growing user base, downstream marketing for reengagement
            - Reengagement emails, push notifications
            - Promotions (discounts, time-limited offers, combination offers, volume prices) - can be used to gauge user response (e.g., value buyer?)


* David M Diez, et al. OpenIntro Statistics (Third Edition)
    - Chapter 1 Introduction to data
        - nominal (categorical variable) and ordinal (categorical variable with ordering) variables
        - associated variables = dependent variables (no association = independent)
        - beware of 'non-response bias' for surveys, as well as convenience sample (bias towards accessibility)
        - confounding variable - correlated with both the explanatory and response variables.
        - Stratified sampling - group the population into strata, then sample from each stratum.
        - blocking - split into blocks based on a variable, random sample from each block to randomize the effects
        -

*  Richard Blum and Christine Bresnahan. Linux Command Line and Shell Scripting Bible, Wiley 2015.
    - Chapter 1 Introduction
        - Linux Kernel <-> GNU System Utilities <-> Application Software
        - Linus Torvalds put his 'copy' of Unix kernel and solicited suggestions on the internet
        - Swapping out - moving memory pages that have not been accessed for a period of time to the swap space
        - 'init process' starts all the other processes
        - Run levels are used to control which processes to run by the init system
        - Kernel modules are a way to add device drivers without compiling Linux Kernel
        - Three classifications of device files: character (e.g., terminal), block (e.g., disk), and network.
        - GNU - developed a complete set of unix utilities, but usually run on Linux kernel
        - X.org - provides open source implementation of X Window System
        - Many of the specialized Linux distributions (e.g., Ubuntu, Linux Mint) are based on Debian.
    - Chapter 2
        -
    - Chapter 3
        - /var 'variable' - for files that change frequently, such as log files
        - File name wildcards - [a-i] character range, [!a] character 'not'.
        - Show inode numbers by 'ls -i' (soft links are different files, hard links are the same)
        - Query file type by 'file' command
    - Chapter 4
        - ps command - historically two versions (BSD style params and Linux ones) - now merged to one
        - (not available on Mac because Linux and Mac differ in a way how to expose process info.)
        - grep command - by default uses Unix-style regex (use egrep for POSIX extended regex)
        - kill command - by default sends a TERM ('terminate if possible') signal
    - Chapter 5
        - Default system shell (usually /bin/sh) used for running system shell scripts
        - Encase a list of commands in parentheses -> a process list (executed in a subshell)
    - Chapter 6
        - 'export' command - export local variable to the global environment.
        - zsh startup files: .zshenv is sourced in all invocations of the whell, while .zshrc is sourced in interactive shells.
        - Defining an array variable e.g., mytest=(one two three four five)
    - Chapter 7
        - Now every process that runs in background has its own account.
        - Linux reserves UIDs below 500 for system accounts. (for normal users, UIDs start from 500)
        - most Linux systems holds passwords under /etc/shadow (only login can access)
        - System copies contents of /etc/skel to user's HOME directory
        - touch command creates a (empty) file using the default permission (which can be set by umask command)
    - Chapter 8
        - A journaling file system writes changes to a temporary file (journal first), then clear it after the data is committed to the physical device.
        - XFS filesystem uses the writeback mode of journaling, supports online resizing of the filesystem
        - Logical volume manager (LVM) lets you dynamically add space over multiple physical partitions.


* Frederick P. Brooks Jr. The Mythical Man-Month.
    - Chapter 1
        - Programming -> programming product (generalized, tested) / programming system (integrated) -> programming system product
        - Programs have to be perfect - adjusting to it is the most difficult part of learning to program.
        - "The challenge and the mission are to find real solutions to real problems with available resources."
    - Chapter 2
        - Men and months are interchangeable commodities only when a task can be partitioned among many workers with no communication between them.
            - counterexample: woman bearing a child always takes 9 months.
        - 33% planning, 16% coding, 25% component test, 25% system test.
        - 'Adding manpower to a late software project makes it later.'
    - Chapter 3
        - Each segment of a large job be tackled by a team, but that team must be organized like a surgical team.
    - Chapter 4
        - Conceptual integrity is the most important consideration in systems design. -> systems design must proceed from one mind, or a ver small number of resonant minds.
    - Chapter 5
        -
    - Chapter 6
        -
    - Chapter 7 Why did the tower of Babel fail?
        - communication and organization
        - How to reduce the amount of communication - division of labor and specialization of function


* Michael Feathers. Working Effectively with Legacy Code.
    - Chapter 1
        - Preserving existing behavior is one of the largest challenges in software development.
    - Chapter 2
        - Don't 'Edit and Pray.' Instead, 'Cover and Modify.'
        - Good unit tests 1) run fast and 2) help us localize problems. Don't talk to DB, files, or networks.
    - Chapter 3
        - Sensing - accessing the value our code computes, and Separation - getting a piece of code to run
        - Fake objects (e.g., creating FakeDisplay instead of real display hardware, that has a 'getLastLine' method)
        - Mock objects - fake objects that perform assertions internally.
    - Chapter 4
        - Seam - a place where you can alter behavior in your program without editing in that place.
        - Object seam - subclass a class in the production code and override various methods of the class.
        - Link seams - a place where you can alter behavior by linking to a (mock, with sensing) library.


* Andrew Hunt and David Thomas. Pragmatic Programmer.
  - Kaizen applies to individuals too. Refine the skills and add new tools.
  - Chapter 1
    - Don't leave broken windows (bad designs, wrong decisions, or poor code) unrepaired.
    - If you don't have time, board it up (e.g., 'Not Implemented')
    - Be a catalyst for change - people find it easier to join an ongoing success.
    - Your knowledge and experience are your most important professional assets. Unfortunately, they're expiring assets.
    - Invest regularly (just like financial portofolio)
    - Learn at least one new language every year.
  - Chapter 2
    - Programmers are constantly in maintenance mode. Maintenance is not a discrete activity, but a routine part of the entire development process.
    - Orthogonality - If I dramatically change the requirements behind a particular function, how many modules are affected? The answer should be one.
    - Prototyping generates disposable code. Tracer code is lean but complete, and forms part of the skeleton of the final system.
    - What to say when asked for an estimate - 'I'll get back to you'
  - Chapter 3
    - Keep knowledge in plain text
    - It is better to know one editor very well, and use it for all editing tasks: documentation, memos, system administration, and so on.
    - Always use source code control
    - Debugging is just problem solving, and attack it as such.
    - we want a bug that can be reproduced with a single command.
    - Rubber ducking - try to explain to somebody (who doesn't have to answer)
  - Chapter 4
    - Accept that you can't write perfect software
    - Liskov substitution principal - subclasses must be usable through the base class interface without the need for the user to know the difference
    - Dead programs tell no lies - crash early
    - If it can't happen, use assertions to ensure that it won't
  - Chapter 5
    - Studies have shown [BBM96] that classes in C++ with larger response sets are more prone to error than classes with smaller response sets (a response set is defined to be the number of functions directly invoked by methods of the class).
  - Chapter 6
    - Don't just test your code, test your assumptions. Use assertions.
    - Building software is more like gardening than construction.
    - "Refactor early, refactor often." - now is the easiest time to refactor. Later there will be more constraints.
    - Don't try to refactor and add functionality at the same time. Make sure you have good tests. Take short steps.
  - Chapter 7
    - Simple technique for getting inside users' requirements: become a user.
    - Don't think outside the box - find the box. Enumerate all the possible solutions. Why doesn't it work? Can you prove it? (e.g., Trojan horse)
  - Chapter 8
    - Generate a brand. Come up with a name for a project, ideally something off-the-wall.
    - Test early. Test often. Test automatically.
    - Use saboteurs to test your testings. Introduce a bug deliberately and check if the tests complain.

* Steve McConnel. Code Complete, Second Edition, 2009.
  - Chapter 5 Design in Construction
    - Tacoma bridge - only by building the bridge could they learn about the additional consideration in the problem that allowed them build another bridge that still stands
    - Minimize the amount of a program you have to think about at any one time (think of 'mental' juggling) - more balls, more errors
    - Think of a maintenance programmer as your audience, and design the system to be self-explanatory
    - System level diagram (of components like user interface, application level classes, databases, etc) should be an acyclic graph
    - One attribute of great designers - anticipating change.
    - Avoid semantic coupling e.g., module A 'knows' module B's inner workings.
  - Chapter 6 Working Classes
    -  [TO READ AGAIN]

  - Chapter 20 The Software-Quality Landscape
    - Catch problems at the "lowest-value" stage (unit tests, reviews, rather than production)
    - Prototyping can lead to better designs, better matches with user needs, and improved maintainability.
    - No single technique achieves >75% defect detection rate - developers need use a combination of techniques.
    - Variety of errors people found was so great - having two independent groups almost doubles the defects detected.
    - Inspections (code reviews) are several times cost-effective than testing.
    - The best way to improve productivity and quality is to reduce the time spent reworking code (requirement change, design change, or debugging)
        - The single biggest activity is debugging and correcting code that doesn't work properly

  - Chapter 23 Debugging
    - debugging occupies 50% of time of total development time
    - roughly 20x difference in time between experienced and inexperienced programmers to find bugs
    - improving quality reduces development cost -> they are not trade-off
    - it is your best interests to assume an error is your fault
    - Scientific method for debugging: gather data through experiment, hypothesize, prove / disprove
    - Classes that have defects before are likely to continue to have defects
    - "Confessional debugging" - try to explain to someone else and the problems will be solved on its own
    - Take a break when you start feeling anxiety - let your subconscious mind tease out a problem
    - Rewrite a bad code (e.g., in 30mins) rather than debugging it (could take two hours)
    - Understand the problem before you fix it.
    - Achieve a global (or at least, a few hundred lines around) understanding of program rather than focusing it locally
    - Different mindsets for building and debugging code - creative, design thinking, and rigidly critical thinking
    - Set compile warning level to highest and deal with warnings as if they are errors

  - Chapter 24 Refactoring
    - Reason to refactor: code is duplicated, long routines, long parameter lists
    - A subclass only uses small fraction of parent's routines
    - Keep the refactoring small, do one at a time
    - Keep 'parking lots' - list of things you noticed during refactoring but not doing right now
    - Targeting error-prone modules which everyone is afraid of is an effective strategy

  - Chapter 33 Personal Character
    - If you want to be great, you are responsible for making yourself great.
    - Study after study found 10 to 1 difference in speed (of programming and debugging), number of errors.
    - The purpose of many good programming practices to reduce the load on your brain.
    - Humble programmers who compensate for their fallibilities write code that's easier to understand and has fewer errors.
    - Find code written by superior programmers and read it.
    - Programming is only 15 percent communicating with the computer and 85 percent communicating with people.
    - Feeling tempted to compile a program to "see what happens" is a warning sign.
    - It's often better to give up on the error after a certain amount of time (say 15 minutes) with no progress - then think differently.
    - The value of 'hands-on' experience is small - 'five years of C programming experience' is a silly statement - If a programmer hasn't learned C after a year or two, the next three years won't make much difference.
    - When you first learn something, learn it the right way - this forms good habits.

* Clean Code
  - 17 Smells and Heuristics
    - When you see commented-out code, delete it!
    - Functions should have a small number of arguments --- more than three is very questionable.
    - Boolean arguments loudly declare that the function does more than one thing.
    - Prefer non-static methods to static methods (make sure that there is no chance that you'll want it to behave polymorphically.)
    - Make sure you understand how algorithms/functions work before. It is not good enough that it passes all the tests. You must know that the solution is correct.
    - Exhaustively test near bugs - bugs tend to congregate.

* David Beazley and Brian K. Jones. Python Cookbook, Third Edition, 2013.
  - Chapter 1
    - Python 3 supports star expressions for unpacking: first, * middle, last = data
    - from collection import deque -> keep the last N elements pushed
    - heapq -> heap, supports O(1) min() and O(log n) push.
    - OrderedDict -> preserves the order of keys
    - Python 3 dict.keys() -> set, not list, support intersection, union, diff, etc.
    - Name a slice by slice(st, ed) (supports start, stop, step)
    - Python >= 2.7 supports Counter (from collections) - dict subclass for counting iteratives
    - itemgetter and attrgetter in operator can be used for sort key func (instead of lambda)
    - namedtuple's replace() can create a new instance with a value replaced
  - Chapter 2
    - str.startswith and endswith takes a tuple (for multiple possibilities)
    - from fnmatch import fnmatch, fnmatchcase -> Unix-like file name wildcard
    - unicodedata.normalize(form, str) form: NKC (normal form decomposition -> composition) NKD (normal form decomposition)
    - newer codes should prefer format over "%". format also supports aligning and variable interpolation.
  - Chapter 3
    - useful random functions: choice, sample, shuffle, getrandbits
    - datetime.strftime() can be slow -> use custom function instead if there are a lot of strings to process
    - use pytz to deal with timezones
  - Chapter 4
    - yield from (generator delegation) expression -> from Python 3.3
    - reversed() can be implemented by __reversed__() (reverse iterator)
    - iterators can be sliced by itertools.islice(), dropwhile()
    - introduction of itertools.combinations, permutations, zip_longest, chain
    - iter(callable, sentinel) -> loop while the return value is not equal to the sentinel
  - Chapter 5
    - object implementing 'buffer interface' -> exposes underlying memory buffer -> can directly write() and readinto()
    - __setstate__() and __getstate__() for pickle -> set and get internal states
  - Chapter 6
    - serialize_instance() and unserialize_instance() for JSON serialization of instances
    - Use memoryview() to avoid unnecessary copies (like slices) http://stackoverflow.com/questions/18655648/what-exactly-is-the-point-of-memoryview-in-python
    - Default function arguments are evaluated only once (at the time of function definition)
    - Use instance test ("is") with a global "object()" to test if any values (including 0, [], None) are passed to default argument
  - Chapter 7
    - lambda: Capture the value at the time of definition using the default value: e.g., lambda x, n=n
  - Chapter 8
    - Use "!r" format string to force repr() instead of str()
    - format() can be customized by __format__()
    - Creating getter/setter -> decorate by @[attname], @[attname.setter], @[attname.deleter]. Don't write getters/setters unless necessary (e.g., type/value check)
    - Descriptors: reusable, generalized properties. see http://nbviewer.ipython.org/gist/ChrisBeaumont/5758381/descriptor_writeup.ipynb
    - Bypass __init__() by involing __new__() directory (e.g., JSON deserialization)
    - Python ast (abstract syntax tree, using in Python compilation) uses the visitor pattern
    - Python's GC is simple refernece counting. You can use weakref to reference to an object without increasing the count.
  - Chapter 9
    - functools.wraps -> Update the wrapper function to look like the wrapped function (e.g., name & docstring)
    - Metaclasses -> class of class (e.g., 'type'), change behaviors of classes by defining __new__, __init__ (with clsname, bases, clsdict)
  - Chapter 10
    - Use __all__ to control what to export as a module
  - Chapter 11
    - Use "requests" http://docs.python-requests.org/ for simple HTTP clients
    - Writing simple remote procedure call using XML-RPC (xmlrpc module)
  - Chapter 12
    - Write simple map-reduce process using futures.ProcessPoolExecutor
    - GIL (global interpreter lock) only affects programs that are heavily CPU bound (not IO)  GIL workaround -> multiprocessing module to create a process pool, or disable using C extension programming
  - Chapter 14
    - Use unittest.mock.patch() to replace sys.stdout with StringIO() (also be used as a decorator to replace a function with another)
    - Use time.perf_counter() to get a clock with the highest available resolution
    - General advice on how to make your program faster: http://chimera.labs.oreilly.com/books/1230000000393/ch14.html#_making_your_programs_run_faster


* Brian W Kernighan and Rob Pike. The Unix Programming Environment. 1983.
  - Chapter 1
  - Chapter 2
    - "sed-uid" bit - grand the permission of the owner when run (used for passwd command)
    - "read" and "execute" permission for directories - "read" the file names of the directory, "execute (search)" to actually retrieve the file. "write" permission required to move/delete the files
    - /dev info: character (c) or block (b), the major number (type) and the minor number (distinguishes different devices)
    - /dev/tty -> terminal (used by crypt to receive the password input)
    - dot "." shell built-in command: execute a script in the current environment (variables are overwritten) or prefix any commands with var=val
  - Chapter 4
    - filters. egrep (extended) and fgrep (fast), now consolidated into the same program (grep)
    - sed convenient command (e.g., sed -n '20,30p' -> print lines 20-30, sed '1d' -> print except the first line)
    - awk special variables: NR (line number), FS (field separator), built-in functions (e.g., length)

* MIT Technology Review Business Report: Data and Decision Making http://www.technologyreview.com/businessreport/data-and-decision-making/download/
  - 1-800-Dentist A/B test to optimize fill out the form using "Optimizely" (by ex-Googler, used Obama campaign, putting personal message from President increased fund-raising by 14%), at least 15% of top 10K websites run A/B tests
  - A Google designer quit because Google cannot decide between two blues so it tested 41 shades...
  - Uncritical reliance on data alone can be problematic, but so is overreliance on intuition or ideology. (e.g., Ron Johnson, CEO of JC penny)
  - Importance of a scientific mindset for decision making (hypothesis -> test by data) - most plausible human explanation is not necessarily correct. Do not infer too much from any one outcome
  - Experimentation, especially controlled experiments to tease out causal effects, not correlation
  - Palantir, PayPal - suite of fraud analysis tools for humans to act on suspicious activities
  - Licklider (Man-Computer Symbiosis) influenced IBM's "cognitive computing" virtual assistant + brain-like chips
  - Linkedin's University Pages - appeal to under 18 users, to show statistics on graduates' careers (e.g., MIT graduates tend to land on Google, IBM, and Oracle)
  - IBM Watson, 2000 engineers working on it, combining other cognitive technologies, including voice and image -> e.g., simple conversations for a call center
  - Reis ("The Lean Startup") technology risk isn't the problem anymore. Market risk is.
  - Correlation Ventures http://www.correlationvc.com/ - pick companies by algorithms

* Peter Thiel "Zero to One"

  - "Every moment in business happens only once. [...] The next Mark Zuckerberg won't create a social network. If you are copying these guys, you aren't learning from them."
  - "What important truth do very few people agree with you on?" - "Most people think the future of the world will be defined by globalization, but the truth is that technology matters more." "What valuable company is nobody building?"
  - "A bad plan is better than no plan."
  - Google is a monopoly in search but a small player in ads
  - All happy companies are different: each one earns a monopoly by solving a unique problem.
  - "the most important question you should be asking: will this business still be around a decade from now?"
  - "proprietary technology must be at least 10 times better than its closest substitute in some important dimension to lead to a real monopolistic advantage." (e.g., Amazon, 10 times as many books as any other bookstores)
  - every startup should start with a very small market. Always err on the side of starting too small. The reason is simple: it's easier to dominate a small market than a large one.
  - biotech startups indefinite approach to business
  - "Making small changes to things that already exist might lead you to a local maximum, but it won't help you find the global maximum."
  - Mark Zuckerberg didn't sell Facebook to Yahoo! for $1B in July 2006 - "A business with a good definite plan will always be underrated in a world where people see the future as random."
  - Albert Einstein "compound interest is the most powerful force in the universe."
  - venture returns follow a power low: "a small handful of companies radically outperform all others."
  - investors who understand the power law make as few investments as possible.
  - "It does matter what you do. You should focus relentlessly on something you're good at doing, but before that you must think hard about whether it will be valuable in the future."
  - there are many more secrets left to find, but they will yield only to relentless searchers.
  - Thiel's law: a startup messed up at its foundation cannot be fixed.
  - how well the founders know each other and how well they work together matter just as much
  - "Why would someone join your company as its 20th engineer when she could go work at Google far more money and more prestige?" - two general kinds of good answers: answers about your mission and answers about your team.
  - Most fights inside a company happen when colleagues compete for the same reponsibilities - make one person responsible for doing just one thing
  - poor sales rather than bad product is the most common cause of failure.
  - "big data"   is usually dumb data. "Most valuable companies in the future won't ask what problems can be solved with computers alone. Instead, they'll ask: how can computers help humans solve hard problems?"
  - doing something different is what's truly good for sociery --- it's also what allows a business to profit by monopolizing a new market
  - no sector will be so important that merely participating in it will be enough to build a great company
