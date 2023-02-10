# README

This README would normally document whatever steps are necessary to get the
application up and running.

Things you may want to cover:

* Ruby version

* System dependencies

* Configuration

* Database creation

* Database initialization

* How to run the test suite

* Services (job queues, cache servers, search engines, etc.)

* Deployment instructions

* ...


irb(main):008:0> course1.students
  Student Load (0.3ms)  SELECT "students".* FROM "students" INNER JOIN "course_students" ON "students"."id" = "course_students"."student_id" WHERE "course_students"."course_id" = ?  [["course_id", 1]]                                                          
=>                                                                       
[#<Student:0x000001e931354320                                            
  id: 1,                                                                 
  first_name: "John",                                                    
  last_name: "Doe",                                                      
  created_at: Fri, 10 Feb 2023 01:20:36.252145000 UTC +00:00,            
  updated_at: Fri, 10 Feb 2023 01:20:36.252145000 UTC +00:00>,           
 #<Student:0x000001e931354168                                            
  id: 2,                                                                 
  first_name: "Jane",                                                    
  last_name: "Doe",                                                      
  created_at: Fri, 10 Feb 2023 01:20:47.689622000 UTC +00:00,            
  updated_at: Fri, 10 Feb 2023 01:20:47.689622000 UTC +00:00>]           
irb(main):009:0>

irb(main):009:0> course2.students
  Student Load (0.4ms)  SELECT "students".* FROM "students" INNER JOIN "course_students" ON "students"."id" = "course_students"."student_id" WHERE "course_students"."course_id" = ?  [["course_id", 2]]         
=> 
[#<Student:0x000001e930740548
  id: 2,
  first_name: "Jane",
  last_name: "Doe",
  created_at: Fri, 10 Feb 2023 01:20:47.689622000 UTC +00:00,
  updated_at: Fri, 10 Feb 2023 01:20:47.689622000 UTC +00:00>]
irb(main):010:0>