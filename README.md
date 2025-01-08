PS E:\web design\learn git\HELLO-GIT> git init
Initialized empty Git repository in E:/web design/learn git/HELLO-GIT/.git/
PS E:\web design\learn git\HELLO-GIT> pwd

Path
----
E:\web design\learn git\HELLO-GIT


PS E:\web design\learn git\HELLO-GIT> ls


    Directory: E:\web design\learn git\HELLO-GIT


Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
-a----        07-01-2025     19:37             19 hello.txt        


PS E:\web design\learn git\HELLO-GIT> ls -a
Get-ChildItem : Parameter cannot be processed because the 
parameter name 'a' is ambiguous. Possible matches include:
-Attributes -Directory -File -Hidden -ReadOnly -System.
At line:1 char:4
+ ls -a
+    ~~
    + CategoryInfo          : InvalidArgument: (:) [Get-ChildItem  
   ], ParameterBindingException
    + FullyQualifiedErrorId : AmbiguousParameter,Microsoft.PowerS  
   hell.Commands.GetChildItemCommand

PS E:\web design\learn git\HELLO-GIT> ls -a
Get-ChildItem : Parameter cannot be processed because the 
parameter name 'a' is ambiguous. Possible matches include:
-Attributes -Directory -File -Hidden -ReadOnly -System.
At line:1 char:4
+ ls -a
+    ~~
    + CategoryInfo          : InvalidArgument: (:) [Get-ChildItem  
   ], ParameterBindingException
    + FullyQualifiedErrorId : AmbiguousParameter,Microsoft.PowerS  
   hell.Commands.GetChildItemCommand

PS E:\web design\learn git\HELLO-GIT> -a
-a : The term '-a' is not recognized as the name of a cmdlet, 
function, script file, or operable program. Check the spelling of  
the name, or if a path was included, verify that the path is       
correct and try again.
At line:1 char:1
+ -a
+ ~~
    + CategoryInfo          : ObjectNotFound: (-a:String) [], Com  
   mandNotFoundException
    + FullyQualifiedErrorId : CommandNotFoundException

PS E:\web design\learn git\HELLO-GIT> ls ----a----
ls : Cannot find path 'E:\web design\learn 
git\HELLO-GIT\----a----' because it does not exist.
At line:1 char:1
+ ls ----a----
+ ~~~~~~~~~~~~
    + CategoryInfo          : ObjectNotFound: (E:\web design\l...  
   O-GIT\----a----:String) [Get-ChildItem], ItemNotFoundExceptio   
  n
    + FullyQualifiedErrorId : PathNotFound,Microsoft.PowerShell.C 
   ommands.GetChildItemCommand

PS E:\web design\learn git\HELLO-GIT> ls-a
ls-a : The term 'ls-a' is not recognized as the name of a cmdlet, 
function, script file, or operable program. Check the spelling of  
the name, or if a path was included, verify that the path is       
correct and try again.
At line:1 char:1
+ ls-a
+ ~~~~
    + CategoryInfo          : ObjectNotFound: (ls-a:String) [], C  
   ommandNotFoundException
    + FullyQualifiedErrorId : CommandNotFoundException

PS E:\web design\learn git\HELLO-GIT> .git
.git : The term '.git' is not recognized as the name of a cmdlet, 
function, script file, or operable program. Check the spelling of  
the name, or if a path was included, verify that the path is
correct and try again.
At line:1 char:1
+ .git
+ ~~~~
    + CategoryInfo          : ObjectNotFound: (.git:String) [], C      
   ommandNotFoundException
    + FullyQualifiedErrorId : CommandNotFoundException

PS E:\web design\learn git\HELLO-GIT> cd .git
PS E:\web design\learn git\HELLO-GIT\.git> ls


    Directory: E:\web design\learn git\HELLO-GIT\.git


Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
d-----        07-01-2025     19:37                hooks
d-----        07-01-2025     19:37                info
d-----        07-01-2025     19:37                objects
d-----        07-01-2025     19:37                refs
-a----        07-01-2025     19:37            130 config
-a----        07-01-2025     19:37             73 description
-a----        07-01-2025     19:37             23 HEAD


