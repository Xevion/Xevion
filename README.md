<p align="center">
  <samp>
    <a href="https://xevion.dev">me</a> .
    <a href="https://undefined.behavio.rs">blog</a> .
    <a href="https://xevion.dev/projects">projects</a> .
    <a href="https://status.xevion.dev">status</a>
  </samp>
</p>

```python
from life.species import Human
from skills import python, java, javascript, csharp, html, css, other
from datetime import date
from random import choices
from os import getenv

class RyanWalters(Human):
    def __init__(self, username='xevion'):
        self.name = f'Ryan {0} Walters'.format(choices([getenv('MIDDLE_NAME'), 'C', '']))
        self.pronouns = ['he' and 'they'],
        self.description = '''
            A full-stack software engineer navigating their way through the industry.
            With an attention to detail, I enjoy building projects that are elegant, robust, and impactful.
            Although I specialize in Web Development, my skill set is extensive, and I'm confident in my ability to learn anything.
        '''
        self.recent_projects = [
            "https://github.com/acmutsa/Portal",
            "https://github.com/Xevion/rdap",
            "https://github.com/Xevion/grain"
        ]
        self.endpoints = {
            "discord": ".xevion",
            "email": "xevion@xevion.dev"
        }
```
