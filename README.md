# Data structure
type Task = {
  name: string,
  duration: number,
  location: string,
  priority: 0 | 1 | 2 | 3 | 4 | 5
}

# GPT-4 development prompts

## Scheduling algorithm
Assume the following types:
type Task = {
  name: string,
  duration: number,
  location: string,
  priority: 0 | 1 | 2 | 3 | 4 | 5,
  project: string
}
Give me TypeScript code for a task scheduling algorithm, that takes a list of objects of type Task and schedules them to timeslots across the next days based on the following criteria:
1. Highest priority tasks go first
2. Only schedule between 08:00 and 16:00 o clock.
3. No overlaps between tasks.