PS E:\web design\learn git\HELLO-GIT\.git> git add hello.txt
fatal: this operation must be run in a work tree
PS E:\web design\learn git\HELLO-GIT\.git> git add hello.txt
fatal: this operation must be run in a work tree
PS E:\web design\learn git\HELLO-GIT\.git> git add hello.txt
fatal: this operation must be run in a work tree
PS E:\web design\learn git\HELLO-GIT\.git> git add <hello.txt>
At line:1 char:9
+ git add <hello.txt>
+         ~
The '<' operator is reserved for future use.
    + CategoryInfo          : ParserError: (:) [], ParentContainsErro  
   rRecordException
    + FullyQualifiedErrorId : RedirectionNotSupported
 
PS E:\web design\learn git\HELLO-GIT\.git> git add hello
fatal: this operation must be run in a work tree
PS E:\web design\learn git\HELLO-GIT\.git> git init
Initialized empty Git repository in E:/web design/learn git/HELLO-GIT/.git/.git/
PS E:\web design\learn git\HELLO-GIT\.git> cd HELLO-GIT
cd : Cannot find path 'E:\web design\learn 
git\HELLO-GIT\.git\HELLO-GIT' because it does not exist.
At line:1 char:1
+ cd HELLO-GIT
+ ~~~~~~~~~~~~
    + CategoryInfo          : ObjectNotFound: (E:\web design\l...\.gi  
   t\HELLO-GIT:String) [Set-Location], ItemNotFoundException
    + FullyQualifiedErrorId : PathNotFound,Microsoft.PowerShell.Comma  
   nds.SetLocationCommand

PS E:\web design\learn git\HELLO-GIT\.git> cd..
PS E:\web design\learn git\HELLO-GIT> git init
Reinitialized existing Git repository in E:/web design/learn git/HELLO-GIT/.git/
PS E:\web design\learn git\HELLO-GIT> ls


    Directory: E:\web design\learn git\HELLO-GIT


----                 -------------         ------ ----
----                 -------------         ------ ----
-a----        07-01-2025     19:44              0 hello-2.txt
-a----        07-01-2025     19:45             19 hello.txt


PS E:\web design\learn git\HELLO-GIT> cd .git
PS E:\web design\learn git\HELLO-GIT\.git> git status
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)       
        HEAD
        config
        description
        hooks/
        info/

nothing added to commit but untracked files present (use "git add" to track)
PS E:\web design\learn git\HELLO-GIT\.git> cd..
PS E:\web design\learn git\HELLO-GIT> git add hello.txt
PS E:\web design\learn git\HELLO-GIT> git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   hello.txt

Untracked files:
  (use "git add <file>..." to include in what will be committed)       
        hello-2.txt

PS E:\web design\learn git\HELLO-GIT> git init
Reinitialized existing Git repository in E:/web design/learn git/HELLO-GIT/.git/
PS E:\web design\learn git\HELLO-GIT> git add hello.txt 
PS E:\web design\learn git\HELLO-GIT> git add .
PS E:\web design\learn git\HELLO-GIT> cd .git
PS E:\web design\learn git\HELLO-GIT\.git> ls


    Directory: E:\web design\learn git\HELLO-GIT\.git


Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
d-----        07-01-2025     19:37                hooks
d-----        07-01-2025     19:37                info
d-----        07-01-2025     19:50                objects
d-----        07-01-2025     19:37                refs
-a----        07-01-2025     19:51            130 config
-a----        07-01-2025     19:37             73 description
-a----        07-01-2025     19:37             23 HEAD
-a----        07-01-2025     19:52            184 index


PS E:\web design\learn git\HELLO-GIT\.git> dir -h


    Directory: E:\web design\learn git\HELLO-GIT\.git


Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
d--h--        07-01-2025     19:49                .git


