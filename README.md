# file-hundling
# File Read & Write Challenge 🖋️

# Read content from an existing file
try:
    with open("input.txt", "r") as infile:
        content = infile.read()

    # Modify the content (example: converting all text to uppercase)
    modified_content = content.upper()

    # Write the modified content to a new file
    with open("output.txt", "w") as outfile:
        outfile.write(modified_content)

    print("File has been successfully read, modified, and saved as 'output.txt'.")

except FileNotFoundError:
    print("Error: The input file does not exist.")
except IOError:
    print("Error: There was an issue reading or writing the file.")
2
# Error Handling Lab 🧪

filename = input("Enter the filename: ")

try:
    with open(filename, "r") as file:
        content = file.read()
    print("File content:")
    print(content)

except FileNotFoundError:
    print(f"Error: The file '{filename}' does not exist.")
except IOError:
    print(f"Error: Could not read the file '{filename}'.")





