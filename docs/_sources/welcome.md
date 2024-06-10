# Sumerian Networks JupyterBook

The goal of the Sumerian Network project has been to build reproducible socio-economic networks from the [Ur III](https://en.wikipedia.org/wiki/Third_Dynasty_of_Ur) archives, and to further refine these models to more accurately reflect the actors and entities active in these unprovenanced archives over the ca. 80 year period in the 21st century BCE. Beginning with ca. 15,000 transliterated texts from the site of Drehem (known in antiquity as [Puzriš-Dagān](https://en.wikipedia.org/wiki/Puzrish-Dagan)), this JupyterBook has a linear progression which applies various tools and methods in [NLP](https://en.wikipedia.org/wiki/Natural_language_processing) and Open Science. In order to make our study reproducible, we used [Jupyter Notebooks](https://en.wikipedia.org/wiki/Project_Jupyter ) (hosted in a [GitHub repository]()) to describe the tools and methods we use in connection with the code and dataset, which result in a series of empirical network models. 

## This book describes a series of steps for building a network from a collection of Sumerian Ur III administrative texts, curated digitally in the following databases:

*   [CDLI](https://cdli.ucla.edu/)
*   [ORACC](http://oracc.museum.upenn.edu/)
*   [BDTNS](http://bdtns.filol.csic.es/)

### The book is intended to help you learn how such a network can be built, and does so using `Python` Jupyter Notebooks. These notebooks can be mounted to your GoogleDrive and run in the Google Colaboratory by running the following cell.

## Related UC Berkeley DH Projects
* [Cuneiform Name Authority](https://digitalhumanities.berkeley.edu/projects/cuneiform-name-authority-ur-iii-period)
* [Sumerian Networks](https://digitalhumanities.berkeley.edu/sumerian-networks-reconstructing-ur-iii)

## Authors & Developers:
[Niek Veldhuis](https://github.com/niekveldhuis), PI (2017-2021)
[Adam Anderson](https://github.com/admndrsn) (2017-2021), [Yashila Bordag](https://github.com/ybordag) (2020-2021), [Colman Bouton]( https://github.com/lorentzfactor) (2021), [Jenny Chen](https://github.com/jchen437) (2018), [Tiffany Chien](https://github.com/tiffchien) (2017-2020), [Lucie Choi](https://github.com/dkqntiqn) (2018), [Dalton Do]( https://github.com/daltondo) (2017-2018), [Zekai Fan](https://github.com/babybear68) (2018-2020), [Kimberly Kao](https://github.com/kimkao) (2018), [Jason Kha]() (2017), [Anya Kulikov](https://github.com/akulikov97) (2018-2021), [Dominic Liu](https://github.com/Dominicliu129) (2020-2021), [Harini Rajan](https://github.com/HariniRajan) (2017-2019), [Max Sullivan](https://github.com/maxsully7) (2020), [Aleksi Sahala]( https://github.com/asahala) (2019), [Anjali Unnithan](https://github.com/anjaliu14) (2018-2021).

```python
!pip install -U -q PyDrive
from pydrive.auth import GoogleAuth
from pydrive.drive import GoogleDrive
from google.colab import auth
from oauth2client.client import GoogleCredentials
# Authenticate and create the PyDrive client.
#auth.authenticate_user()
#gauth = GoogleAuth()
#gauth.credentials = GoogleCredentials.get_application_default()
#drive = GoogleDrive(gauth)

#create necessary directories
import os
os.makedirs('jsonzip', exist_ok=True)
os.makedirs('output', exist_ok=True)
```
