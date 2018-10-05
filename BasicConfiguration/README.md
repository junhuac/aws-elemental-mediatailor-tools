If you've never created an AWS Elemental MediaTailor configuration before, it is worthwhile to follow [this tutorial](https://github.com/aws-samples/aws-media-services-simple-live-workflow/tree/master/5-MediaTailor). It walks you through setting up MediaTailor in the context of a live video streaming workflow.

Creating a configuration has been automated here using this [template](../CloudFormation/BasicConfiguration). 

On its own, the template is not a big time saver as compared to creating a configuration manually via the MediaTailor console. However, it can be used (with some edits) in conjunction with other templates to automate a more involved workflow. One example would be a workflow that creates an AWS Elemental MediaLive channel that pushes to AWS Elemental MediaPackage, then a MediaTailor configuration using the MediaPackage channel as a video source.