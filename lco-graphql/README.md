# lco-graphql

A standard babel setup
Starter project setup for upcoming crash courses

#### documentation: https://graphql.org/learn/

##### repo : https://github.com/rupaku/graphql

##### npm install // to install dependency

##### npm install express graphql express-graphql nanoid

##### npm start // to run

##### input:

mutation{
createCourse(input:{
courseName:"JS"
price:199
stack:MOBILE
teachingAssists:[
{
firstName:"rupa"
lastName:"Kumari"
experience:1
},
{
firstName:"rk"
lastName:"surname"
experience:1
}
]
}){
id,
courseName
}

}

##### output

{
"data": {
"createCourse": {
"id": "f0DgnK-C9ksm01MjSE8AK",
"courseName": "JS"
}
}
}

##### input

query{
getCourse(id:"f0DgnK-C9ksm01MjSE8AK"){
id
teachingAssists{
experience
}
}
}

##### output

{
"data": {
"getCourse": {
"id": "f0DgnK-C9ksm01MjSE8AK",
"teachingAssists": [
{
"experience": 1
},
{
"experience": 1
}
]
}
}
}
