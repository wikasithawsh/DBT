## 01 install DBT core 
python3 -m pip install --upgrade pip
python3 -m venv myenv_dbtswf 
source myenv_dbtswf/bin/activate

pip install injecta PyYAML

pip install dbt-snowflake
pip install dbt-core
