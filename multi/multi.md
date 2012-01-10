!SLIDE
# Multiple Commands

!SLIDE
# Multiple Commands
* Non-conditional: `cmd1 ; echo 'always'`
* Conditional:
  * `cmd1 && echo 'win'`
  * `cmd1 || echo 'fail'`

!SLIDE
# Every command returns a number
Zero is happy

!SLIDE commandline
# Conditional Commands
    $ rake test && growlnotify -m "yay"

!SLIDE commandline
# Conditional Commands
    $ rake test && growlnotify -m "yay" || growlnotify -m "boo!"


!SLIDE
# Chaining commands together

!SLIDE
# The Mighty Pipe

!SLIDE commandline incremental
Take the output of the previous command and pass it into the next

    $ cat multi.md | grep "Take the output"
    Take the output of the previous command and pass it into the next

!SLIDE smaller

# ls -alS /usr/bin | tr -s ' ' | cut -d ' ' -f 5,9

.note The long output of ls is sorted and then piped to the translate command. This removes the padding, leaving each field separated by a single space. cut then uses the space character as a field delimiter, and takes fields 5 and 8 from the output. What you get is a list of files, sorted by size, displaying only the size and the filename.

!SLIDE

# Redirection
echo "this" > file.txt
echo "this" >> file.txt
rake routes > routes.txt


