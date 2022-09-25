# A--Mongo-Blogger-pt2
Assignment
const getPosts = (searchObject, sortObject, limit, skip) => {
const posts = db.blogs.find(searchObject).toArray()
return posts
}

// 1. Update searchObject so that the query in getPosts searches for 
//all posts with a createdAt date greater than May 1, 2022
const searchObject = {
    db.BlogsDB.findAll({
      createdAt:{$gt:Date("5/1/2022") 
    }
})
const sortObject = {}
const limit = 10
const skip = 0

const createPost = (newPost) => {
const id = getUUID()
const createdAt = Date()
const lastModified = Date()
const postData = {
  createdAt: "Date",
  lastModified: "Date",
  id:"getUUID"
}
db.BlogDB.insertOne(postData)
}

const newPost = {
title: "The Dark Knight Movie Review",
text: "This movie was amazing because I am Batman.",
author: "Bruce Wayne",
categories: ["superhero", "action", "thriller"]
}
// createPost(newPost)
//Uncomment the following line when you're ready to run getPosts
// const posts = getPosts(searchObject, sortObject, limit, skip)
// console.log(posts)


//  2. Add code in createPost so that a new blog post will be created when createPost is called.
//Note: id, createdAt and lastModified will have to be generated. The id field can be generated with the provided getUUID()
//function which will return a random UUID.
const updatePost = (id, newPostData) => {
db.blogs.updateOne({createdAt}, {lastModified}) // Update this line with your code
}

const updatedPost = {
title: "The Dark Knight Movie Review",
text: "This movie was amazing because I am Batman, and totally not Bruce Wayne. I don't even know who that is.",
author: "Batman",
categories: ["superhero", "action", "thriller"]
}
const postId = "getUUID" // This variable should be the uuid of the blog post you created before using createPost

//Uncomment the following line when you're ready to run updatePost
updatePost(postId, updatedPost)/


//  3. Add code in updatePost so that Mongo will find the post created before using createPost and update it to the new data
// in updatedPost.
// Note: You will need to change the postId variable to be the UUID given to the blog post you created before using createPost().

const deletePost = (id) => {
// Your code here ...
}

const postIdToDelete = ""

// Uncomment the following line when you're ready to run deletePost
// deletePost(postIdToDelete)


// 4. Add code in deletePost so that it will find a post by the given id and delete it.
db.BlogsDB.deleteOne({
    id:"c2d455d4-a0ff-4a07-8e04-098371240003"
})

//*****************END OF CODE**************************
