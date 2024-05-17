## Code
```c
#include <stdio.h>
// defining employee structure
struct employee{
    char name[20];
    int date,month,year,salary;
};

void main(){
    int n;
    printf("enter number of persons to enter: ");
    scanf("%d",&n);
    struct employee p[n];
    for(int i=0;i<n;i++){  // iterating through p array to add employee
        printf("Enter name : ");
        scanf("%s",p[i].name);
        printf("Enter date of birth: ");
        scanf("%d %d %d",
        &p[i].date,
        &p[i].month,
        &p[i].year
        );
        printf("enter salary: ");
        scanf("%d",&p[i].salary);
        printf("Details of %s added!\n\n",p[i].name);
    }
    // printing the details of the employees
    printf("=== Details of Employees added ===\n");
    for(int i=0;i<n;i++){
        printf("Detailes of %s\n",p[i].name);
        printf("Name : %s\n",p[i].name);
        printf("DOB: %d / %d / %d\n",
        p[i].date,
        p[i].month,
        p[i].year
        );
        printf("Salary : %d\n",p[i].salary);
    }
}
```
## Algorithm
 
### Step 1 : Start

### Step 2 : Define the structure
- initialize name,date of birth and salary.

### Step 3 : Initailize n number of employees to be added

### Step 4 : Read n

### Step 5 : Define the structure variable as an array say,arr[n]

### Step 6 : IF i is less than n, repeat 6.1 to 6.3
- 6.1 read name and store to the array (like, arr[i].name) 
- 6.2 read dob
- 6.3 read salary

### Step 7 : Print the details of the employees by iterating through array from i = 0 to i = n

### Step 8 : Stop