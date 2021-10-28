# Posty App - Cloudflare workers  
##Workers URL/Homepage: https://posty-worker-api.jramakrishnan.workers.dev/  
Consists of files written with typescript template for the following apis:
* GET /api/posts
Gets all the posts from KV
https://posty-worker-api.jramakrishnan.workers.dev/api/posts   
<img width="1423" alt="Screen Shot 2021-10-28 at 12 05 02 PM" src="https://user-images.githubusercontent.com/91042044/139319504-5619d29d-386f-4eaf-982b-1687fefd886c.png">

* POST /api/makepost
Api to create a post and write it into KV
https://posty-worker-api.jramakrishnan.workers.dev/api/makepost  
Example Body:
```
{
"title":"New Post",
"username":"JayasriRamakrishnan",
"content":"I had a wonderful day",
"image":"https://pbs.twimg.com/profile_images/1313131647315910666/opulcRqc.jpg"
}
```
<img width="1423" alt="Screen Shot 2021-10-28 at 12 05 02 PM" src="https://user-images.githubusercontent.com/91042044/139319582-aefc2bec-0766-4349-81ab-155e3522231a.png">

* POST /api/updatepost
Additional API to update likes and comments from web app for the respective posts
https://posty-worker-api.jramakrishnan.workers.dev/api/updatepost  
Example body:
```
{
"title":"New Post",
"username":"JayasriRamakrishnan",
"content":"I had a wonderful day",
"image":"https://pbs.twimg.com/profile_images/1313131647315910666/opulcRqc.jpg",
"postedAt":"10/28/2021, 05:00:05 AM", 
"love" : 4, 
"comments": []
}
```
<img width="1425" alt="Screen Shot 2021-10-28 at 10 17 22 AM" src="https://user-images.githubusercontent.com/91042044/139319631-27f3c070-631b-4ee2-89e4-39085ad4b26c.png">

