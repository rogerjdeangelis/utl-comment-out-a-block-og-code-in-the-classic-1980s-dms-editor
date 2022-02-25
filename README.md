    %let pgm=utl-comment-out-a-block-of-code-in-the-classic-l980s-dms-editor;

    Comment out a block of code in the classic 1980s dms editor

      Two methods

          1. '/*' and '*/'
          2, '%macro skip;' and '%mend skip;'

    The key function is that the find command moves the cursor.
    Cursor location and cursor position no longer work?

    Note I have been doing this since the 1980's.
    I feel I can do anything the enhanced editors do and much more.


    Stackoverflow
    https://tinyurl.com/2p9y44s7
    https://stackoverflow.com/questions/71229235/toggle-comments-keyboard-shortcut-ctrl-does-not-work

    github
    https://tinyurl.com/5xxbs9js
    https://github.com/rogerjdeangelis/utl-comment-out-a-block-og-code-in-the-classic-1980s-dms-editor

    https://goo.gl/xXYQ3d
    https://github.com/rogerjdeangelis/utl_classic_sas_editor_display_manager_commands_improved
     _                   _
    (_)_ __  _ __  _   _| |_
    | | `_ \| `_ \| | | | __|
    | | | | | |_) | |_| | |_
    |_|_| |_| .__/ \__,_|\__|
            |_|

    Command ===>

    00001
    00002 data class;
    00003  set sashelp.class;
    00004 run;quit;
    00005
    00006
                 _               _
      ___  _   _| |_ _ __  _   _| |_
     / _ \| | | | __| `_ \| | | | __|
    | (_) | |_| | |_| |_) | |_| | |_
     \___/ \__,_|\__| .__/ \__,_|\__|
                    |_|
    Command ===>

    00001 /*
    00002 data class;
    00003  set sashelp.class;
    00004 run;quit;
    00005 */
    00006

    Command ===>

    00001 %macro skip;
    00002 data class;
    00003  set sashelp.class;
    00004 run;quit;
    00005 %mend skip;
    00006
     _ __  _ __ ___   ___ ___  ___ ___
    | `_ \| `__/ _ \ / __/ _ \/ __/ __|
    | |_) | | | (_) | (_|  __/\__ \__ \
    | .__/|_|  \___/ \___\___||___/___/
    |_|

    You need to highlight lines 00001 through 00005
    And tyoe the commands c ' ' '/*';f ';' last;c ' ' '*/';
    on the command line. Note you can put the command on a function key,
    mouse acton, or command macro.

    It is a shame but we have been losing scripting commands over the years.
    ISPF was much more powerfull.

    Command ===> c ' ' '/*';f ';' last;c ' ' '*/';

    00001
    00002 data class;
    00003  set sashelp.class;
    00004 run;quit;
    00005
    00006

    Command ===> c ' ' '%macro skip;';f ';' last;c ' ' '%mend skip;';

    00001
    00002 data class;
    00003  set sashelp.class;
    00004 run;quit;
    00005
    00006
