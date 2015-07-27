% VIMCAT(1) vimcat user manual
% Abdó Roig-Maranges <abdo.roig@gmail.com>
% April 29, 2015

# NAME

vimcat - vim based syntax highlighter

# SYNOPSIS

vimcat [options] file1 [file2 ...]

# DESCRIPTION
cat's a file to stdout, syntax-highlighting it using vim as a backend.

On GitHub: <http://github.com/rkitover/vimpager>

To use a different vimrc with vimcat, put your settings into a ~/.vimcatrc.

To disable loading plugins, put "set noloadplugins" into a ~/.vimcatrc file.

If output is not a terminal, it will simply run cat, so using vimcat in
pipe commands is safe. If you actually need the ANSI codes, use -o .

# COMMAND LINE OPTIONS

## -c cmd

Run a vim command after opening the file. Multiple -c arguments are
supported.

## --cmd cmd

Run a vim command when entering vim before anything else. Multiple --cmd
arguments are supported.

## -u vimrc

Use an alternate .vimrc or .vimcatrc.

## -o output_file

Write output to output_file instead of the terminal. This works when
vimcat is not run on a terminal as well.

If output_file is "-" then output is written to STDOUT.