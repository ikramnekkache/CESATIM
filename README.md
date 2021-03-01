# CESATIM
This package contains the source code of the CESATIM Solver proposed in I. Nekkache, S. Jabbour, L. Sais:   Towards a Compact SAT-based Encoding ofItemset Mining Tasks. In: The 18th International Conference on the Integration of Constraint Programming, Artificial Intelligence, and Operations Research, Vienna, Austria, July 5th-July 8th, 2021. 

The source codes is already compiled.
In case you modify the code, make sur you compile the code in core folder with one of the following commands:
make 
or 
make CC=gcc-9 CXX=g++-9 

To run the CESATIM Solver , execute the following command in core folder: 

time -p ./CESATIM database_name -minSupport=minsupp -ncores=1 -verb=3

        a- database_name: name of the database (a file having for extension .txt or .dat) 
  
        b- minSupport: a minimal threshold of support that must be satisfied for enumerating the frequent itemsets in the transactions database.

        c- ncores: the number of cores used in CESATIM by the CPU for solving the problem .
        d- verb: used to print some information about the final result such as the number of clauses and the number of models founded.

Example: ./CESATIM chess.dat -minSupport=250 -ncores=1 -verb=3

For more options use the following command:

./CESATIM --help
