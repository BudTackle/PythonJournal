def main():
    while True:
        try:
            # Prompt the user to enter numbers separated by spaces
            numbers = input("Please enter a list of numbers separated by spaces: ")

            # Split the input string into individual number strings
            number_list = numbers.split()

            # Convert the number strings to floats
            number_list = [float(num) for num in number_list]

            # Calculate the average
            average = sum(number_list) / len(number_list)

            # Display the result
            print(f"The average of the entered numbers is: {average}")
            break
        except ValueError:
            print("Please enter valid numbers separated by spaces.")
            continue

# Run the program
if __name__ == "__main__":
    main()
