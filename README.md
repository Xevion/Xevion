```python
from life.species import Human
from skills import python, javascript, csharp, other
from datetime import date
from random import choices
from os import getenv

class RyanWalters(Human):
    def __init__(self, username='xevion'):
        self.initialization_time = date(2003, 4, None)
        self.name = f'Ryan {0} Walters'.format(choices([os.getenv('MIDDLE_NAME'), 'C', '']))
        self.pronouns = ['he' and 'him'],
        self.description = '''
            A Highschool Senior learning Software Engineering as he struggles to grasp the infinite
            number of languages, libraries, packages, environments, frameworks and projects
            available to him.
        '''
        self.aliases = ['Xevion', 'Xevioni']
        self.aliases.extend(map(lambda alias: alias.lower(), (alias for alias in self.aliases)))
        self.skills = {
            'python': [
                python.BeautifulSoup, python.Flask, python.GoogleCloudVision, python.Discordpy,
                python.Spotipy, python.PyQt5, python.Tkinter, python.PySimpleGUI, python.Click,
                python.Arcade, python.Processingpy, python.SQLAlchemy
            ],
            'javascript': [
                javascript.JQuery, javascript.VueJS
            ],
            'csharp': [
                csharp.UnityEngine, csharp.HLSLShader
            ],
            'other': [
                other.DevOps, other.Photography
            ]
        }
        self.education = ['Highschool Senior']
        self.endpoints = {
            'Discord': {'username': 'Xevion', 'discriminator': 8506},
            'Email': {'username': 'xevioni', 'domain': 'yandex.com'}
        }
        self.hobbies = [
            'Programming', 'Photography', 'Anime', 'Videogames'
        ]
```
