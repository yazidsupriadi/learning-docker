Go to Docker Hub and log in if you need to.

Click the Create Repository button.

For the repo name, use getting-started. Make sure the Visibility is Public.

Click the Create button!

## Pushing our image

### Login to Docker Hub with
    docker login -u YOUR-USER-NAME
    
### Use the docker tag command to give the getting-started image a new name. Be sure to swap out YOUR-USER-NAME with your Docker ID
    docker tag getting-started YOUR-USER-NAME/getting-started
Now try your push command again. If you're copying the value from Docker Hub, you can drop the tagname portion, as we didn't add a tag to the image name. If you don't specify a tag, Docker will use a tag called latest.

    docker push YOUR-USER-NAME/getting-started
