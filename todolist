
tasks = []

def add_task(task):

    tasks.append(task)
    print(f"Added task: {task}")

def view_tasks():

    if not tasks:
        print("No tasks available.")
    else:
        for i, task in enumerate(tasks, 1):
            print(f"{i}. {task}")

def mark_task_done(task_index):

    try:
        task_index = int(task_index) - 1
        if 0 <= task_index < len(tasks):
            del tasks[task_index]
            print(f"Task {task_index+1} marked as done.")
        else:
            print("Invalid task index.")
    except ValueError:
        print("Invalid task index.")

def main():
    while True:
        print("Todo List Menu:")
        print("1. Add task")
        print("2. View tasks")
        print("3. Mark task as done")
        print("4. Quit")

        choice = input("Enter your choice: ")

        if choice == "1":
            task = input("Enter new task: ")
            add_task(task)
        elif choice == "2":
            view_tasks()
        elif choice == "3":
            task_index = input("Enter task index to mark as done: ")
            mark_task_done(task_index)
        elif choice == "4":
            print("Goodbye!")
            break
        else:
            print("Invalid choice. Please try again.")

if __name__ == "__main__":
    main()
