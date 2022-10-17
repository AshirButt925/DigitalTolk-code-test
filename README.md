# DigitalTolk-code-test
1. the authentication system is not good. I saw in this project you are check user authentication via .env variables that's is the not good practice becase the .env file is not same for the all users. For example if multiple developers are working on this project may the all the developers have different envirment file may some have not have the checking variables of admin or supper admin then the logic are implementing in this project is not good. you must have to use any authentication system like oAuth / JWT etc or you may use your own roles or may be use LARAVEL spatie package for roles and permissions.
2. the repository pattren that are use in this project is good.
3. i saw there are many loops used in this project and alot of if else conditions over there.the useage of loops too much is not good and also the way of usage loops is also not Good. For example, you are using loop before use loop there should be the way to check the variable is it array? or is it not an empty array if the array is empty then the loop throw an exception this is not array etc.. so in simple words must check the array type before using any loop.
4. the saw in this project there are the usage of egger loading this is the way that i like.
5. check the whereHas feedback before checking where ignore_feedback because
   the whereHas clauser gets all the record again and the purpose of the $allJobs->where('ignore_feedback', '0') clause
   is died.
6. I also noticed you are using if else to check the where conditions i think the is also not good practice to use if else you may use where clause and also orWhere clause over there to check the if table have the column and value or not.
7. The concepts of re-usability is not used in this project of the conditions are recoded overthere that i didn't like
8. less usage of re-usability and also not used the pre defiened methods like array_map or collections to genereate the array. 