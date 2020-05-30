# 100 Days Of Code - Log

## Day 0: May 20, 2020

**Today's Progress**: Publicly committed to the task at my Github.io blog at <https://leon-paul-hart.github.io/>. I set up the blog in Jekyll on Github a while back, but it's finally been put to use today as I don't have twitter or other social media to post to.

**Thoughts:** I think the hardest part for me has been committing to this challenge and starting the ball rolling, for various reasons detailed in my blog post here <https://leon-paul-hart.github.io/blog/adhd/neurodiversity/2020/05/20/ADHD-and-the-100-days-of-code-challenge.html> extended endeavors like this can be problematic for me. With work taking up a lot of my energy too its hard spending a whole day coding and coming back home to do more! But I'm feeling inspired by the latest Microsoft Build conference and I'm excited to get stuck in while the inspiration is flowing, hope I can keep it up if the inspiration starts to falter!

**Link to work:** <https://github.com/leon-paul-hart/leon-paul-hart.github.io>

---

## Day 1: May 21, 2020

**Today's Progress**: Eek! Already off to a bit of a rocky start, was at work today, but once I sat down to do my hour of coding for the task I found my attention a bit all over the place.

So today I managed to...

- Make some actual commits to the 100-days-of-code repository itself to fix some broken URLs.
  - [Pull Request #311](https://github.com/kallaway/100-days-of-code/commit/6335f2d99b36f7ae289d10ba025fd27331b5ff20)
  - [Pull Request #312](https://github.com/kallaway/100-days-of-code/commit/37d919a796f840f85d64140d742c96b4001d71b9)
- Cleaned up my own fork of the repository.
  - [leon-paul-hart/100-days-of-code](https://github.com/leon-paul-hart/100-days-of-code/commits/master)
- And started building a .Net core console app for searching the [Open Movie Database API](https://www.omdbapi.com/)
  - [leon-paul-hart/OMDb_API_Console_App](https://github.com/leon-paul-hart/OMDb_API_Console_App)

**Thoughts:** I [registered for an API key](https://www.omdbapi.com/apikey.aspx), and got the console app running and pulling back the sample JSON from the API, which was easier than I expected it to be, I was over complicating it to start with. I did hit a real wall though when I went to try and set up a configuration file in the project that would keep my API key a secret and not commit it to the repo where anyone can see it. It's a free key, and it's limited in its number of requests per day, its not the end of the world if it gets exposed, BUT it goes against best practices. I'm discovering that the myriad of configuration options available in .Net development is absolutely [INSANE](https://docs.microsoft.com/en-gb/dotnet/api/system.configuration?view=dotnet-plat-ext-3.1), again, I'm probably over complicating it, I'm more than likely missing something simple, but I'm learning some core functionality about building applications that can utilise proper configuration settings.

**Link to work:** <https://github.com/leon-paul-hart/OMDb_API_Console_App>

---

## Day 2: May 22, 2020

**Today's Progress**: Still thinking about the configuration issue and how to get it working in a .Net Core console app, there is a lot of documentation on how to use configuration files in ASP.Net Core applications, which come with templates already set up to use configuration files, but not a lot of documentation for simple console apps. I did find a few articles though that I am working through :

- <https://garywoodfine.com/configuration-api-net-core-console-application/>
- <https://pradeeploganathan.com/dotnet/configuration-in-a-net-core-console-application/>
- <https://stackoverflow.com/questions/38114761/asp-net-core-configuration-for-net-core-console-application>
- <https://ballardsoftware.com/adding-appsettings-json-configuration-to-a-net-core-console-application/>
- <https://blog.bitscry.com/2017/05/30/appsettings-json-in-net-core-console-app/>

**Thoughts:** The issue here is that they all show a completely different way of doing things, going to have to go through them and figure out what is the most relevant method.

**Link to work:** Little in the way of programming process that I can show, as uploading the develop branch to Github would expose the API key as it is currently in the code for debugging.

---

## Day 3 : May 29, 2020

**Today's Progress**: So I fell off the wagon a bit sooner than expected... its been a few days since I last managed to properly sit down and programme for a full hour outside of work, but I've been thinking about the issue with the configuration settings for the [OMDb_API_Console_App](https://github.com/leon-paul-hart/OMDb_API_Console_App) and decided to skip having a configuration file for now, instead I've refactored the application to request the user inputs an API key of their own at runtime and it will use that provided key as a parameter in the final API query. This seems like a simpler and more user friendly way of doing things.

**Thoughts:** Pivoting like this is something I hope to get faster at doing over time and with practice, sometimes the notion of a 'best practice' can actually go against what is the best course of action. A recurring problem I have is making things overly complex from the start and painting myself into a corner. Constantly re-assessing and simplifying is a skill I am working on developing, and this is where I see the benefit of the #100DaysOfCode approach. Where an existing large complicated project with a lot of existing structure and decisions made by others permeating every line of code can be intimidating, and can limit what a relatively junior developer like myself feels comfortable making decisions on, a small solo project like this allows me to exercise that decision making process without worrying about stepping on senior developers toes, or making decisions which could be unintentionally detrimental to the project through lack of knowledge or understanding of the broader application stack.

**Link to work:** [OMDb_API_Console_App](https://github.com/leon-paul-hart/OMDb_API_Console_App)

---

## Day 4 : May 30, 2020

**Today's Progress**: Off at a tangent today! I dusted off an old Java CodeClan project that I was proud of at the time, only to be horrified at the state of the code... I guess it's a sign of progress! I ended up going over the code and fixing a lot of silly conceptual mistakes and refining the unit tests that were in place, even added some more to fill the gaps I had missed at the time, there is A LOT of work to be done to get this project up to a reasonable standard that I wouldn't be embarrassed by today. The main learning of today was getting the project working properly in the IntelliJ Idea IDE, as at the time of the training all the java projects we created were made in a text editor for learning purposes (IntelliJ did exist then, we're not talking decades ago!) This activity spun off into getting the project running and building using Maven, which was a learning curve in and of itself, but I succeeded! and with my final commit of the day the project is now in a decent state for further (much needed) development.

**Thoughts:** Looking back on how much I struggled at the time when creating this project and comparing it to now is quite eye opening. I wouldn't have been able to do a fraction of what I completed today back then, I would have been absolutely floored. I'm still no Java expert, and I haven't changed the code much (yet!) but just being able to navigate my way around a new IDE and several new/updated Frameworks all while getting to grips and refactoring poorly written learner code from my past... it's a good feeling, I've held off the imposter syndrome for another day. I HAVE grown as a developer. Feels good :)

**Link to work:** [Java_Zoo_Manager](https://github.com/leon-paul-hart/Java_Zoo_Manager)

---