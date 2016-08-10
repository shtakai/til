# Using dotenv in Flask

1. pip install dotenv

2. create .env file

```
SECRET_KEY="SECRET_SOMETHING"
```

3. import and load

```
from os.path import join, dirname
from dotenv import load_dotenv
import os


dotenv_path = join(dirname(__file__), '.env')
load_dotenv(dotenv_path)
```

4. read env

```
SECRET = os.environ['SECRET_KEY']
```
