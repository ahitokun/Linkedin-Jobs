# Linkedin EasyApply Bot -UPDATED 2021
Automate the application process on LinkedIn(Easy Apply)

Video: 
## Setup 

The run the bot install requirements
```bash
pip install -r requirements.txt
```

Enter your username, password, and search settings into the `config.yaml` file

```yaml
username: # Insert your username here
password: # Insert your password here

positions:
- # positions you want to search for
- # Another position you want to search for
- # A third position you want to search for

locations:
- # Location you want to search for
- # A second location you want to search in 

uploads:
 Resume: # PATH TO Resume 
 Cover Letter: # PATH TO cover letter
 Photo: # PATH TO photo
# Note file_key:file_paths contained inside the uploads section should be writted without a dash ('-') 

output_filename:
- # PATH TO OUTPUT FILE (default output.csv)

33blacklist:
- # Company names you want to ignore
```

__NOTE: AFTER EDITING SAVE FILE, DO NOT COMMIT FILE__

### Uploads

There is no limit to the number of files you can list in the uploads section. 
The program takes the titles from the input boxes and tries to match them with 
list in the config file.

## Execute

You can execute by running the ipynb file in the Jupyter ntoebook
You can also execute the bot by running the following in your terminal

## Notes

The bot will run by default for 10 hours and will sleep to make sure everything loads, have also  added random to make us look human.

```
## Notes
python3 easyapplybot.py
```

