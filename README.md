#inlcude<stdio.h>
struct employee
{
  string ename;
  int age,phn_no;
  int salary;
};
 void display(struct employee emp[], int n)
 {
    printf("Name\tAge\tPhone Number\tSalary\n");
    for(int i=0;i<n;i++)
    {
       printf("\t",emp[i].ename);
       printf("%d\t",emp[i].age,emp[i].phn_no,emp[i].salary);
     }
  }
  
  int main()
  {
     int n=3;
     struct employee emp[n];
     
     emp[0].ename="Chirag";
     emp[0].age=24;
     emp[0].phn_no =1234567788;
     emp[0].salary=20000;
     
     emp[1].ename="Arnav";
     emp[1].age=31;
     emp[1].phn_no = 1234567891;
     emp[1].salary=56000;
     
     emp[2].ename="Shivam";
     emp[2].age=45;
     emp[2].phn_no = 8881101111;
     emp[2].salary = 30500;
     
     display(emp,n);
     
     return 0;
   }  
     
