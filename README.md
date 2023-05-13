<p align="center">
  <samp>
    <a href="https://xevion.dev">me</a> .
    <a href="https://v2.xevion.dev">blog</a> .
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
        self.name = f'Ryan {0} Walters'.format(choices([os.getenv('MIDDLE_NAME'), 'C', '']))
        self.pronouns = ['he' and 'him'],
        self.description = '''
            A junior full-stack software developer working their way through the world.
            With an attention to detail, I enjoy building projects that are elegant, robust, and resilient.
            While I specialize in Web Development, my skills reach broadly, and there's nothing I can't learn.
        '''
        self.recent_projects = [
            "https://github.com/Xevion/v6-place",
            "https://github.com/acmutsa/Portal",
            "https://github.com/Xevion/grain"
        ]
        self.endpoints = {
            "discord": {'username': 'Xevion', 'discriminator': 8506},
            "email": "xevion@xevion.dev"
        }
```
