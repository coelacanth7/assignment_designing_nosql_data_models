## You're building a backend for a university that requires students to be able to login. Once logged in, the students can view the exam grades for their classes. They should be able to view results by semester. Each semester should only show the classes in which that student is enrolled that semester.

## User Authentification

{
  * Type : User Authentification
  * Username: String
    * Must be unique
    * Contain only letters and numbers
  * Password: String
    * Must be at least 8 characters
  * email: String
    * Must contain @ symbol  

}

## semester for userProfile

{
  * Type: semester for userProfile
  * semesterNum: integer
  * userProfile: userAuthentification.username
  * classes: [ Array of enrolled classes]
    * map to userGrades.classes.class.classname

}

## User grades:

{
  * type: userGrades
  * userProfile: userAuthentification.username
  * OverallGrade: integer
    * between 0 - 4
  * classes: {
    * class: {
      * classname: string
      * grades: [ arrray of grades ]
        * each position is exam number
        
    }

  }

}
