# mystor

echo "# mystor" >> README.md
git init
git add README.md
git commit -m "first commit"
git remote add origin git@github.com:kofik/mystor.git
git push -u origin master

git add .
git commit -am "small changes"
git remote add origin git@github.com:kofik/mystor.git
git push -u origin master