PS E:\web design\learn git\HELLO-GIT\.git> cat index
DIRCg}6»'3½8g}6»'3½8¤æâ›²ÑÖCK‹)®wZØÂäŒS‘
hello-2.txtg}53Ž”¸g}7)zAÔ¤Î‚ƒÛïLt&zœ€ž1Kñ       hello.txtWÆ:UK°²Z36žïd¡lv˜k
PS E:\web design\learn git\HELLO-GIT\.git> cd..
PS E:\web design\learn git\HELLO-GIT> git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   hello-2.txt
        new file:   hello.txt

PS E:\web design\learn git\HELLO-GIT>  git commit -m "add v0 feature to hello"
[master (root-commit) 81405f8] add v0 feature to hello
 2 files changed, 1 insertion(+)
 create mode 100644 hello-2.txt
 create mode 100644 hello.txt
PS E:\web design\learn git\HELLO-GIT> git status
On branch master
nothing to commit, working tree clean
PS E:\web design\learn git\HELLO-GIT> git log
commit 81405f8da8f6c5a68a3b6807b48c29070814429f (HEAD -> master)
Author: maurya-kavi <kavindramehta60@gmail.com>
Date:   Tue Jan 7 20:10:51 2025 +0530

    add v0 feature to hello
PS E:\web design\learn git\HELLO-GIT> git diff
PS E:\web design\learn git\HELLO-GIT> git diff 81405f8da8f6c5a68a3b6807b48c29070814429f
PS E:\web design\learn git\HELLO-GIT> git status
On branch master
nothing to commit, working tree clean
PS E:\web design\learn git\HELLO-GIT> cd hello.txt
At line:1 char:1
At line:1 char:1
+ cd hello.txt
+ ~~~~~~~~~~~~
    + CategoryInfo          : ObjectNotFound: (hello.txt:String) [Set  
   -Location], ItemNotFoundException
    + FullyQualifiedErrorId : PathNotFound,Microsoft.PowerShell.Comma  
   nds.SetLocationCommand

PS E:\web design\learn git\HELLO-GIT> cd hello
cd : Cannot find path 'E:\web design\learn git\HELLO-GIT\hello'        
because it does not exist.
At line:1 char:1
+ cd hello
+ ~~~~~~~~
    + CategoryInfo          : ObjectNotFound: (E:\web design\learn gi  
   t\HELLO-GIT\hello:String) [Set-Location], ItemNotFoundException     
    + FullyQualifiedErrorId : PathNotFound,Microsoft.PowerShell.Comma  
   nds.SetLocationCommand

PS E:\web design\learn git\HELLO-GIT> git diff
PS E:\web design\learn git\HELLO-GIT> git init
Reinitialized existing Git repository in E:/web design/learn git/HELLO-GIT/.git/
PS E:\web design\learn git\HELLO-GIT> git diff
PS E:\web design\learn git\HELLO-GIT> git diff
diff --git a/hello.txt b/hello.txt
index ce8283d..684dbdf 100644
--- a/hello.txt
+++ b/hello.txt
@@ -1 +1 @@
-Hello World I am V0
\ No newline at end of file
+Hello World I am V1
\ No newline at end of file
PS E:\web design\learn git\HELLO-GIT> git add .
PS E:\web design\learn git\HELLO-GIT> git diff
PS E:\web design\learn git\HELLO-GIT> git add a.txt
PS E:\web design\learn git\HELLO-GIT> git init
Reinitialized existing Git repository in E:/web design/learn git/HELLO-GIT/.git/
PS E:\web design\learn git\HELLO-GIT> git a.txt
git: 'a.txt' is not a git command. See 'git --help'.
PS E:\web design\learn git\HELLO-GIT> git add a.txt
PS E:\web design\learn git\HELLO-GIT> git add a.txt
PS E:\web design\learn git\HELLO-GIT> git diff
PS E:\web design\learn git\HELLO-GIT> git log
commit 81405f8da8f6c5a68a3b6807b48c29070814429f (HEAD -> master)
Author: maurya-kavi <kavindramehta60@gmail.com>
Date:   Tue Jan 7 20:10:51 2025 +0530

    add v0 feature to hello
PS E:\web design\learn git\HELLO-GIT> git status
On branch master
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   a.txt
        modified:   hello.txt

