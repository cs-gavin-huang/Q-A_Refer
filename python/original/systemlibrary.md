# Python-SystemLibrary

* [What is sys._MEIPASS in Python - Stack Overflow](https://stackoverflow.com/questions/22472124/what-is-sys-meipass-in-python)

  > Q: What is sys._MEIPASS. What is the value of this variable and it's use ? I was a looking one python script but when I ran it on eclipse(pydev). It showing error.
  >
  > 
  >
  > A: sys._MEIPASS is a temporary folder for PyInstaller. See [this question](https://stackoverflow.com/questions/7674790/bundling-data-files-with-pyinstaller-onefile) for more information.

  ```python
  # kivy - Open source Python library for rapid development of applications
  root = os.path.join(sys._MEIPASS, 'kivy_install')
  
  os.environ['KIVY_DATA_DIR'] = os.path.join(root, 'data')
  os.environ['GST_PLUGIN_PATH'] = '{};{}'.format(
      sys._MEIPASS, os.path.join(sys._MEIPASS, 'gst-plugins'))
  
  # ====
  
  
  ```

  