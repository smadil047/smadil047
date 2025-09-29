# set correct identity (important)
git config --global user.name "Syed Adil"
git config --global user.email "your-email@example.com"   # use the email linked to your GitHub account

# create local folder and README
mkdir smadil047
cd smadil047
cat > README.md <<'EOF'
# Hi — I'm Syed Adil

I’m Syed Adil, early project contributor & blockchain enthusiast.

- 🔭 I work on early testnets, node-run testnets, and DePIN projects.
- 🛠️ I publish guides, scripts, and testnet notes here.
- 📫 Reach me via GitHub issues or ping me on Discord.

Pinned repos:
- `alpha-prowlers-docs` — docs & testnet notes
- `crypto-scripts` — small scripts for validators/testnets

EOF

git init
git add README.md
git commit -m "Add profile README"
# create remote repo on GitHub (use gh or create the repo on the website then push)
# Example using gh:
gh auth login
gh repo create smadil047 --public --source=. --remote=origin --push
