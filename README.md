# LVM Int Ass

## What is it?
LVM Int Ass is a assembler and interpreter for a learning virtual machine

## Flags
**CLI flags are set:**
- mode - assembler or interpreter mode (assemble, interpret)
- input_file (txt) - your txt file with data
- output_file (bin) - your output file (if it doesn't exist, the program will create it)
- log_file (xml) - your log file (if it doesn't exist, the program will create it)
- result_file (xml) - your file with results (if it doesn't exist, the program will create it)
- memory_range [start:end] - memory range for interpreter

## Examples

### Input File
```
A=30, B=1, C=51
A=1, B=1, C=817
A=7, B=6, C=3
A=45, B=0, C=7, D=2
```
### Example for interpreter
```
python main.py interpret --input_file output.bin --result_file result.json --memory_range 0:10

```
### Example for assembler
```
python main.py assemble --input_file input.txt --output_file output.bin --log_file log.json

```
