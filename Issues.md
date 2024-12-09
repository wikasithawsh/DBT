--------------------------------
01: Install DBT CORE
Command = pip install dbt-snowflake
## ERROR 1.0 : Cannot uninstall 'PyYAML'. It is a distutils installed project and thus we cannot accurately determine which files belong to it which would lead to only a partial uninstall.

![image](https://github.com/user-attachments/assets/db599aac-e9ae-4783-a4cf-ca0fbc4bfe7c)

## Solution > 
python3 -m pip install --upgrade pip
### Use a Virtual Environment
python3 -m venv myenv_dbtswf
source myenv_dbtswf/bin/activate
## Then install required packages 
pip install injecta PyYAML

## Error 1.2 : 
![image](https://github.com/user-attachments/assets/ebeec96c-5156-4b84-9d0c-b31d640f910a)

##Downgrade PyYAML to a Compatible Version
pip install "PyYAML<6.0"
 ![image](https://github.com/user-attachments/assets/07037167-4154-44e2-a216-3701c47f10f7)

![image](https://github.com/user-attachments/assets/52f2da6e-dc34-46f2-bc08-3e1d7488b179)



