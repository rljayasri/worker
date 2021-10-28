# Posty App - Cloudflare workers
Consists of files written with typescript template for the following apis:
* GET /api/posts
Gets all the posts from KV
https://posty-worker-api.jramakrishnan.workers.dev/api/posts
* POST /api/makepost
Api to create a post and write it into KV
https://posty-worker-api.jramakrishnan.workers.dev/api/makepost
Example Body:
{
"title":"New Post",
"username":"JayasriRamakrishnan",
"content":"I had a wonderful day",
"image":"https://pbs.twimg.com/profile_images/1313131647315910666/opulcRqc.jpg"
}
* POST /api/updatepost
Additional API to update likes and comments from web app for the respective posts
https://posty-worker-api.jramakrishnan.workers.dev/api/updatepost
Example body:
{"title":"New Post",
"username":"JayasriRamakrishnan",
"content":"I had a wonderful day",
"image":"https://pbs.twimg.com/profile_images/1313131647315910666/opulcRqc.jpg",
"postedAt":"10/28/2021, 05:00:05 AM", 
"love" : 4, 
"comments": []
}

