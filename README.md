# visual-increment.vim

### Description

This plugin adds a simple functionality for creating increasing and decreasing
number or letter sequences on multiple lines via visual mode.

Simply select the desired columns via visual mode and use standard vim mapping
for adding or subtracting.

### Usage

1. For example we have an array of 5 items, and we would like to define them:

        char example[5];
        example[0] = 'e';
        example[0] = 'e';
        example[0] = 'e';
        example[0] = 'e';
        example[0] = 'e';

2. Press `<C-V>` at the first index and select all the index columns on multiple
   lines, press `<C-A>`

        char example[5];
        example[0] = 'e';
        example[1] = 'e';
        example[2] = 'e';
        example[3] = 'e';
        example[4] = 'e';

3. Repeat the same by selecting the char values and press `<C-X>`

        char example[5];
        example[0] = 'e';
        example[1] = 'd';
        example[2] = 'c';
        example[3] = 'b';
        example[4] = 'a';

4. You can use `[count]` to define the increment step between each line. For
   example by pressing `5<C-A>` at the index column from point 1., you will get:

        char example[5];
        example[5] = 'e';
        example[10] = 'e';
        example[15] = 'e';
        example[20] = 'e';
        example[25] = 'e';

### License

visual-increment is released under the MIT license:

Copyright 2011 Matej Svec. All rights reserved.

Permission is hereby granted, free of charge, to any person obtaining a copy of
this software and associated documentation files (the "Software"), to deal in
the Software without restriction, including without limitation the rights to
use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
the Software, and to permit persons to whom the Software is furnished to do so,
subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

The software is provided "as is", without warranty of any kind, express or
implied, including but not limited to the warranties of merchantability, fitness
for a particular purpose and noninfringement. In no event shall the authors or
copyright holders be liable for any claim, damages or other liability, whether
in an action of contract, tort or otherwise, arising from, out of or in
connection with the software or the use or other dealings in the software.

