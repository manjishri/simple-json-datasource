# 🤝 Collaboration Guide for Simple JSON Datasource

## Quick Start for Your Friend

### Step 1: Clone the Repository
```bash
git clone https://github.com/manjishri/simple-json-datasource.git
cd simple-json-datasource
```

### Step 2: Switch to Collaboration Branch
```bash
git checkout genspark_ai_developer
```

### Step 3: Install Dependencies
```bash
npm install -g yarn
yarn install
```

### Step 4: Start Coding!
You're ready to collaborate! 🚀

---

## 📋 Daily Workflow

### Before You Start Working

1. **Pull the latest changes:**
   ```bash
   git checkout genspark_ai_developer
   git pull origin genspark_ai_developer
   ```

2. **Check what branch you're on:**
   ```bash
   git branch
   ```
   (You should see `* genspark_ai_developer`)

### While Working

1. **Check status frequently:**
   ```bash
   git status
   ```

2. **Test your changes:**
   ```bash
   npm run build
   ```

### After Making Changes

1. **Stage your changes:**
   ```bash
   git add .
   # Or stage specific files:
   git add src/file1.js src/file2.js
   ```

2. **Commit with a clear message:**
   ```bash
   git commit -m "feat: add new feature description"
   # Or
   git commit -m "fix: resolve bug in query endpoint"
   ```

3. **Pull latest changes (in case your friend pushed):**
   ```bash
   git pull origin genspark_ai_developer
   ```

4. **Push your changes:**
   ```bash
   git push origin genspark_ai_developer
   ```

---

## 🔄 Handling Conflicts

If you and your friend edit the same file, you might get a merge conflict:

### When Pull Shows Conflicts:

```bash
# Git will tell you which files have conflicts
git status

# Open the conflicted files in your editor
# Look for markers like:
# <<<<<<< HEAD
# Your changes
# =======
# Friend's changes
# >>>>>>> branch-name

# Edit the file to keep the correct code
# Remove the conflict markers

# After resolving:
git add <resolved-file>
git commit -m "resolve: merge conflict in <file>"
git push origin genspark_ai_developer
```

---

## 💡 Best Practices

### Communication

- **Coordinate tasks:** Discuss who works on what to avoid conflicts
- **Use descriptive commit messages:**
  - ✅ Good: `"feat: add support for tag-values API endpoint"`
  - ❌ Bad: `"fixed stuff"`

### Commit Message Format

Use conventional commits:
- `feat:` - New feature
- `fix:` - Bug fix
- `docs:` - Documentation changes
- `style:` - Code style changes (formatting)
- `refactor:` - Code refactoring
- `test:` - Adding tests
- `chore:` - Maintenance tasks

### Work Patterns

1. **Pull before starting work** - Always get the latest code
2. **Commit frequently** - Small, focused commits are better
3. **Push regularly** - Share your progress daily
4. **Test before pushing** - Make sure your code builds
5. **Review each other's code** - Learn and improve together

---

## 🎯 Common Commands Reference

### Check Status
```bash
git status                    # See what files changed
git log --oneline            # See recent commits
git branch -a                # See all branches
```

### Undo Changes
```bash
git checkout -- <file>       # Discard changes in a file
git reset HEAD <file>        # Unstage a file
git reset --soft HEAD~1      # Undo last commit (keep changes)
```

### See Differences
```bash
git diff                     # See unstaged changes
git diff --staged            # See staged changes
git diff origin/genspark_ai_developer  # Compare with remote
```

### Working with Your Friend's Changes
```bash
git fetch origin             # Download latest info
git pull origin genspark_ai_developer  # Get and merge changes
git log origin/genspark_ai_developer   # See friend's commits
```

---

## 🚀 Creating a Pull Request

When your feature is ready to merge into `master`:

1. **Make sure everything is committed and pushed:**
   ```bash
   git status
   git push origin genspark_ai_developer
   ```

2. **Go to GitHub:**
   - Visit: https://github.com/manjishri/simple-json-datasource
   - Click "Pull requests" tab
   - Click "New pull request"
   - Select: `base: master` ← `compare: genspark_ai_developer`
   - Add title and description
   - Click "Create pull request"

3. **Ask your friend to review** before merging

---

## 📞 Communication Tips

### Use Git for Asynchronous Communication

**Leave notes in commits:**
```bash
git commit -m "fix: update query API - @friend please test this"
```

**Use GitHub issues:**
- Create issues for bugs or features
- Assign to each other
- Comment and discuss

**Use Pull Request reviews:**
- Comment on specific lines of code
- Request changes
- Approve changes

---

## 🆘 Troubleshooting

### "Your branch is behind"
```bash
git pull origin genspark_ai_developer
```

### "Your branch has diverged"
```bash
git pull --rebase origin genspark_ai_developer
# Or
git pull origin genspark_ai_developer  # then resolve conflicts
```

### "Permission denied"
- Make sure your friend has access to the repository
- Check GitHub settings → Collaborators
- Add your friend's GitHub username

### "Merge conflict"
- Don't panic! This is normal
- Follow the "Handling Conflicts" section above
- When in doubt, communicate with your friend

---

## 📚 Project-Specific Info

### Build the Project
```bash
npm run build
```

### Project Structure
```
simple-json-datasource/
├── src/            # Source code
├── dist/           # Built files
├── spec/           # Tests
├── Gruntfile.js    # Build configuration
└── package.json    # Dependencies
```

### Key Files to Know
- `src/datasource.js` - Main datasource logic
- `src/query_ctrl.js` - Query editor
- `package.json` - Project dependencies

---

## 🎓 Learning Resources

- **Git Basics:** https://git-scm.com/book/en/v2/Getting-Started-About-Version-Control
- **GitHub Flow:** https://guides.github.com/introduction/flow/
- **Resolving Conflicts:** https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/addressing-merge-conflicts

---

## ✅ Collaboration Checklist

Daily routine:
- [ ] Pull latest changes
- [ ] Make your changes
- [ ] Test your changes
- [ ] Commit with clear message
- [ ] Pull again (in case of new changes)
- [ ] Push your changes
- [ ] Communicate with your friend

---

**Happy Coding! 🎉**

Questions? Issues? Talk to your collaborator or create a GitHub issue!
