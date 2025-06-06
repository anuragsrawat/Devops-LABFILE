# DevOps Lab 3

## Name: Anurag Singh Rawat
**SAP ID:** 500109945

**Roll Number:** R2142221322

**Batch:** Full Stack AI B3

## GIT BASICS

#### Using SSH and HTTP for Git

##### SSH Key Setup

Using SSH, we need both public and private keys to clone repositories securely.

#### 1. Generating SSH Key
Run the following command to generate an SSH key:
```sh
ssh-keygen -t ed25519 -C "Anurag2004rawat@gmail.com"
```

Verify if the key is generated at the default location:
```sh
ls ~/.ssh
```

#### 2. Reading the SSH Key
To read the key, use:
```sh
cat ~/.ssh/id_ed25519.pub
```

#### 3. Adding SSH Key to SSH-Agent
```sh
ssh-add ~/.ssh/id_ed25519
```

#### 4. Adding the Key to GitHub
- Go to GitHub Settings → SSH and GPG keys → Add a new key
- Copy the contents of `id_ed25519.pub` and paste it

### Cloning Repository Using SSH
```sh
git clone git@github.com:anurag0808/Devopslabb1-h.git
```

---

### Cloning Repository Using HTTP
```sh
git clone https://github.com/anurag0808/Devopslabb1-h.git
```

If authentication is required, Git will prompt for your credentials.

---

## Git Workflow

### 1. Initialize and Clone Repository
```sh
git init
git clone <repository-url>
```

### 2. Working on a Repository
1. Navigate to the repository.
2. Make desired changes.
3. Add changes to the staging area:
   ```sh
   git add .
   ```
4. Commit changes with a message:
   ```sh
   git commit -m "Your commit message"
   ```

### 3. Resolving Merge Conflicts
If multiple changes are made from different locations, always pull before pushing:
```sh
git pull origin main
git merge
```
Then push the changes:
```sh
git push origin main
```

---

## VIM Commands (for Git commit messages)
```bash
1. i → Insert mode
2. q → Quit
3. esc → Changing modes
4. shift + v → Visual mode
   - y → Copy / shift + insert
   - p → Paste
5. ‘H’ , ‘J’, ‘K’, ‘L’ → Move left, up, down, right
6. dd → Delete the line
7. u → Undo
8. /something → Search something
9. esc+ :wq → Save and quit
```