PS E:\web design\learn git\HELLO-GIT> git log
commit 81405f8da8f6c5a68a3b6807b48c29070814429f (HEAD -> master)
Author: maurya-kavi <kavindramehta60@gmail.com>
Date:   Tue Jan 7 20:10:51 2025 +0530

    add v0 feature to hello
PS E:\web design\learn git\HELLO-GIT> git status
On branch master
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   a.txt
        modified:   hello.txt

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   hello-2.txt

PS E:\web design\learn git\HELLO-GIT> git add hello-2.txt
PS E:\web design\learn git\HELLO-GIT> git log
commit 81405f8da8f6c5a68a3b6807b48c29070814429f (HEAD -> master)
Author: maurya-kavi <kavindramehta60@gmail.com>
Date:   Tue Jan 7 20:10:51 2025 +0530

    add v0 feature to hello
PS E:\web design\learn git\HELLO-GIT> git status
On branch master
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   a.txt
        modified:   hello-2.txt
        modified:   hello.txt

PS E:\web design\learn git\HELLO-GIT> git log 
commit 81405f8da8f6c5a68a3b6807b48c29070814429f (HEAD -> master)
Author: maurya-kavi <kavindramehta60@gmail.com>
Date:   Tue Jan 7 20:10:51 2025 +0530

    add v0 feature to hello
PS E:\web design\learn git\HELLO-GIT> cd .git
PS E:\web design\learn git\HELLO-GIT\.git> cd objects
PS E:\web design\learn git\HELLO-GIT\.git\objects> ls


    Directory: E:\web design\learn git\HELLO-GIT\.git\objects


Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
d-----        08-01-2025     12:11                68
d-----        07-01-2025     20:10                81
d-----        08-01-2025     12:11                89
d-----        07-01-2025     20:10                8d
d-----        08-01-2025     12:24                91
d-----        07-01-2025     19:50                ce
d-----        07-01-2025     19:52                e6
d-----        07-01-2025     19:37                info
d-----        07-01-2025     19:37                pack


PS E:\web design\learn git\HELLO-GIT\.git\objects> cd 81
PS E:\web design\learn git\HELLO-GIT\.git\objects\81> cd..
PS E:\web design\learn git\HELLO-GIT\.git\objects> cd..
PS E:\web design\learn git\HELLO-GIT\.git> cd..
PS E:\web design\learn git\HELLO-GIT> pwd

Path
----
E:\web design\learn git\HELLO-GIT


PS E:\web design\learn git\HELLO-GIT> cd objects
cd : Cannot find path 'E:\web design\learn git\HELLO-GIT\objects' 
because it does not exist.
At line:1 char:1
+ cd objects
+ ~~~~~~~~~~
    + CategoryInfo          : ObjectNotFound: (E:\web design\l...LLO-  
   GIT\objects:String) [Set-Location], ItemNotFoundException
    + FullyQualifiedErrorId : PathNotFound,Microsoft.PowerShell.Comma  
   nds.SetLocationCommand

PS E:\web design\learn git\HELLO-GIT> ls


    Directory: E:\web design\learn git\HELLO-GIT


Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
-a----        08-01-2025     12:11             11 a.txt
-a----        08-01-2025     12:23             14 hello-2.txt
-a----        08-01-2025     12:09             19 hello.txt


PS E:\web design\learn git\HELLO-GIT> cat 81405f8da8f6c5a68a3b6807b48c29070814429f
cat : Cannot find path 'E:\web design\learn 
git\HELLO-GIT\81405f8da8f6c5a68a3b6807b48c29070814429f' because it     
does not exist.
At line:1 char:1
+ cat 81405f8da8f6c5a68a3b6807b48c29070814429f
+ ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
    + CategoryInfo          : ObjectNotFound: (E:\web design\l...48c2 
   9070814429f:String) [Get-Content], ItemNotFoundException
    + FullyQualifiedErrorId : PathNotFound,Microsoft.PowerShell.Comma  
   nds.GetContentCommand

