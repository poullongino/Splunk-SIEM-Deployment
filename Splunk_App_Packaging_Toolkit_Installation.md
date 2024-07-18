Install Python --> Python 3.7.8

py --list

py -3.7 -m pip install virtualenv 

cd C:\Users\raman\Documents

mkdir Splunk_Migration

cd Splunk_Migration

py -3.7 -m virtualenv venv

venv\Scripts\activate

python --version

curl https://download.splunk.com/misc/packaging-toolkit/splunk-packaging-toolkit-1.0.1.tar.gz --output splunk-packaging-toolkit-1.0.1.tar.gz

pip install splunk-packaging-toolkit-1.0.1.tar.gz

pip install semantic_version==2.6.0

slim partition splunk-add-on-for-unix-and-linux_900.tgz
