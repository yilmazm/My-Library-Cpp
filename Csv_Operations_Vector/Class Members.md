# Functions and variables

## Private Variables

|Type|Variable|
|-------------|-------------|
|char|cruncher|
|std::string|fileName|
|std::vector<std::vector<std::string>>|csvTable|

## Public Functions

### Constructors and Destructer

|Type|Variable|
|-------------|-------------|
||CsvOp(char inCruncher = ';');|
||CsvOp(std::string inFileName, char inCruncher = ';');|
||CsvOp(std::vector<std::vector<std::string>> inCsvTable, const char inCruncher = ';');|
||~CsvOp();|

### ... functions

|Type|Variable|
|-------------|-------------|
|void|sort_by_column(int columnOrder);|
|void|read_csv_file();|
|std::vector<std::string>|column_list(unsigned int returnColumn, unsigned int searchColumn=0, std::string searchString="");|
|std::vector<std::vector<std::string>>|find_row_by_column(unsigned int searchColumn, std::string searchString);|
|bool|write_to_file();|
|bool|write_to_file(const std::string &inFileName, const char &inCruncher);|

### Inline functions

|Type|Variable|
|-------------|-------------|
|void|clear();|
|void|insert(int lineOrder, std::vector<std::vector<std::string>> anotherTable);|
|void|insert(int lineOrder, const std::vector<std::string> &line);|

### Static functions

|Type|Variable|
|-------------|-------------|
|std::vector<std::string>|line_to_vector(const std::string &line, char seperator);|

### Getters and Setters

|Type|Variable|
|-------------|-------------|
|char|getCruncher() const;|
|void|setCruncher(char value);|
|std::string|getFileName() const;|
|void|setFileName(const std::string &value);|
|std::vector<std::vector<std::string>>|getCsvTable() const;|

### Garbarage functions

|Type|Variable|
|-------------|-------------|
|void|print_table();|
|void|print_table(std::vector<std::vector<std::string>> table);|
