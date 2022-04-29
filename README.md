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