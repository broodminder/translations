# translations
This is the public repo for translations. 
Three platforms are considered
- Mybroodminder.com
- The Bees App
- Beecounted.org

Any contributor can update existing translations or create translations to a new language. Simply follow the Pull request workflow to submit your translations.

You can also send us an email to [support&broodminder.com](mailto:support&broodminder.com)


Somme considerations to get you started :

- The master files are the english ones.

- The translation files are XML or json format. The translation only targets the `<value>` fields.

- You can use Visual Studio Code to manage your translations having side by side the English master and your translation. Simply follow this video [Compare files in VSC](https://youtu.be/50f5FBw9BSI)

- ChatGPT can be of great help translating large parts of that file. Simply copy paste (200 lines at once)

![comparing files](./assets/translating_to_german.png)

# How to translate json file

## Initialization

Requirements :
- python 3.11.x
- pyenv

### 1 - Create environnement
```
pyenv virtualenv 3.11.2 translations
cp .env.example .env
```

Fill the *.env* file with the configuration you want.

### 2 - Activate environnement
```
pyenv activate translations
```

### 3 - Export python libraries
```
pip install -r requirements.txt
```

## How to use it ?
```
python translateFiles.py
```

You should have all translated files then you can make a verification and commit.