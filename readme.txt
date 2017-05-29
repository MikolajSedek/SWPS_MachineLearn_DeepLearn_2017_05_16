
Jeśli chcesz:
1) Tylko obejrzeć statyczną prezentację - otwórz pliki html z prezentacjami :)
2) Uruchomić Jupiter Notebook z kodem w Py:

Polecam skorzystać z maszyny wirtualnej na Linuxie lub Dockera (np. Kitematic + obraz: https://hub.docker.com/r/cannin/jupyter-keras-tensorflow-tools/).

Próba uruchomienia tych notebooków pod Windowsem / MacOS prawdopodobnie się nie uda, albo będzie wymagać daleko idących zmian.


Warto do obrazu Dockera domontować dyski - inaczej nie zapamięta zmian.

Trzeba doinstalować brakujące biblioteki (wystarczy dokleić i wywołać w pierwszym okienku notebooka lub z linii poleceń - wtedy bez "!"):

!pip install -U gensim
!pip install glove_python
!apt-get install graphviz -y 
!pip install pydot-ng 
!pip install --upgrade xgboost keras tensorflow seaborn imblearn 
!apt-get install python-tk -y

Jeśli chcesz uruchomić Deep Learning na GPU to tylko na Linuxie zainstalowanym jako system operacyjny (nie ma mowy o maszynie wirtualnej na innym systemie), poradnik tutaj:
http://ksopyla.com/machine-learning/instalacja-tensorflow-0-9-cuda-7-5-na-ubuntu-16-04/ 