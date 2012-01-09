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

