# Capstone Planning Log

**ALL TIMES ARE IN CST**

* **2022-04-29 10:48AM**: Deciding where I should initially head to figure out
  this project.
* **2022-04-29 11:03AM**: I'm annoyed with typing these date time's out so I'm
  going to automate this with an AutoHotKey script.
* **2022-04-29 11:25AM**: BAM!
  ```
  ^!s::
  FormatTime, CurrentDateTime, A_NowUTC, yyyy-MM-dd HH:mmtt
  SendInput * **%CurrentDateTime%**: 
  return
  ```
* **2022-04-29 11:27AM**: Environment management is probably my biggest hurdle
  because so much of my prior Python dev experience is just making a directory
  and then polluting my system python installation with whatever I want.
* **2022-04-29 11:30AM**: Reading up on Python environments:
  - https://jacobian.org/2019/nov/11/python-environment-2020
  - https://realpython.com/python-virtual-environments-a-primer/
  - https://realpython.com/effective-python-environment/
  - https://realpython.com/dependency-management-python-poetry/
* **2022-04-29 11:54AM**: Whoops, forgot to commit.
* **2022-04-29 11:57AM**: From what I can gather everyone has an opinion, and
  there isn't really a specific path forward. As is usual.
  > If you are just learning, I would go with whatever latest python3 version is
  > in the package repos for your system and just manage the virtualenvs
  > yourself.
  >
  > Ive used poetry and pyenv; they are useful when you are working on python
  > applications that use different python versions. They may introduce unneeded
  > complexity for a beginner. 
* **2022-04-29 12:10PM**: I feel confident that his was the right direction to
  head in, but there are so many options I've hit that wall of indecision
  because I want to make the "right" decision.
* **2022-04-29 12:16PM**: As I read these articles it feels like Poetry is the
  right choice.
* **2022-04-29 13:21PM**: Looking at Poetry docs now.
  https://python-poetry.org/docs/
* **2022-04-29 13:48PM**: Break for lunch.
* **2022-04-29 15:03PM**: Reading through: https://realpython.com/comparing-python-command-line-parsing-libraries-argparse-docopt-click/
* **2022-04-29 16:01PM**: Feeling pretty solid about everything even though I
  haven't put hand to keyboard with any code about this. I'm going to look at
  the documentation for Black now (also Flake8 which I saw mentioned somewhere.)
* **2022-04-29 17:09PM**: Looking over the Porkbun API documentation, and using
  cURL to test it out.
* **2022-04-29 18:02PM**: As expected I've broken something with one of my
  domains. Thankfully it's one that doesn't matter.
* **2022-04-29 18:03PM**: As of this moment I am all read out. I'm going to work
  on some toy examples of building a CLI with Python & Click.
* **2022-05-01 15:05PM**: Found a great article about setting up pre-commit with
  Black & flake8. https://dev.to/m1yag1/how-to-setup-your-project-with-pre-commit-black-and-flake8-183k
* **2022-05-06 10:27AM**: I was able to get pre-commit setup. Right now I'm
  getting myself used to the new workflow that was recommended to me. I'm still
  unsure if this is the kind of workflow you'd want to have in general, but I'm
  rolling with it for now.
  ```mermaid
  graph TD
    a[Need to make changes] --> b[Create new branch off main]
    b --> c[Make and commit changes]
    c --> d[switch back to main]
    d --> e[git merge --squash `branchname` && git commit]
    e --> f[edit commit message]
    f --> g[git push]
    g --> h[git branch -D `branchname`]
    h --> |Realize all the things you did wrong|a
  ```
* **2022-05-06 12:07PM**: It's been slow going with Click, but I feel a little
  more confident right now. As of right now I can check prices for domains, but
  it needs a little more polish, and is honestly one of the simpler functions of
  the application.
* **2022-05-06 17:10PM**: Part of the struggle here is that not only are the
  concepts new & difficult, the language used to express them is new and
  difficult. Jargon will be the death of me.
* **2022-05-15 15:06PM**: What a complete shit show this weekend has been. I hit
  a wall related to how I wanted to structure the CLI, and it was just
  frustration after frustration after that. A firmer understanding of how Click
  intends for it's groups, commands, and options would have been nice before I
  dove in. Maybe diving in is what was required to learn. Regardless I've got
  somewhat of a path forward now so I'm able to start writing out the logic for
  each command & subcommand.
* **2022-05-15 15:32PM**: Making each option a dictionary member feels solid to
  me. We'll see if that holds up in 15 minutes.
* **2022-05-15 16:21PM**: Still feeling pretty good about where I'm heading. Now
  that I'm feeling it I'm able to crank out code for each subcommand, and it's
  fantastic.
* **2022-05-15 17:49PM**: Gotta love getting in the groove and running straight
  into a bug with the API you've based your whole capstone around. Fantastic.