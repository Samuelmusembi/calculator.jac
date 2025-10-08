walker Calculator {
    has num1: int
    has num2: int;
    has choice: str;

    can enter {
        print("🧮 Welcome to Jac Calculator!");
        print("Choose an operation: +, -, *, /");

        take input "Enter choice (+, -, *, /): " into choice;
        take input "Enter first number: " into num1;
        take input "Enter second number: " into num2;

        if choice == "+" {
            print(num1 + num2);
        } elif choice == "-" {
            print(num1 - num2);
        } elif choice == "*" {
            print(num1 * num2);
        } elif choice == "/" {
            if num2 != 0 {
                print(num1 / num2);
            } else {
                print("❌ Error: Division by zero!");
            }
        } else {
            print("⚠️ Invalid choice.");
        }
    }
}

with entry:__main__ {
    root spawn Calculator();
}
# calculator.jac
ac Projects – A collection of beginner-friendly programs written in the Jac programming language. Includes simple examples like a calculator, guessing game, and more to explore Jac’s syntax and features.
