# BlogApi

This blog api server is a part of the EdX tutorial on NodeJs.

The APIs are built using Express Server

The format of the blog posts and the comments is as below

```
[{
  name: "Post 1",
  url: "Blog url",
  text: "Blog text",
  comments: [{
    text: "Comment1"
  },{
    text: "Comment2"
  }]
},{
  name: "Post 2",
  url: "Blog url",
  text: "Blog text",
  comments: [{
    text: "Comment1"
  },{
    text: "Comment2"
  }]

} ... ]
```

The available APIs in the server are

For Blog Posts
- GET    => /posts
- GET    => /posts/{:postId}
- POST   => /posts
- PATCH  => /posts/{:postId}
- DELETE => /posts/{:postId}

For comments
- GET    => /posts/{:postId}/comments
- GET    => /posts/{:postId}/comments/{:commentId}
- POST   => /posts/{:postId}/comments
- PATCH  => /posts/{:postId}/comments/{:commentId}
- DELETE => /posts/{:postId}/comments/{:commentId}

