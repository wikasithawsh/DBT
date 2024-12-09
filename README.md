# This is the DBT Snowflake project 

--------------------------------------------------------------------------------------------------------------
python3 -m pip install --upgrade pip
python3 -m venv myenv_dbtswf 
source myenv_dbtswf/bin/activate

pip install injecta PyYAML

pip install dbt-snowflake
pip install dbt-core
----------------------------------------------------------------------------------------------------------------
## dbt project configs in vscode 
>> dbt -vscode > 
models:
  dbt_sw_project:
    # Config indicated by + and applies to all files under models/example/
    #example:
      #+materialized: view
    staging:
      +materialized: view
      snowflake_warehouse: dbt_wh
    marts: 
      +materialized: table
      snowflake_warehouse: dbt_wh
    
>>>
left side > added new folders under models 
staging 
marts 

![image](https://github.com/user-attachments/assets/1365dce3-f8b3-4bdf-b8d1-2d44506bb729)

-------------------------------------------------------------------------------------------------------------------
dbt-labs/dbt-utils
/home/wiks/Documents/2024_learn/2024_DEC
source myenv_dbtswf/bin/activate

## created packaged.yml file & added below there 
packages:
  - package: dbt-labs/dbt_utils
    version: 1.1.1

install db packages using below command

dbt deps

![image](https://github.com/user-attachments/assets/c43d6baa-e9ad-4acc-a3fc-6cb82baf9e0d)

--------------------------------------------------------------------------------------------------------------------
## Step 03 : Create Source & Staging Tables 
