"""
Place Metadata, QInterface, and Validator folders into .../Documents/maya/scripts/ folder

Edit filepaths then copy the following code into a Maya Python script and run.

To add the code as a shelf button: Hit Ctrl + A, then Middle Click-dragging the code up to shelf
"""

import sys


# rename [User directory name] to user account Maya files is installed under
sys.path.append('/Users/[User directory name]/Documents/maya/scripts/Metadata')
sys.path.append('/Users/[User directory name]/Documents/maya/scripts/QtInterface')
sys.path.append('/Users/[User directory name]/Documents/maya/scripts/Validator')

import validator_commands

# Change 'run()' to 'validate()' to run validation without changing settings
# Change to 'assets()' to open the asset window
# Change to 'validate_json()' to run validation using settings from json file
validator_commands.run()