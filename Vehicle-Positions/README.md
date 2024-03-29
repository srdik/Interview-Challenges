# Vehicle Position Challenge

## Task
The binary data file _positions.dat_ contains a position for each of 2 million vehicles. Your task is to write a program that finds the nearest vehicle 
positions in the data file to each of the 10 co-ordinates provided in the table below. Your program should be able to find all 10 closest positions in less time 
than the benchmark approach that simply loops through each of the 2 million positions and keeps the closest to each of the 10 co-ordinates. The challenge is to 
optimize for speed and improve on the benchmark to the best of your ability.

## Specifics
  * Use Git to clone the project template to your PC
  * Use C language and GCC compiler toolchain (recommend MinGW/MSYS for Windows users)
  * Add your code to _solution.c_
  * Complete _makefile_ with rules to compile and clean
     * Compile: Should only recompile code when any source code changed
       * Disable optimization
       * Disable generation of debug information (for final submission)
       * Enable all general warnings
       * Enable conversion warnings
     * Clean: Should not show error if files does not exist
  * Add code to time execution of the content of the _main()_ function with millisecond accuracy

## How to submit your solution
 * Create a private repository on Github (free)
 * Add the following contributors to your repository:
   * https://github.com/ErnestL
   * https://github.com/CarloPutter
 * Create a pull request for your solution
 * Notify us of completion with an email containing your repository URL
   * Nix.Stephens@mixtelematics.com
   * Ernest.Lotter@mixtelematics.com
   * Carlo.Putter@mixtelematics.com

## Additional information

### Structure of the objects within _position.dat_:

Field               |Data Type
--------------------|--------------------------------------------------------
Position ID         |32 bit integer
Vehicle Registration|Null terminated string (ASCII)
Latitude            |32 bit floating point
Longitude           |32 bit floating point
UTC Timestamp       |64 bit unsigned integer (number of seconds since Epoch)

### 10 co-ordinates:

Position  |1          | 2        | 3         | 4        | 5        | 6         | 7         | 8        | 9        | 10
----------|-----------|----------|-----------|----------|----------|-----------|-----------|----------|----------|------------
Latitude  |34.544909  |32.345544 |33.234235  |35.195739 |31.895839 |32.895839  |34.115839  |32.335839 |33.535339 |32.234235
Longitude |-102.100843|-99.123124|-100.214124|-95.348899|-97.789573|-101.789573|-100.225732|-99.992232|-94.792232|-100.222222
