# Windows Commands, Git & GitHub

## **Link:**

- [Udemy.com](https://www.udemy.com/course/git-github-practical-guide/)

- [Git](https://git-scm.com/)

- [GitHub](https://github.com/)

- [Cmder](https://cmder.net/)

# **Windows Commands (CMD)**

**`TAB =Automatické dokončování`**

---

## **Základní pojmy:**

| ENG       | CZE             |
| :-------- | :-------------- |
| File      | Soubor          |
| Folder    | Složka          |
| Create    | Vytvořit        |
| Copy      | Kopírovat       |
| Move      | Přesunout       |
| Delete    | Odstranit       |
| Switch    | Přepnout        |
| Snapshot  | Snímek projektu |
| Merge     | Sloučit/Spojit  |
| Untracked | Nesledováno     |
| Modified  | Změněno         |

---

## **Terminál ve Win 🪟**

[Docs.microsoft.com](https://docs.microsoft.com/en-us/windows-server/administration/windows-commands/windows-commands)

## **Directory (Adresáře)**:

- Home directory
- Users directory
- Root directory

---

## **The Basic:**

- ### **Clean up terminal:**

  ```
  cls
  ```

  ***

- ### **List Item (Seznam souborů a složek v aktuální složce):**

  ```
  ls
  ```

  ***

- ### **Directory (ls + info):**

  ```
  dir
  ```

  ***

- ### **End protocol:**

  ```
  q
  ```

  ***

- ### **Move level up:**

  ```
  cd ..
  ```

  ***

- ### **Root directory:**

  ```
  cd /
  ```

  ***

- ### **Switch hard disk drives:**

  ```
  D:
  ```

---

## **Absolute vs Relative Paths:**

- ### **Absolute paths (Od Root Directory):**

  ```
  CD C:\NameFolder\NameFolder
  ```

  ***

- ### **Realative paths (Od aktuální polohy):**

  ```
  cd "NameFolder"
  ```

  ***

  ```
  cd NameFolder\
  ```

  ***

  ```
  cd NameFolder\NameFolder
  ```

  ***

  ```
  cd ..\NameFolder
  ```

---

## **File & Folder - Creating & Deleting & Copying & Moving & Reading:**

- ### **Create Folder:**

  ```
  mkdir NameFolder
  ```

  ***

- ### **Create File:**

  ```
  echo Text in File > NameFile.typ
  ```

  ***

- ### **Read the file:**

  ```
  type NameFile.typ
  ```

  ***

- ### **Delete File:**

  ```
  del NameFile.typ
  ```

  ***

- ### **Delete Folder:**

  ```
  rmdir NameFolder
  ```

  ***

- ### **Copy File:**

  ```
  copy NameFile.typ NameFolder
  ```

  ***

- ### **Copy All file in Folder**

  ```
  copy NameFolder NameFolder
  ```

  ***

- ### **Move File**

  ```
  move NameFile.typ NameFolder
  ```

  ***

- ### **Move Folder**

  ```
  move NameFolder NameFolder
  ```

---

# **GIT**

## **About Git:**

- Its free.
- Open source.
- Distributed version control system.
- Check and track code changes over time (Kontrola a sledování změn kódu v průběhu času).
- Version Control System.
- Local tool.
- Manage Code History.
- Track Changes (Sledujte změny).

---

## **Instal:**

1. GNU General Public License -> Next.
2. Select Destination Location -> C:\Program Files\Git.
3. Select Compoments -> Null.
4. Select Start Menu Folder -> Git.
5. Choosing the default editor user by Git -> Select other editor as Git's default editor.
6. Adjusting the name of the initial branch in new repositories -> Override the default branch name for new repositories.
7. Adjusting your PATH environmet -> Git from the command line and also from 3rd-party software.
8. Choosing the SSH executable -> Use bundled OpenSSH.
9. Choosing HTTPS transport backend -> Use the OpenSSL library.
10. Configuring the line ending conversions -> Checkout Windows-style, commit Unix-style line endings.
11. Configuring the terminal emulator to use with Git Bash -> Use MinTTY (the default terminal of MSYS2).
12. Choose the default behavior of 'git pull' -> Default (fast-forward or merge).
13. Choose a credential helper -> Git Credential Manager Code.
14. Configuring extra options -> Enable file system caching.
15. INSTAL.

---

## **Git můžeme ovládat pomocí:**

1. Graphical User Interface (GUI).
2. Command Prompt (CMD).

---

# **GIT Terminal**

## Získání nápovědy

**`Budete-li někdy při používání Gitu potřebovat pomoc, existují tři způsoby, jak můžete pro libovolný z příkazů Gitu vyvolat manuálovou stránku s nápovědou:`**

```
git help <příkaz>
```

```
git <příkaz> --help
```

```
man git-<příkaz>
```

🐍 **`Například nápovědu pro příkaz config vyvoláte zadáním:`**

```
git help config
```

**`Tyto příkazy jsou šikovné, neboť je můžete spustit kdykoli, dokonce i offline. Pokud nestačí ani manuálová stránka ani tato kniha a uvítali byste osobní pomoc, můžete zkusit kanál #git nebo #github na IRC serveru Freenode (irc.freenode.net). Na těchto kanálech se většinou pohybují stovky lidí, kteří mají se systémem Git bohaté zkušenosti a často ochotně pomohou.`**

---

## **SETINGS GIT:**

```
git config --global user.name "Starousek"
```

```
git config --global user.email Starousek_Program@outlook.cz
```

---

## **The Basic:**

- ### **GIT Version:**

  ```
  git --version
  ```

  ***

- ### **Config List:**

  ```
  git config --list
  ```

  ***

- ### **Info Working Directory:**

  ```
  git status
  ```

  ***

- ### **Info Working Directory Short:**

  ```
  git status --short
  ```

  ***

- ### **Snapshot:**

  ```
  git log
  ```

  ***

- ### **List File:**

  **`Staging Area (Index File)`**

  ```
  git ls-files
  ```

---

## **\<File\>**

- ### **One File**

  ```
  FileName.typ
  ```

  ***

- ### **All File**

  ```
  .
  ```

  ***

- ### **All File by type**

  ```
  *.typ
  ```

---

## **Stavy:**

1. ### **Working Directory - `Untracked files:` = Soubory které nejsou sledované.**

   **`?? = Untracked files`**

2. ### **.git (Hidden) Repository:**

   - ### **Staging Area (Index File) - `Changes to be committed:`, `Changes not staged for commit:` = Soubory které jsou sledováné**

     **`A = New file`**

     **`M = Modified`**

     **`D = Deleted`**

     **`R = Renamed`**

   ***

   - ### **Commitis (Objects Folder) - Nová verze APP s vlastní ID `ab03ab8c0b76f6ca5e0b6d463251ca745f82c74c` (**Snapshot**).**

---

## **Staging Area (Index File):**

- ## **Initialize:**

  Create: .git (hidden) = Repository.

  ```
  git init
  ```

  ***

- ## **Add:**

  **`Untracked files: -> Changes to be committed:`**

  **`Changes not staged for commit: -> Changes to be committed:`**

  - ### **Add:**

    ```
    git add <File>
    ```

    ***

  - ### **rm**

    **`D = Deleted`**

    ```
    git rm <File>
    ```

  ***

- ## **Revert changes:**

  - ### **`Untracked files:`**

    **`🚨Delete New file`**

    - #### **List New file:**

      ```
      git clean -dn
      ```

      ***

    - #### **Cleam file**

      ```
      git clean -df
      ```

    ***

  - ### **`Changes not staged for commit:`**

    **`D = Deleted`** **`-> Obnoví odstraněné soubor`**

    **`M = Modified`** **`->🚨Odstraní všechny změni v souboru od posledního commitu`**

    ```
    git restore <file>
    ```

    ```
    git checkout <file>
    ```

    ***

  - ### **`Changes to be committed: -> Changes not staged for commit:`**

    ```
    git restore --staged <file>
    ```

    ```
    git reset
    ```

    ***

  - ### **`Changes to be committed: -> Untracked files:`**

    ```
    git rm --cached <file>
    ```

    ***

  - ### **`Snapshot -> Changes to be committed:`**

    **`Delete last commit`**

    **`~X`** **`X=Počet komitů`**

    ```
    git reset --soft HEAD~1
    ```

    ***

  - ### **`Snapshot -> Untracked files:`**

    **`Delete last commit`**

    **`~X`** **`X=Počet komitů`**

    ```
    git reset HEAD~1
    ```

    ***

  - ### **`Snapshot`**

    **`🚨Delete Commit + všechny změny v něm`**

    **`~X`** **`X=Počet komitů`**

    ```
    git reset --hard HEAD~1
    ```

  ***

- ## **`Changes to be committed: -> Snapshot`**

  ```
  git commit -m "NameSnapshot"
  ```

---

## **Commitis (Objects Folder):**

- ## **Switch Commit:**

  - ### **Checkout**

    **`Switch Commint`**

    ```
    git checkout <ID>
    ```

    ***

  - ### **Switch**

    **`Last Commint`**

    ```
    git switch -
    ```

  ***

- ## **Branches:**

  **`Hlavní branch je`** **`(MAIN)`**

  **`HEAD`** **`-> Odkazuje na poslední Commit v branch.`**

  **`HEAD detached`** **`-> Jsme mimo branch.`**

  **`<NameBranches>`** **`Nesmí obsahovat mezery.`**

  ***

  - ### **List Branches in Repository:**

    ```
    git branch
    ```

    ***

  - ### **ADD NEW Branch:**

    **`Copy MAIN Branch`**

    ```
    git branch <NameBranches>
    ```

    ***

  - ### **Switch Branch:**

    ```
    git checkout <NameBranch>
    ```

    ```
    git switch <NameBranch>
    ```

    ***

  - ### **ADD NEW + Switch Branch:**

    ```
    git checkout -b <NameBranch>
    ```

    ```
    git switch -c <NameBranch>
    ```

    ***

  - ### **Merge Branch:**

    - #### **Fast-Forward_Merge**

      **`Musíme být v branch, kam chceme sloučit jinačí branch.`**

      ```
      git merge <NameBranch>
      ```

      ***

      **`Sloučení bez commitů`**

      **`Branch commit -> Changes to be committed:`**

      **`Je potřeba vytvořit nový Commit.`**

      ```
      git merge --squash <NameBranch>
      ```

    ***

    - #### **Non-Fast-Forward**

      **`Automaticky vytvoříme nový commit:`**

      **`Merge branch '<NameBranch>'`**

      ```
      git merge --no-ff <NameBranch>
      ```

      **`Pokud máme v branch do které chceme sloučit novější commit`**

      ```
      git merge <NameBranch>
      ```

    - #### **Rebase**

      **`Přepíše ID commit`**

      ```
      git rebase
      ```

    ***

  - ### **Delete Branch:**

    - #### **Delete pokud byly sloučené:**

      ```
      git branch -d <NameBranch>
      ```

    - #### **🚨Delete pokud nebyly sloučené:**

      ```
      git branch -D <NameBranch>
      ```

---

## **Git Stash**

**`Changes not staged for commit:`**

- ### **Save**

  ```
  git stash
  ```

  ```
  git stash push -m "NameStash"
  ```

  ***

- ### **List**

  **`stash@{i}:`** **`i=Nuber`**

  ```
  git stash list
  ```

  ***

- ### **Load:**

  - #### **Last One**

    ```
    git stash apply
    ```

    ***

  - #### **Index {i}**

    ```
    git stash apply i
    ```

  ***

- ### **Load + Delete**

  ```
  git stash pop i
  ```

  ***

- ### **Delete:**

  - #### **Last One**

    ```
    git stash drop
    ```

    ***

  - #### **Index {i}**

    ```
    git stash drop i
    ```

    ***

  - #### **ALL**

    ```
    git stash clear
    ```

---

## **GIT-REFLOG**

- ### **List**

  **`30 dení historie`**

  **`a04f988 = ID`**

  ```
  git reflog
  ```

  ***

- ### **Load**

  ```
  git reset --hard ID
  ```

  ***

  ```
   git checkout ID
  ```

---

## **.gitIgnore**

- ### **One File**

  ```
  NameFile.typ
  ```

  ***

- ### **All File type:**

  ```
  *.typ
  ```

  ***

- ### **Neměl by být ignorován:**

  ```
  !NameFile.typ
  ```

  ***

- ### **Folder**

  ```
  NameFolder
  ```

  ```
  NameFolder/*
  ```

---

# GitHub

## About GitHub:

- Je zadarmo.
- Largest Development Platform (Největší vývojová platforma.).
- Cloud Hosting & Collaboration Provider (Poskytovatel cloudového hostingu a spolupráce).
- Git Repository Hosting.

---

- ### **Create a new repository on the command line:**

  ```
  echo "# WIKI-PikaHeim" >> README.md
  git init
  git add README.md
  git commit -m "first commit"
  git branch -M main
  git remote add origin https://github.com/Starousek/WIKI-PikaHeim.git
  git push -u origin main
  ```

- ### **Push an existing repository from the command line:**

  ```
  git remote add origin https://github.com/Starousek/WIKI-PikaHeim.git
  git branch -M main
  git push -u origin main
  ```
