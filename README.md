# SQOL
> Structure Query Object Language

is the best data structure made by **JEDI Studio**

```sql
@entity User {
 @description "Description for entity here"
 @schema { 
   uId: number | string | null,
   username: string,
   address: object | array,
   job_status: boolean,
   workNumber: any
 },
 @validations {
   uId: { required: true, maxLength: 10 },
   userName: { required: true, minLength: 3 },
   address: { required: true },
   workNumber { required: false, default: 'No Number' }
 },
 @entries {
  (123231, "Jedi-Studio", { City: 'Dubai', Street: 'Sheikh Zayed street', buildingNo: 120, flatNo: 203 }, 009710545600431),
   // More enteries goes here
 }
}

// Mor entities goes here @validation and @description are optionals
```
