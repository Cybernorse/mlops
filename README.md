<!-- usable starting commands -->

git init 
dvc init
dvc add data_given/winequality.csv
git add .
git commit -m "first commiting wine"
git remote add origin https://github.com/Cybernorse/mlops.git
git branch -M main
git push -u origin main


dvc repro  # to log data and pipelines to dvc