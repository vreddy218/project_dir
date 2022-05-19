# project_dir

vredd218@LIN33003674 MINGW64 ~ (master)
$ mkdir project_dir
mkdir: cannot create directory ‘project_dir’: File exists

vredd218@LIN33003674 MINGW64 ~ (master)
$ cd project_dir

vredd218@LIN33003674 MINGW64 ~/project_dir (master)
$ git init
Initialized empty Git repository in C:/Users/VREDD218/project_dir/.git/

vredd218@LIN33003674 MINGW64 ~/project_dir (master)
$ touch index.html

vredd218@LIN33003674 MINGW64 ~/project_dir (master)
$ git status
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        index.html

nothing added to commit but untracked files present (use "git add" to track)

vredd218@LIN33003674 MINGW64 ~/project_dir (master)
$ git add index.html

vredd218@LIN33003674 MINGW64 ~/project_dir (master)
$ git commit -m "Adding a new file"
[master (root-commit) c7042db] Adding a new file
 Committer: Reddy Muppana <venkata-sataya-sai-ram.reddy@capgemini.com>
Your name and email address were configured automatically based
on your username and hostname. Please check that they are accurate.
You can suppress this message by setting them explicitly. Run the
following command and follow the instructions in your editor to edit
your configuration file:

    git config --global --edit

After doing this, you may fix the identity used for this commit with:

    git commit --amend --reset-author

 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 index.html

vredd218@LIN33003674 MINGW64 ~/project_dir (master)
$ git status
On branch master
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        New Text Document.txt

nothing added to commit but untracked files present (use "git add" to track)

vredd218@LIN33003674 MINGW64 ~/project_dir (master)
$ git add --all

vredd218@LIN33003674 MINGW64 ~/project_dir (master)
$ git status
On branch master
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   New Text Document.txt


vredd218@LIN33003674 MINGW64 ~/project_dir (master)
$ git commit
Aborting commit due to empty commit message.

vredd218@LIN33003674 MINGW64 ~/project_dir (master)
$ git commit -m "adding a text file"
[master 4f7e67a] adding a text file
 Committer: Reddy Muppana <venkata-sataya-sai-ram.reddy@capgemini.com>
Your name and email address were configured automatically based
on your username and hostname. Please check that they are accurate.
You can suppress this message by setting them explicitly. Run the
following command and follow the instructions in your editor to edit
your configuration file:

    git config --global --edit

After doing this, you may fix the identity used for this commit with:

    git commit --amend --reset-author

 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 New Text Document.txt

vredd218@LIN33003674 MINGW64 ~/project_dir (master)
$ git log
commit 4f7e67a84fcde88551507dabcc69e73eed8e092f (HEAD -> master)
Author: Reddy Muppana <venkata-sataya-sai-ram.reddy@capgemini.com>
Date:   Thu May 19 12:27:49 2022 +0530

    adding a text file

commit c7042dbbafcc5448e55a9eb4f251a70dd0d8a81c
Author: Reddy Muppana <venkata-sataya-sai-ram.reddy@capgemini.com>
Date:   Thu May 19 12:17:26 2022 +0530

    Adding a new file

vredd218@LIN33003674 MINGW64 ~/project_dir (master)
$ git status
On branch master
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   New Text Document.txt

no changes added to commit (use "git add" and/or "git commit -a")

vredd218@LIN33003674 MINGW64 ~/project_dir (master)
$ git add .

vredd218@LIN33003674 MINGW64 ~/project_dir (master)
$ git status
On branch master
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   New Text Document.txt


vredd218@LIN33003674 MINGW64 ~/project_dir (master)
$ git config --help

vredd218@LIN33003674 MINGW64 ~/project_dir (master)
$ git config
usage: git config [<options>]

Config file location
    --global              use global config file
    --system              use system config file
    --local               use repository config file
    --worktree            use per-worktree config file
    -f, --file <file>     use given config file
    --blob <blob-id>      read config from given blob object

