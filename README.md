# jadm333.github.io
Personal webpage

Deploy steps

```bash
# Generate page
pelican content -o output -s pelicanconf.py
# Copy output folder to gh-pages branch
ghp-import output -b gh-pages
# Change brancj
git checkout gh-pages
git add .
git commit -m "Sync page"
git push
```