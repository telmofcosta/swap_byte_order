*NAME*
  *swap_byte_order* - swaps byte order of a file

*DESCRIPTION*

  the *swap_byte_order* utility swaps byte order of a file. Usefull to switch
  between big-endiand and little-endian or any other order in 4 bytes chunks.
  For that reason, it only deals with file with size multiple of 4 bytes. It
  writes to the standard output.

usage:
    swap_byte_order <filename> <swap_order>

    *filename*    Name of the file to change

    *swap_order*  A combination of the digits 0, 1, 2, 3 in any wanted order

*EXAMPLES*

   Having a file my_file.bin with content "0123456789abcdef"

   the command:

   swap_byte_order my_file.bin 1032

   will write to the standard output the following:

   1023546798abdcef
