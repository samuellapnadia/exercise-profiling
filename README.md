# MODULE 5 
## Performance Testing (using JMeter)
### /all-student-name 
![View Results Tree](screenshots/asn1.png)
*View Results Tree.*
![View Results in Table](screenshots/asn2.png)
*View Results in Table.*
![Summary Report](screenshots/asn3.png)
*Summary Report.*
![Graph Results](screenshots/asn4.png)
*Graph Results.*

### /highest-gpa
![View Results Tree](screenshots/gpa1.png)
*View Results Tree.*
![View Results in Table](screenshots/gpa2.png)
*View Results in Table.*
![Summary Report](screenshots/gpa3.png)
*Summary Report.*
![Graph Results](screenshots/gpa4.png)
*Graph Results.*

### Command Line
#### /all-student-name
![Command Line /all-student-name](screenshots/asncl.png)
*Command Line.*
![Log File /all-student-name](screenshots/asnlog.png)
*Log File.*

#### /highest-gpa
![Command Line /highest-gpa](screenshots/gpacl.png)
*Command Line.*
![Log File /highest-gpa](screenshots/gpalog.png)
*Log File.*

## Profiling
### Optimization Results
#### /all-student-name 
![Command Line /all-student-name](screenshots/asn2.png)
*Before Optimization.*
![Log File /all-student-name](screenshots/asnafter.png)
*After Optimization.*

#### /highest-gpa
![Command Line /highest-gpa](screenshots/gpa2.png)
*Before Optimization.*
![Log File /highest-gpa](screenshots/gpaafter.png)
*After Optimization.*

### Explanation
Before optimization, the runtime for each thread request was significantly high, leading to long sample times for the /all-student-name and /highest-gpa endpoints.
To address this, I optimized key methods such as findStudentWithHighestGpa() and joinStudentNames() by reducing inefficient loops and utilizing database queries effectively.
After implementing these optimizations, the runtime for both endpoints dropped significantly, improving response times and overall performance.