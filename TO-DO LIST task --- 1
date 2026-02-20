tasks = []

while True:
    print("\n--- TO-DO LIST ---")
    print("1. Add Task")
    print("2. View Tasks")
    print("3. Mark Task as Done")
    print("4. Delete Task")
    print("5. Exit")

    choice = input("Enter your choice (1-5): ")

    if choice == "1":
        task = input("Enter task: ")
        tasks.append([task, "Not Done"])
        print("Task added!")

    elif choice == "2":
        if not tasks:
            print("No tasks found.")
        else:
            print("\nYour Tasks:")
            for i, t in enumerate(tasks):
                print(f"{i+1}. {t[0]} - [{t[1]}]")

    elif choice == "3":
        if not tasks:
            print("No tasks to mark.")
        else:
            try:
                number = int(input("Enter task number to mark as done: "))
                if 1 <= number <= len(tasks):
                    tasks[number - 1][1] = "Done"
                    print("Task marked as done!")
                else:
                    print("Invalid task number.")
            except ValueError:
                print("Please enter a valid number.")

    elif choice == "4":
        if not tasks:
            print("No tasks to delete.")
        else:
            try:
                number = int(input("Enter task number to delete: "))
                if 1 <= number <= len(tasks):
                    deleted = tasks.pop(number - 1)
                    print(f"Deleted task: {deleted[0]}")
                else:
                    print("Invalid task number.")
            except ValueError:
                print("Please enter a valid number.")

    elif choice == "5":
        print("Goodbye!")
        break

    else:
        print("Invalid choice. Please enter a number from 1 to 5.")
