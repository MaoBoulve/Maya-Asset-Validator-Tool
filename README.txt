# Copy and paste this whole text into Maya's python script editor

# Place Maya-Game-Asset-Validator-Tool folders into C:\Users\[user]\Documents\maya\scripts\
# Edit filepaths then copy the following code into a Maya Python script and run.

# To add the code as a shelf button:
# Select all script text, then Middle-click drag the code up to shelf

import sys

# rename [User directory name] to user account Maya files is installed under
sys.path.append('/Users/[User directory name]/Documents/maya/scripts/Maya-Game-Asset-Validator-Tool/Metadata')
sys.path.append('/Users/[User directory name]/Documents/maya/scripts/Maya-Game-Asset-Validator-Tool/QtInterface')
sys.path.append('/Users/[User directory name]/Documents/maya/scripts/Maya-Game-Asset-Validator-Tool/Validator')

import validator_commands

# Change 'run()' to 'validate()' to run validation without changing settings
# Change to 'assets()' to open the asset window
# Change to 'validate_json()' to run validation using settings from json file
validator_commands.run()
