## You're building an application that requires user login. Once logged in the user has a bunch of profile information and preference settings available to them. They will need to be able to set their birthday, gender, phone number and location (city, state, country). They should be able to provide text to tell about themselves. They also should be able to enable and disable the visibility of their birthday, gender, phone number, and location.

## User Authentification:
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

## User Profile:
{
  * Type: User Profile
  * Firstname: String
  * Lastname: String
  * birthday: Datetime
  * gender: String
  * PhoneNumber: String
    * Must be 10 digits
  * aboutMe: text
  * location: {
    * country: String
    * state: String
    * city: string

  }
  * DisabledFields: [ array of DisabledFields ]
  
}
