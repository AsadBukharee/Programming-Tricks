# Programming-Tricks
Here are the solutions of problems I faced During development
===================================================================
Progress Bar in python
===================================================================
import click
import time

for filename in range(3):
    with click.progressbar(range(100), fill_char='=', empty_char=' ') as bar:
        for user in bar:
            time.sleep(0.01)
Here the output you get:

$ python test.py
  [====================================]  100%
  [====================================]  100%
  [=========                           ]   27%
  
  ===================================================================
  Other Example at : http://qpleple.com/add-progress-bars-to-your-python-loops/
  ===================================================================
