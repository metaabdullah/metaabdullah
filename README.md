A standard game of Tic-Tac-Toe in Leo.

⭕ ❕ ⭕ ❕ ❌

➖ ➕ ➖ ➕ ➖

⭕ ❕ ⁣❌ ❕ ⭕

➖ ➕ ➖ ➕ ➖

❌ ❕ ❌ ❕ ⭕

Representing State
Leo allows users to define composite data types with the struct keyword. The game board is represented by a struct called Board, which contains three Rows. An alternative representation would be to use an array, however, these are not yet supported in Leo.

Language Features
struct declarations
conditional statements
early termination. Leo allows users to return from a function early using the return keyword.
Running the Program
Leo provides users with a command line interface for compiling and running Leo programs. Users may either specify input values via the command line or provide an input file in inputs/.

Providing inputs via the command line.
Run
leo run <function_name> <input_1> <input_2> ...
See ./run.sh for an example.

Using an input file.
Modify inputs/tictactoe.in with the desired inputs.
Run
leo run <function_name>
Executing the Program
leo execute <function_name> <input_1> <input_2> ...
Playing the Game
1. Create a new game board
leo run new
0	0	0
0	0	0
0	0	0
2. Player 1 makes a move
leo run make_move 1u8 1u8 1u8 "{ r1: { c1: 0u8, c2: 0u8, c3: 0u8 }, r2: { c1: 0u8, c2: 0u8, c3: 0u8 }, r3: { c1: 0u8, c2: 0u8, c3: 0u8 } }"
1	0	0
0	0	0
0	0	0
3. Player 2 makes a move
leo run make_move 2u8 2u8 2u8 "{ r1: { c1: 1u8, c2: 0u8, c3: 0u8 }, r2: { c1: 0u8, c2: 0u8, c3: 0u8 }, r3: { c1: 0u8, c2: 0u8, c3: 0u8 } }"
1	0	0
0	2	0
0	0	0
