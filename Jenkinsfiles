stages:
  - style
  - test
  - deploy

# This job is for style test, running by using python 2.7

pep8:
  stage: style
  script:
    - pip install tox
    - tox -e pep8
  tags:
    - python-2.7

#This job is for unit test for 2.7 and 3.4

unittest-py27:
  stage: test
  script:
    - pip install tox
    - tox -e py27
  tags:
    - python-2.7

unittest-py34:
  stage: test
  script:
    - pip install tox
    - tox -e py34
  tags:
    - python-3.4
