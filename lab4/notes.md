\# Lab 4 Notes



\## Question 1

`--global` makes the setting apply to every repository for your user account on this computer. Without it, Git would save the name and email only in the current repository's `.git/config`, so you would have to set them again in every new repo.



\## Question 2

`.git` appeared. It is a hidden folder, which is why plain `ls` doesn't show it. It holds the whole repository: the commit history, branches, tags, config, and the staging area.



\## Question 3

Git offered to track about \[FILL IN: the number you saw] files and folders. Most of them were inside `.venv/`, which is a virtual environment full of other people's library code that I did not write.



\## Question 4

Everything inside `.venv/` disappeared from the untracked list, along with `\_\_pycache\_\_/` and `.pyc` files. Only my own files remained, plus `.gitignore` itself.



\## Question 5

`.gitignore` should be committed, not ignored. It is part of the project, and committing it means the ignore rules are saved in the history and apply to anyone who clones the repo.



\## Question 6

`README.md` moved from "Untracked files" to "Changes to be committed". In the three-places model, it moved from the working directory to the staging area, ready for the next commit.



\## Question 7

Git printed a line like `\[main (root-commit) abc1234] Lab work so far`, followed by a summary saying \[FILL IN: N] files changed, with the insertions and a list of the created files. "root-commit" shows it was the first commit in the repo.



\## Question 8

The first seven characters are the short commit hash, taken from the commit's full 40-character SHA-1 ID (my own was \[FILL IN: your hash]). They uniquely identify that commit, so I can refer to it in commands like `git show` or `git tag`.



\## Question 9

The loop is: edit or create files, check with `git status`, stage with `git add`, then save with `git commit`. Running `git log` afterwards confirms the new commit is in the history.



\## Question 10

`README.md` is named in capitals and placed at the top level of the repo because GitHub looks for exactly that file and shows it on the repo's front page. It is the first thing a visitor reads, so it works as the project's introduction, unlike ordinary notes files.



\## Question 11

`gh auth login` signed me in through the browser and stored an authentication token on my computer. Because I chose to authenticate Git, Git uses that saved token automatically when I push over HTTPS, so it never asks for a password.



\## Question 12

The front page shows the rendered `README.md`, displayed as formatted text with headings and bullets. GitHub automatically displays the README from the root of a repository below the file list.



\## Question 13

No, pushing did not change my local history. `git push` only copies my local commits to GitHub. The `-u` flag also set `origin/main` as the upstream branch, so a plain `git push` works afterwards.



\## Question 14

A private repository exists on GitHub and is stored there, but only I and the people I invite can see it. If a repository does not exist on GitHub at all, there is nothing stored online: no cloud backup, no link, and no way for the TAs to be given access.