PS E:\web design\learn git\HELLO-GIT> cd .git
PS E:\web design\learn git\HELLO-GIT\.git> git cat-file -p 81405f8da8f6c5a68a3b6807b48c29070814429f
fatal: Not a valid object name 81405f8da8f6c5a68a3b6807b48c29070814429f
PS E:\web design\learn git\HELLO-GIT\.git> git cat-file 81405f8da8f6c5a68a3b6807b48c29070814429f
fatal: only two arguments allowed in <type> <object> mode, not 1

usage: git cat-file <type> <object>
   or: git cat-file (-e | -p) <object>
   or: git cat-file (-t | -s) [--allow-unknown-type] <object>
   or: git cat-file (--textconv | --filters)
                    [<rev>:<path|tree-ish> | --path=<path|tree-ish> <rev>]
   or: git cat-file (--batch | --batch-check | --batch-command) [--batch-all-objects]
                    [--buffer] [--follow-symlinks] [--unordered]       
                    [--textconv | --filters] [-Z]

Check object existence or emit object contents
    -e                    check if <object> exists
    -p                    pretty-print <object> content

Emit [broken] object attributes
    -t                    show object type (one of 'blob', 'tree', 'commit', 'tag', ...)
    -s                    show object size
    --[no-]allow-unknown-type
                          allow -s and -t to work with broken/corrupt objects
    --[no-]use-mailmap    use mail map file
    --[no-]mailmap ...    alias of --use-mailmap

Batch objects requested on stdin (or --batch-all-objects)
    --batch[=<format>]    show full <object> or <rev> contents
    --batch-check[=<format>]
                          like --batch, but don't emit <contents>      
    -Z                    stdin and stdout is NUL-terminated
    --batch-command[=<format>]
                          read commands from stdin
    --batch-all-objects   with --batch[-check]: ignores stdin, batches all known objects

Change or optimize batch output
    --[no-]buffer         buffer --batch output
    --[no-]follow-symlinks
                          follow in-tree symlinks
    --[no-]unordered      do not order objects before emitting them    

Emit object (blob or tree) with conversion or filter (stand-alone, or with batch)
    --textconv            run textconv on object's content
    --filters             run filters on object's content
    --[no-]path blob|tree use a <path> for (--textconv | --filters); Not with 'batch'

PS E:\web design\learn git\HELLO-GIT\.git> git cat-file -p 81405f8da8f6c5a68a3b6807b48c29070814429f
fatal: Not a valid object name 81405f8da8f6c5a68a3b6807b48c29070814429f
PS E:\web design\learn git\HELLO-GIT\.git> git cat-file -e 81405f8da8f6c5a68a3b6807b48c29070814429f
PS E:\web design\learn git\HELLO-GIT\.git> cat indx
cat : Cannot find path 'E:\web design\learn git\HELLO-GIT\.git\indx' 
because it does not exist.
At line:1 char:1
+ cat indx
+ ~~~~~~~~
    + CategoryInfo          : ObjectNotFound: (E:\web design\l...O-GI  
   T\.git\indx:String) [Get-Content], ItemNotFoundException
    + FullyQualifiedErrorId : PathNotFound,Microsoft.PowerShell.Comma  
   nds.GetContentCommand

