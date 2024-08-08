# Odoo_Problem
In this repo, you will find the bug, the issue, and my solution.

# 1. Problem #1 if you want to write the testcase in odoo follow the some steps:
 -->first Understand the file structure where we will write the testcase in odoo module
  #-->your_module_name
      --contoller
      --module
      ---Tests
         --test_case01.py
         --test_case02.py
      --__init__.py
      --manifest.py
 # enable the testcasefile and run its commands are:
   /home/codetrade/Workspace/odoo/odoo-bin -c /home/codetrade/docker_projects/odoo17/custom_addons/broad-captial/broadcapital_base -u broadcapital_base --test-enable --stop-after-init

# if you want to create the coverage-file in odoo then:
  coverage run --source=odoo.addons.broadcapital_base --omit='/tests/' /home/codetrade/Workspace/odoo/odoo/odoo-bin --addons-path=/home/codetrade/Workspace/odoo/odoo/addons/,/home/codetrade/Workspace/odoo/odoo/odoo/addons/,/home/codetrade/docker_projects/odoo17/custom_addons/broad-captial -d testdb19  -u broadcapital_base --test-enable --stop-after-init --xmlrpc-port=7020

# after that you run the succesful the testcase file 
# you need to run the command to create the coverage_html file
  --coverage html -d broadcapital_base

# then you find the coverage report check its   
  Thanks to Read....
