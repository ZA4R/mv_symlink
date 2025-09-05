# mv_symlink
A Bash wrapper for 'mv' which which adds '-l' flag that moves a folder as usual and additionally create a soft link in the original location pointing to the new location. I forget the symlink cmd all the time so this is a neccessity :)

# USAGE
'''bash
mv -l src dest'''

output:
'''bash
mv src dest
ln -s dest src'''

# NOTES
- Requires Bash
- Passes all flags to mv aside from '-l'
- Does not inform you of overwrite