Action
    --get                 get value: name [value-pattern]
    --get-all             get all values: key [value-pattern]
    --get-regexp          get values for regexp: name-regex [value-pattern]
    --get-urlmatch        get value specific for the URL: section[.var] URL
    --replace-all         replace all matching variables: name value [value-pattern]
    --add                 add a new variable: name value
    --unset               remove a variable: name [value-pattern]
    --unset-all           remove all matches: name [value-pattern]
    --rename-section      rename section: old-name new-name
    --remove-section      remove a section: name
    -l, --list            list all
    --fixed-value         use string equality when comparing values to 'value-pattern'
    -e, --edit            open an editor
    --get-color           find the color configured: slot [default]
    --get-colorbool       find the color setting: slot [stdout-is-tty]

Type
    -t, --type <>         value is given this type
    --bool                value is "true" or "false"
    --int                 value is decimal number
    --bool-or-int         value is --bool or --int
    --bool-or-str         value is --bool or string
    --path                value is a path (file or directory name)
    --expiry-date         value is an expiry date

Other
    -z, --null            terminate values with NUL byte
    --name-only           show variable names only
    --includes            respect include directives on lookup
    --show-origin         show origin of config (file, standard input, blob, command line)
    --show-scope          show scope of config (worktree, local, global, system, command)
    --default <value>     with --get, use default value when missing entry


vredd218@LIN33003674 MINGW64 ~/project_dir (master)
$ git status
On branch master
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   New Text Document.txt


vredd218@LIN33003674 MINGW64 ~/project_dir (master)
$ git ls-files
New Text Document.txt
index.html

vredd218@LIN33003674 MINGW64 ~/project_dir (master)
$ git status
On branch master
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   New Text Document.txt

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   index.html


vredd218@LIN33003674 MINGW64 ~/project_dir (master)
$ git add index.html

vredd218@LIN33003674 MINGW64 ~/project_dir (master)
$ git status
On branch master
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   New Text Document.txt
        modified:   index.html


vredd218@LIN33003674 MINGW64 ~/project_dir (master)
$ git log
commit 4f7e67a84fcde88551507dabcc69e73eed8e092f (HEAD -> master)
Author: Reddy Muppana <venkata-sataya-sai-ram.reddy@capgemini.com>
Date:   Thu May 19 12:27:49 2022 +0530

    adding a text file

commit c7042dbbafcc5448e55a9eb4f251a70dd0d8a81c
Author: Reddy Muppana <venkata-sataya-sai-ram.reddy@capgemini.com>
Date:   Thu May 19 12:17:26 2022 +0530

    Adding a new file

vredd218@LIN33003674 MINGW64 ~/project_dir (master)
$ git log --all
commit 4f7e67a84fcde88551507dabcc69e73eed8e092f (HEAD -> master)
Author: Reddy Muppana <venkata-sataya-sai-ram.reddy@capgemini.com>
Date:   Thu May 19 12:27:49 2022 +0530

    adding a text file

commit c7042dbbafcc5448e55a9eb4f251a70dd0d8a81c
Author: Reddy Muppana <venkata-sataya-sai-ram.reddy@capgemini.com>
Date:   Thu May 19 12:17:26 2022 +0530

    Adding a new file

vredd218@LIN33003674 MINGW64 ~/project_dir (master)
$ git revert
usage: git revert [<options>] <commit-ish>...
   or: git revert <subcommand>

    --quit                end revert or cherry-pick sequence
    --continue            resume revert or cherry-pick sequence
    --abort               cancel revert or cherry-pick sequence
    --skip                skip current commit and continue
    --cleanup <mode>      how to strip spaces and #comments from message
    -n, --no-commit       don't automatically commit
    -e, --edit            edit the commit message
    -s, --signoff         add a Signed-off-by trailer
    -m, --mainline <parent-number>
                          select mainline parent
    --rerere-autoupdate   update the index with reused conflict resolution if possible
    --strategy <strategy>
                          merge strategy
    -X, --strategy-option <option>
                          option for merge strategy
    -S, --gpg-sign[=<key-id>]
                          GPG sign commit


vredd218@LIN33003674 MINGW64 ~/project_dir (master)
$ git status
On branch master
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   New Text Document.txt
        modified:   index.html

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   index.html


vredd218@LIN33003674 MINGW64 ~/project_dir (master)
$ git add index.html

