# easy_test_config

An easy way to handle test settings.

## The config.yaml file,

How this works is any settings in the `test-config.yaml` file will take precedence.  After that, the framework will load additional configs that are specified in the 'EXTRACONFIGS` enviornment variable or `EXTRACONFIGS` property specified on the `test-config.yaml` file.  (environment variable will take precedence if specified)

# How to Use

1. Create any number of *.yaml files with settings you want and put them in the /configs directory.
2. Create a `test-config.yaml` in the base of your test project.
3. In the `test-config.yaml` add a 'EXTRACONFIGS` property, and specify the additional yaml files you wish to load.
4. If you need to override any variables, write them in the `test-config.yaml`


