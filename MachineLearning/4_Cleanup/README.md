# Cleanup Instructions

**If you're running this inside of an Event Engine environment, you can stop reading.**

1. Navigate to your Cloud9 environment
1. Run the following commands to delete your resources:
    ```
    # The inference resources from module 3
    aws cloudformation delete-stack --stack-name wildrydes-ml-mod3-4
    # The machine learning resources from module 2
    aws cloudformation delete-stack --stack-name wildrydes-ml-mod2-3
    # The Glue resources from module 2
    aws cloudformation delete-stack --stack-name wildrydes-ml-mod2-2
    # The data processing resources from module 1
    aws cloudformation delete-stack --stack-name wildrydes-ml-mod1-1
    # Delete all objects from your bucket
    aws s3 rm s3://YOUR_BUCKET_NAME --recursive
    # Delete your bucket
    aws s3 rb s3://YOUR_BUCKET_NAME
    ```
1. Exit your Cloud9 environment
1. Select the environment you've been using
1. Click **Delete**
1. Follow the directions

**CONGRATS!** You're done!
