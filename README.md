# proctee
Tee stdin to program

    USAGE:

        proctee [-o out] ... -- [prog ...]

    Pipe stdin to stdout as-is, while teeing stdin to "prog ..." and piping
    prog's stdout to one or more `out's.

    -o      Specifies the output file that the prog's stdout should be written to.
            Multiple -o can be specified.

    Visually:

            STDIN --> STDOUT
              |
              v
             prog
              |
              v
         out1, out2, ...

