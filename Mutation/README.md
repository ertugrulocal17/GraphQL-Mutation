# GraphQL Mutation

## Codes

```
query getAllUser {
  users {
    id
    username
    email
  }
}

mutation addNewUser {
  addUser(
    data: { username: "Yeni başka kullanici", email: "yenii@gmail.com" }
  ) {
    id
    username
    email
  }
}

mutation updateUser {
  updateUser(
    id:"1"
    data:{
      username:"Kullanici guncellendi"
      email:"guncel@gmail.com"
    }
  ){
    id
    username
    email
  }
}

mutation deleteUser{
  deleteUser(
    id:"1"
  ){
    id
    username
    email
  }
}

mutation deleteAllUsers{
  deleteAllUser{
    count
  }
}

query listAllEvents {
  events {
    id
    title
    desc
    date
    from
    to
    location_id
    user_id
  }
}

mutation addNewEvent {
  addEvent(
    data: {
      title: "New Event 1"
      desc: "New Event Desc 1"
      date: "10/10/2023"
      from: "13:00"
      to: "14:00"
      location_id: "3"
      user_id: "3"
    }
  ) {
    id
    title
    desc
    date
    from
    to
    location_id
    user_id
  }
}

mutation updateEvent{
  updateEvent(
    id:"1"
    data:{
      title:"Guncellenen event"
      desc:"Guncellentn desc"
      date:"12/12/2022"
      from:"22.22"
      to:"23.23"
      location_id:"1"
      user_id:"1"
    }
  ){
    id
    title
    desc
    date
    from
    to
    location_id
    user_id
  }
}

mutation deleteEvent{
  deleteEvent(
    id:"1"
  ){
    id
    title
    desc
    date
    from
    to
    location_id
    user_id
  }
}

mutation deleteAllEvents{
  deleteAllEvent{
    count
  }
}


query listAllLocations {
  locations {
    id
    name
    desc
    lat
    lng
  }
}
mutation addLocation {
  addLocation(
    data:{
    name: "New Location 1"
    desc: "New Location Desc 1"
    lat: -22.11
    lng: -33.12
    }
  ) {
    id
    desc
    lat
    lng
  }
}
mutation updateLocation{
  updateLocation(
    id:"1"
    data:{
      name:"Guncellenen Location"
      desc:"Guncellenen Desc"
      lat:-22.22
      lng:-33.33
    }
  ){
    id
    name
    desc
    lat
    lng
  }
}

mutation deleteLocation{
  deleteLocation(
    id:"1"
  ){
    id
    name
    desc
    lat
    lng
  }
}

mutation deleteAllLocation{
  deleteAllLocation{
    count
  }
}

query listAllParticipants {
  participants {
    id
    user_id
    event_id
  }
}

mutation addNewParticipant {
  addParticipant(data: { user_id: "3", event_id: "3" }) {
    user_id
    event_id
  }
}

mutation updateParticipant{
  updateParticipant(
    id:"1"
    data:{
      user_id:"20"
      event_id:"30"
    }
  ){
    id
    user_id
    event_id
  }
}

mutation deleteParticipant{
  deleteParticipant(
    id:"1"
  ){
    id
    user_id
    event_id
  }
}

mutation deleteAllParticipants {
  deleteAllParticipant{
    count
  }
}
```