vredd218@LIN33003674 MINGW64 ~/project_dir (master)
$ git status
On branch master
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   New Text Document.txt
        modified:   index.html


vredd218@LIN33003674 MINGW64 ~/project_dir (master)
$ git mv add my-add
fatal: bad source, source=add, destination=my-add

vredd218@LIN33003674 MINGW64 ~/project_dir (master)
$
vredd218@LIN33003674 MINGW64 ~/project_dir (master)
$ git revert
usage: git revert [<options>] <commit-ish>...
   or: git revert <subcommand>

    --quit                end revert or cherry-pick sequence
    --continue            resume revert or cherry-pick sequence
    --abort               cancel revert or cherry-pick sequence
    --skip                skip current commit and continue
    --cleanup <mode>      how to strip spaces and #comments from message
    -n, --no-commit       don't automatically commit
    -e, --edit            edit the commit message
    -s, --signoff         add a Signed-off-by trailer
    -m, --mainline <parent-number>
                          select mainline parent
    --rerere-autoupdate   update the index with reused conflict resolution if possible
    --strategy <strategy>
                          merge strategy
    -X, --strategy-option <option>
                          option for merge strategy
    -S, --gpg-sign[=<key-id>]
                          GPG sign commit


vredd218@LIN33003674 MINGW64 ~/project_dir (master)
$ git stage index.html

vredd218@LIN33003674 MINGW64 ~/project_dir (master)
$ git status
On branch master
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   New Text Document.txt
        modified:   index.html


vredd218@LIN33003674 MINGW64 ~/project_dir (master)
$ git add 'i would rename it to' git my-add
fatal: pathspec 'i would rename it to' did not match any files

vredd218@LIN33003674 MINGW64 ~/project_dir (master)
$ mkdir git_revert_test

vredd218@LIN33003674 MINGW64 ~/project_dir (master)
$ cd git_revert_test

vredd218@LIN33003674 MINGW64 ~/project_dir/git_revert_test (master)
$ git status
On branch master
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   ../New Text Document.txt
        modified:   ../index.html


vredd218@LIN33003674 MINGW64 ~/project_dir/git_revert_test (master)
$ git my-add index.html
git: 'my-add' is not a git command. See 'git --help'.

vredd218@LIN33003674 MINGW64 ~/project_dir/git_revert_test (master)
$ git- --help
bash: git-: command not found

vredd218@LIN33003674 MINGW64 ~/project_dir/git_revert_test (master)
$ git --help
usage: git [--version] [--help] [-C <path>] [-c <name>=<value>]
           [--exec-path[=<path>]] [--html-path] [--man-path] [--info-path]
           [-p | --paginate | -P | --no-pager] [--no-replace-objects] [--bare]
           [--git-dir=<path>] [--work-tree=<path>] [--namespace=<name>]
           [--super-prefix=<path>] [--config-env=<name>=<envvar>]
           <command> [<args>]

These are common Git commands used in various situations:

start a working area (see also: git help tutorial)
   clone     Clone a repository into a new directory
   init      Create an empty Git repository or reinitialize an existing one

work on the current change (see also: git help everyday)
   add       Add file contents to the index
   mv        Move or rename a file, a directory, or a symlink
   restore   Restore working tree files
   rm        Remove files from the working tree and from the index

examine the history and state (see also: git help revisions)
   bisect    Use binary search to find the commit that introduced a bug
   diff      Show changes between commits, commit and working tree, etc
   grep      Print lines matching a pattern
   log       Show commit logs
   show      Show various types of objects
   status    Show the working tree status

grow, mark and tweak your common history
   branch    List, create, or delete branches
   commit    Record changes to the repository
   merge     Join two or more development histories together
   rebase    Reapply commits on top of another base tip
   reset     Reset current HEAD to the specified state
   switch    Switch branches
   tag       Create, list, delete or verify a tag object signed with GPG

collaborate (see also: git help workflows)
   fetch     Download objects and refs from another repository
   pull      Fetch from and integrate with another repository or a local branch
   push      Update remote refs along with associated objects

'git help -a' and 'git help -g' list available subcommands and some
concept guides. See 'git help <command>' or 'git help <concept>'
to read about a specific subcommand or concept.
See 'git help git' for an overview of the system.


