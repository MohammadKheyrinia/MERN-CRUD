*  مونگو دی بی بر خلاف دیتابیس های ریلیشنال نواسکیوال هست یعنی بجای اینکه دیتا رو به صورت ردیف و سطون ذخیره کنیم به صورت بی سان که شبیه جی سان هست ذخیره می کنیم *

#  document 
`{
    name:'mohammad',
    age:'20',
    password:'1234'
}` 

- مونگو شل رو با این سی ام دی ران می کنیم : mongosh
- showdbs نمایش دیتابیس
- use dbname برای سویچ کردن بین دیتابیس ها
- db.createCollection("") ساخت کالکشن
- db.dropDatabase() حذف دیتابیس
- db.students.insertOne({name:"mmd",age:"20"}) اضافه کردن داکیومنت
- db.students.insertMany({},{},{}) اضافه کردن چند داکیومنت
- db.students.find() ریترن کردن تمامی داکیومنت ها در کالکشن

# Datatypes
String - INT - Bool - Date object - NULL(novalue) - 
arrays["x","y","z"] - nested docs

# sort
`db.students.find().sort({})`

# update & delete
`db.students.updateOne({_id:ObjectId("67a1d2afa624fc0859110224")},{$unset:{age:""}})` 
- فرض مثال اینجا اول ای دی داکیومنت رو گرفتیم بعدش ایج رو کلن حذف کردیم ازش

`db.students.updateMany({},{$set:{age:true}})`

-  اینجا کل داکیومنت هارو ایجشون رو تروو کردیم

`db.students.deleteOne({name:"reza"})`

- هر نیمی که اسمش رضا هست رو پاک کن