PS E:\web design\learn git\HELLO-GIT\.git> cat index
DIRCg~ñ<Äg~ÿ7!s\¤
‰•Õ£„;É¸Ö—©Ç²¥{Tœ•a.txtg}6»'3½8g~ ÷^¤‘æRdÝ]LÐZsgØà1žy
hello-2.txtg}53Ž”¸g~½¸¤hM½ú€[®·?;ÅãFm©,ÇÔ       hello.txtTREE-1 0      
l;HïKÑ9„ÿ¥žô®Ð–
B/
PS E:\web design\learn git\HELLO-GIT\.git> cd..
PS E:\web design\learn git\HELLO-GIT> cat index
cat : Cannot find path 'E:\web design\learn git\HELLO-GIT\index' 
because it does not exist.
At line:1 char:1
+ cat index
+ ~~~~~~~~~
    + CategoryInfo          : ObjectNotFound: (E:\web design\learn gi  
   t\HELLO-GIT\index:String) [Get-Content], ItemNotFoundException      
    + FullyQualifiedErrorId : PathNotFound,Microsoft.PowerShell.Comma  
   nds.GetContentCommand

PS E:\web design\learn git\HELLO-GIT> git commit -m "this is my version 2"
[master 98f0e87] this is my version 2
 3 files changed, 3 insertions(+), 1 deletion(-)
 create mode 100644 a.txt
PS E:\web design\learn git\HELLO-GIT> git log
commit 98f0e87589cc92e88cfc29f75cbdb97f51fe9116 (HEAD -> master)
Author: maurya-kavi <kavindramehta60@gmail.com>
Date:   Wed Jan 8 13:08:20 2025 +0530

    this is my version 2

commit 81405f8da8f6c5a68a3b6807b48c29070814429f
Author: maurya-kavi <kavindramehta60@gmail.com>
Date:   Tue Jan 7 20:10:51 2025 +0530

    add v0 feature to hello
PS E:\web design\learn git\HELLO-GIT>  cd .git
PS E:\web design\learn git\HELLO-GIT\.git> ls


    Directory: E:\web design\learn git\HELLO-GIT\.git


Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
d-----        07-01-2025     19:37                hooks
d-----        07-01-2025     19:37                info
d-----        07-01-2025     20:10                logs
d-----        08-01-2025     13:08                objects
d-----        07-01-2025     19:37                refs
-a----        08-01-2025     13:08             21 COMMIT_EDITMSG       
-a----        08-01-2025     12:14            130 config
-a----        07-01-2025     19:37             73 description
-a----        07-01-2025     19:37             23 HEAD
-a----        08-01-2025     13:08            289 index


PS E:\web design\learn git\HELLO-GIT\.git> cat config
[core]
        repositoryformatversion = 0
        filemode = false
        bare = false
        logallrefupdates = true
        symlinks = false
        ignorecase = true
PS E:\web design\learn git\HELLO-GIT\.git> cd..
PS E:\web design\learn git\HELLO-GIT> git remote add origin https://github.com/maurya-kavi/Master-Git-GitHub.git
PS E:\web design\learn git\HELLO-GIT> git remote -v
origin  https://github.com/maurya-kavi/Master-Git-GitHub.git (fetch)
origin  https://github.com/maurya-kavi/Master-Git-GitHub.git (push)    
PS E:\web design\learn git\HELLO-GIT> git push -u origin main
error: src refspec main does not match any
error: failed to push some refs to 'https://github.com/maurya-kavi/Master-Git-GitHub.git'
PS E:\web design\learn git\HELLO-GIT> git push -u origin main
error: src refspec main does not match any
error: failed to push some refs to 'https://github.com/maurya-kavi/Master-Git-GitHub.git'
PS E:\web design\learn git\HELLO-GIT> git branch -M main
PS E:\web design\learn git\HELLO-GIT> git push -u origin main
Enumerating objects: 9, done.
Counting objects: 100% (9/9), done.
Delta compression using up to 16 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (9/9), 622 bytes | 622.00 KiB/s, done.
Total 9 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/maurya-kavi/Master-Git-GitHub.git
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.
PS E:\web design\learn git\HELLO-GIT> git cat-file -t ^C
PS E:\web design\learn git\HELLO-GIT> git cat-file -t Commit 98f0e87
>>
fatal: too many arguments

usage: git cat-file <type> <object>
   or: git cat-file (-e | -p) <object>
   or: git cat-file (-t | -s) [--allow-unknown-type] <object>
   or: git cat-file (--textconv | --filters)
                    [<rev>:<path|tree-ish> | --path=<path|tree-ish> <rev>]
   or: git cat-file (--batch | --batch-check | --batch-command) [--batch-all-objects]
                    [--buffer] [--follow-symlinks] [--unordered]       
                    [--textconv | --filters] [-Z]

Check object existence or emit object contents
    -e                    check if <object> exists
    -p                    pretty-print <object> content

Emit [broken] object attributes
    -t                    show object type (one of 'blob', 'tree', 'commit', 'tag', ...)
    -s                    show object size
    --[no-]allow-unknown-type
                          allow -s and -t to work with broken/corrupt objects
    --[no-]use-mailmap    use mail map file
    --[no-]mailmap ...    alias of --use-mailmap

Batch objects requested on stdin (or --batch-all-objects)
    --batch[=<format>]    show full <object> or <rev> contents
    --batch-check[=<format>]
                          like --batch, but don't emit <contents>      
    -Z                    stdin and stdout is NUL-terminated
    --batch-command[=<format>]
                          read commands from stdin
    --batch-all-objects   with --batch[-check]: ignores stdin, batches all known objects

Change or optimize batch output
    --[no-]buffer         buffer --batch output
    --[no-]follow-symlinks
                          follow in-tree symlinks
    --[no-]unordered      do not order objects before emitting them    

Emit object (blob or tree) with conversion or filter (stand-alone, or with batch)
    --textconv            run textconv on object's content
    --filters             run filters on object's content
    --[no-]path blob|tree use a <path> for (--textconv | --filters); Not with 'batch'

PS E:\web design\learn git\HELLO-GIT> cd .git     
PS E:\web design\learn git\HELLO-GIT\.git> cd objects
PS E:\web design\learn git\HELLO-GIT\.git\objects> cd 98
PS E:\web design\learn git\HELLO-GIT\.git\objects\98> cd..
PS E:\web design\learn git\HELLO-GIT\.git\objects> cd..
PS E:\web design\learn git\HELLO-GIT\.git> cd....
cd.... : The term 'cd....' is not recognized as the name of a cmdlet, 
function, script file, or operable program. Check the spelling of the  
name, or if a path was included, verify that the path is correct and   
try again.
At line:1 char:1
+ cd....
+ ~~~~~~
    + CategoryInfo          : ObjectNotFound: (cd....:String) [], Com  
   mandNotFoundException
    + FullyQualifiedErrorId : CommandNotFoundException

PS E:\web design\learn git\HELLO-GIT\.git> cd object
cd : Cannot find path 'E:\web design\learn git\HELLO-GIT\.git\object' 
because it does not exist.
At line:1 char:1
+ cd object
+ ~~~~~~~~~
    + CategoryInfo          : ObjectNotFound: (E:\web design\l...GIT\  
   .git\object:String) [Set-Location], ItemNotFoundException
    + FullyQualifiedErrorId : PathNotFound,Microsoft.PowerShell.Comma  
   nds.SetLocationCommand

PS E:\web design\learn git\HELLO-GIT\.git> cd objects
PS E:\web design\learn git\HELLO-GIT\.git\objects> cd....
cd.... : The term 'cd....' is not recognized as the name of a cmdlet, 
function, script file, or operable program. Check the spelling of the  
name, or if a path was included, verify that the path is correct and   
try again.
At line:1 char:1
+ cd....
+ ~~~~~~
    + CategoryInfo          : ObjectNotFound: (cd....:String) [], Com  
   mandNotFoundException
    + FullyQualifiedErrorId : CommandNotFoundException

PS E:\web design\learn git\HELLO-GIT\.git\objects> cd.. ..
PS E:\web design\learn git\HELLO-GIT\.git> cd..
PS E:\web design\learn git\HELLO-GIT> git add .
PS E:\web design\learn git\HELLO-GIT> git commit -m "change to v4"
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean
PS E:\web design\learn git\HELLO-GIT> git push
Everything up-to-date
PS E:\web design\learn git\HELLO-GIT> git status
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean
PS E:\web design\learn git\HELLO-GIT> git add.
git: 'add.' is not a git command. See 'git --help'.

The most similar command is
        add
PS E:\web design\learn git\HELLO-GIT> git add .
PS E:\web design\learn git\HELLO-GIT> git commit -m "chage to v4"
[main de2e922] chage to v4
 1 file changed, 1 insertion(+), 1 deletion(-)
PS E:\web design\learn git\HELLO-GIT> git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 16 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 275 bytes | 275.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.   
To https://github.com/maurya-kavi/Master-Git-GitHub.git
   98f0e87..de2e922  main -> main
PS E:\web design\learn git\HELLO-GIT> git branch -M main
PS E:\web design\learn git\HELLO-GIT> git push -u origin main
branch 'main' set up to track 'origin/main'.
Everything up-to-date
PS E:\web design\learn git\HELLO-GIT> git log
commit de2e922c9aed494355a94ed1ab295364dbaf5e29 (HEAD -> main, origin/main)
Author: maurya-kavi <kavindramehta60@gmail.com>
Date:   Wed Jan 8 14:32:33 2025 +0530

    chage to v4

commit 98f0e87589cc92e88cfc29f75cbdb97f51fe9116
Author: maurya-kavi <kavindramehta60@gmail.com>
Date:   Wed Jan 8 13:08:20 2025 +0530

    this is my version 2

commit 81405f8da8f6c5a68a3b6807b48c29070814429f
Author: maurya-kavi <kavindramehta60@gmail.com>
Date:   Tue Jan 7 20:10:51 2025 +0530

    add v0 feature to hello
PS E:\web design\learn git\HELLO-GIT> git cat
git: 'cat' is not a git command. See 'git --help'.

The most similar commands are
        clean
        mktag
        stage
        stash
        tag
        var
PS E:\web design\learn git\HELLO-GIT> cat index
cat : Cannot find path 'E:\web design\learn git\HELLO-GIT\index' 
because it does not exist.
At line:1 char:1
+ cat index
+ ~~~~~~~~~
    + CategoryInfo          : ObjectNotFound: (E:\web design\learn gi  
   t\HELLO-GIT\index:String) [Get-Content], ItemNotFoundException      
    + FullyQualifiedErrorId : PathNotFound,Microsoft.PowerShell.Comma  
   nds.GetContentCommand

PS E:\web design\learn git\HELLO-GIT> git cat-file -p       
fatal: <object> required with '-p'

usage: git cat-file <type> <object>
   or: git cat-file (-e | -p) <object>
   or: git cat-file (-t | -s) [--allow-unknown-type] <object>
   or: git cat-file (--textconv | --filters)
                    [<rev>:<path|tree-ish> | --path=<path|tree-ish> <rev>]
   or: git cat-file (--batch | --batch-check | --batch-command) [--batch-all-objects]
                    [--buffer] [--follow-symlinks] [--unordered]
                    [--textconv | --filters] [-Z]

Check object existence or emit object contents
    -e                    check if <object> exists
    -p                    pretty-print <object> content

Emit [broken] object attributes
    -t                    show object type (one of 'blob', 'tree', 'commit', 'tag', ...)
    -s                    show object size
    --[no-]allow-unknown-type
                          allow -s and -t to work with broken/corrupt objects
    --[no-]use-mailmap    use mail map file
    --[no-]mailmap ...    alias of --use-mailmap

Batch objects requested on stdin (or --batch-all-objects)
    --batch[=<format>]    show full <object> or <rev> contents
    --batch-check[=<format>]
                          like --batch, but don't emit <contents>      
    -Z                    stdin and stdout is NUL-terminated
    --batch-command[=<format>]
                          read commands from stdin
    --batch-all-objects   with --batch[-check]: ignores stdin, batches all known objects

Change or optimize batch output
    --[no-]buffer         buffer --batch output
    --[no-]follow-symlinks
                          follow in-tree symlinks
    --[no-]unordered      do not order objects before emitting them    

Emit object (blob or tree) with conversion or filter (stand-alone, or with batch)
    --textconv            run textconv on object's content
    --filters             run filters on object's content
    --[no-]path blob|tree use a <path> for (--textconv | --filters); Not with 'batch'

PS E:\web design\learn git\HELLO-GIT> cd de   
cd : Cannot find path 'E:\web design\learn git\HELLO-GIT\de' because 
it does not exist.
At line:1 char:1
+ cd de
+ ~~~~~
    + CategoryInfo          : ObjectNotFound: (E:\web design\learn gi  
   t\HELLO-GIT\de:String) [Set-Location], ItemNotFoundException        
    + FullyQualifiedErrorId : PathNotFound,Microsoft.PowerShell.Comma  
   nds.SetLocationCommand

PS E:\web design\learn git\HELLO-GIT> 
