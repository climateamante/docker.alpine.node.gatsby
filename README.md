# ![](http://images1-focus-opensocial.googleusercontent.com/gadgets/proxy?container=focus&gadget=a&no_expand=0&resize_w=30&rewriteMime=image/*&url=https://user-images.githubusercontent.com/29623356/59837660-772a7680-9302-11e9-8b67-fe556597eb3b.png)  Docker Template For [Gatsby](https://github.com/gatsbyjs/gatsby) ![](http://images1-focus-opensocial.googleusercontent.com/gadgets/proxy?container=focus&gadget=a&no_expand=0&resize_w=30&rewriteMime=image/*&url=https://user-images.githubusercontent.com/29623356/60942388-4c936400-a297-11e9-97b3-5ce7921baa9b.png)  
 >  Example: Get up and running with the [SendGrid Documentation](https://github.com/sendgrid/docs) 

### I've pulled the Docker image, now what?

1. Create an `app` folder for your local working directory
> helpful for saving files locally once the container is stoped

2. Start an instance of the image
```sh
    docker run \
    -v $PWD/app:/var/www/app \
    -p 80:8000 \
    --name alpine.node.gatsby.dev \
    -it --rm climateamante/alpine.node.gatsby:latest /bin/ash
```

3. Fork or clone The [SendGrid Documentation](https://github.com/sendgrid/docs) Gatsby into the `app` folder after creating an instance of the image.

4. Start the develop process.
 - `gatsby develop -H 0.0.0.0`
 - The Docker instance has mapped Gatsby from port `8000` is now mapped to the `localhost:80`

5. Start local development and contributing to open-source documentation!