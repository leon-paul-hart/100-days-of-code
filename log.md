# 100 Days Of Code - Log

## Day 0: May 20, 2020

**Today's Progress**: Publicly committed to the task at my Github.io blog at <https://leon-paul-hart.github.io/>. I set up the blog in Jekyll on Github a while back, but it's finally been put to use today as I don't have twitter or other social media to post to.

**Thoughts:** I think the hardest part for me has been committing to this challenge and starting the ball rolling, for various reasons detailed in my blog post here <https://leon-paul-hart.github.io/blog/adhd/neurodiversity/2020/05/20/ADHD-and-the-100-days-of-code-challenge.html> extended endeavors like this can be problematic for me. With work taking up a lot of my energy too its hard spending a whole day coding and coming back home to do more! But I'm feeling inspired by the latest Microsoft Build conference and I'm excited to get stuck in while the inspiration is flowing, hope I can keep it up if the inspiration starts to falter!

**Link to work:** <https://github.com/leon-paul-hart/leon-paul-hart.github.io>

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
