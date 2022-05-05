# MUIA_DCCVE_AttitudeDetermination
### This repository is intented to be used in the UPM VDI Ubuntu desktop. It constains the required files to do the attitude determination practical lessons.
### To install the required files do:

cd /opt/42
git clone https://github.com/KOlfe/MUIA_DCCVE_AttitudeDetermination.git
cp /opt/42/MUIA_DCCVE_AttitudeDetermination/42.json /opt/42/Database/42.json
cp /opt/42/MUIA_DCCVE_AttitudeDetermination/AC.json /opt/42/Database/AC.json
python /opt/42/Database/JsonToIPC.py
#cd /opt/42

make clean
make

cp /opt/42/MUIA_DCCVE_AttitudeDetermination/desktop/42Simulator.desktop /home/upm/Escritorio/
chmod u=rwx,g=rwx,o=rwx /opt/42/MUIA_DCCVE_AttitudeDetermination/desktop/simular.sh 
chmod u=rwx,g=rwx,o=rwx /home/upm/Escritorio/42Simulator.desktop

cp /opt/42/MUIA_DCCVE_AttitudeDetermination/desktop/TRIAD_function.m /home/upm
cp /opt/42/MUIA_DCCVE_AttitudeDetermination/desktop/triad.desktop /home/upm/Escritorio/
chmod u=rwx,g=rwx,o=rwx /opt/42/MUIA_DCCVE_AttitudeDetermination/desktop/startTRIAD.sh 
chmod u=rwx,g=rwx,o=rwx /home/upm/Escritorio/triad.desktop

cp /opt/42/MUIA_DCCVE_AttitudeDetermination/desktop/Q_function.m /home/upm
cp /opt/42/MUIA_DCCVE_AttitudeDetermination/desktop/q.desktop /home/upm/Escritorio/
chmod u=rwx,g=rwx,o=rwx /opt/42/MUIA_DCCVE_AttitudeDetermination/desktop/startQ.sh 
chmod u=rwx,g=rwx,o=rwx /home/upm/Escritorio/q.desktop
