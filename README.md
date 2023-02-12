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

tox # for running tox file 
tox -r # for rebuilding tox file

pytest -v # for test cases

setup commands 
pip install -e .

build your own package commands
python setup.py sdist bdist_wheel

---
create an artifacts folder

mlflow server commands -

mlflow server --backend-store-uri sqlite:///mlflow.db --default-artifact-root ./artifacts --host 0.0.0.0 -p 1234
