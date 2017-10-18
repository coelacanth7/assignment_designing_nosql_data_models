## You're building a restaurant table reserving app that allows users to reserve tables for specified numbers of people. The app will need to show only tables that are available and the times they are available. The app will need to store reservations under a given name with a phone number and number of guests.

## User Profile

{
  Type: user profile
  name: String
  PhoneNumber: string

}

## reservation

{
  Type: reservation
  guestName: userProfile.name
  GustPhoneNumber: userProfile.PhoneNumber
  numberofGuests: integer
  table: Table.TableNum

}


## table

{
  Type: table
  TableNum: integer
  NumOfSeats: integer
  availability: {
    Date: {
      timeslot: integer
      available: boolean
      
    }

  }

}
