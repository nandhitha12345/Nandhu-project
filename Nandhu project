def read_and_write_txt():
    try:
        # Writing to a file
        with open('sample.txt', 'w') as file:
            file.write("Hello World!\n")
            file.write("This is a sample file.\n")
            file.write("Used for file operations in Python.\n")
        
        # Reading from the file
        with open('sample.txt', 'r') as file:
            content = file.read()
            print("File Content:\n", content)
            
    except Exception as e:
        log_error(f"Error in read_and_write_txt: {e}")

def count_words_lines():
    try:
        with open('sample.txt', 'r') as file:
            lines = file.readlines()
            line_count = len(lines)
            word_count = sum(len(line.split()) for line in lines)
            print(f"Total Lines: {line_count}")
            print(f"Total Words: {word_count}")
    except Exception as e:
        log_error(f"Error in count_words_lines: {e}")

def parse_csv_manually():
    try:
        # Sample CSV content written manually
        with open('data.csv', 'w') as f:
            f.write("name,age,city\n")
            f.write("Alice,30,New York\n")
            f.write("Bob,25,Los Angeles\n")
            f.write("Charlie,35,Chicago\n")

        # Reading CSV manually
        with open('data.csv', 'r') as f:
            lines = f.readlines()
            headers = lines[0].strip().split(",")
            print("Headers:", headers)
            for line in lines[1:]:
                values = line.strip().split(",")
                record = dict(zip(headers, values))
                print("Record:", record)
    except Exception as e:
        log_error(f"Error in parse_csv_manually: {e}")

def log_error(message):
    with open('error_log.txt', 'a') as error_file:
        error_file.write(message + "\n")

# Call all functions
read_and_write_txt()
count_words_lines()
parse_csv_manually()
