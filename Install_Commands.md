---------------------------------------------------------------------------------------------------------------
## 01 install DBT core \
python3 -m pip install --upgrade pip \
python3 -m venv myenv_dbtswf \
source myenv_dbtswf/bin/activate \

pip install injecta PyYAML \

pip install dbt-snowflake \
pip install dbt-core \
---------------------------------------------------------------------------------------------------------------
## dbt initialize 
dbt init 

![image](https://github.com/user-attachments/assets/0d5dac14-4867-438d-9bc1-42bd259a5fbd)

![image](https://github.com/user-attachments/assets/a4cbed4f-8998-4dc8-bb44-8a0525231c34)

---------------------------------------------------------------------------------------------------------------
## Configure dbt_project.yml and packages 
