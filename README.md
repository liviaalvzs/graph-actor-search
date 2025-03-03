# Actor Graph Search - Degrees of Separation

Project made for submission on CS50 AI course. 

The objective is to find the shortest path of connections (degrees of separation) between two actors based on movies they have starred in.

```bash
python degrees.py [directory]
```

Where `[directory]` is the folder containing the CSV files. Defaults to `large`.

### Example

```bash
$ python degrees.py large               
Loading data...
Data loaded.
Name: Timothée Chalamet
Name: Heath Ledger
3 degrees of separation.
1: Timothée Chalamet and Zendaya starred in Dune
2: Zendaya and Michelle Williams starred in The Greatest Showman
3: Michelle Williams and Heath Ledger starred in Brokeback Mountain
```

## Functions

- `load_data(directory)`: Loads CSV data.
- `main()`: Runs the program.
- `shortest_path(source, target)`: Finds the shortest path between two actors.
- `person_id_for_name(name)`: Resolves actor names to IDs.
- `neighbors_for_person(person_id)`: Returns movies and actors that are connected.
