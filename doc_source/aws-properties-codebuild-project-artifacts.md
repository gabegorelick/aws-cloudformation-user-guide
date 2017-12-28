# AWS CodeBuild Project Artifacts<a name="aws-properties-codebuild-project-artifacts"></a>

`Artifacts` is a property of the [AWS::CodeBuild::Project](aws-resource-codebuild-project.md) resource that specifies output settings for artifacts generated by an AWS CodeBuild build\.

## Syntax<a name="aws-properties-codebuild-project-artifacts-syntax"></a>

To declare this entity in your AWS CloudFormation template, use the following syntax:

### JSON<a name="aws-properties-codebuild-project-artifacts-syntax.json"></a>

```
{
  "[[ERROR] BAD/MISSING LINK TEXT](#cfn-codebuild-project-artifacts-location)" : String,
  "[[ERROR] BAD/MISSING LINK TEXT](#cfn-codebuild-project-artifacts-name)" : String,
  "[[ERROR] BAD/MISSING LINK TEXT](#cfn-codebuild-project-artifacts-namespacetype)" : String,
  "[[ERROR] BAD/MISSING LINK TEXT](#cfn-codebuild-project-artifacts-packaging)" : String,
  "[[ERROR] BAD/MISSING LINK TEXT](#cfn-codebuild-project-artifacts-path)" : String,
  "[[ERROR] BAD/MISSING LINK TEXT](#cfn-codebuild-project-artifacts-type)" : String
}
```

### YAML<a name="aws-properties-codebuild-project-artifacts-syntax.yaml"></a>

```
[[ERROR] BAD/MISSING LINK TEXT](#cfn-codebuild-project-artifacts-location): String
[[ERROR] BAD/MISSING LINK TEXT](#cfn-codebuild-project-artifacts-name): String
[[ERROR] BAD/MISSING LINK TEXT](#cfn-codebuild-project-artifacts-namespacetype): String
[[ERROR] BAD/MISSING LINK TEXT](#cfn-codebuild-project-artifacts-packaging): String
[[ERROR] BAD/MISSING LINK TEXT](#cfn-codebuild-project-artifacts-path): String
[[ERROR] BAD/MISSING LINK TEXT](#cfn-codebuild-project-artifacts-type): String
```

## Properties<a name="w3ab2c21c14d291b7"></a>

`Location`  
The location where AWS CodeBuild saves the build output artifacts\. For valid values, see the [http://docs.aws.amazon.com/codebuild/latest/userguide/create-project.html#create-project-cli](http://docs.aws.amazon.com/codebuild/latest/userguide/create-project.html#create-project-cli) field in the *AWS CodeBuild User Guide*\.  
*Required: *Conditional\. If you specify `CODEPIPELINE` or `NO_ARTIFACTS` for the `Type` property, don't specify this property\. For all of the other types, you must specify this property\.  
*Type*: String

`Name`  
The name of the build output folder where AWS CodeBuild saves the build output artifacts\. For \.zip packages, the name of the build output \.zip file that contains the build output artifacts\.  
*Required: *Conditional\. If you specify `CODEPIPELINE` or `NO_ARTIFACTS` for the `Type` property, don't specify this property\. For all of the other types, you must specify this property\.  
*Type*: String

`NamespaceType`  
The information AWS CodeBuild adds to the build output path, such as a build ID\. For more information, see the [http://docs.aws.amazon.com/codebuild/latest/userguide/create-project.html#create-project-cli](http://docs.aws.amazon.com/codebuild/latest/userguide/create-project.html#create-project-cli) field in the *AWS CodeBuild User Guide*\.  
*Required: *No  
*Type*: String

`Packaging`  
Indicates how AWS CodeBuild packages the build output artifacts\. For valid values, see the [http://docs.aws.amazon.com/codebuild/latest/userguide/create-project.html#create-project-cli](http://docs.aws.amazon.com/codebuild/latest/userguide/create-project.html#create-project-cli) field in the *AWS CodeBuild User Guide*\.  
*Required: *No  
*Type*: String

`Path`  
The path to the build output folder where AWS CodeBuild saves the build output artifacts\.  
*Required: *No  
*Type*: String

`Type`  
The type of build output artifact\. For valid values, see the [http://docs.aws.amazon.com/codebuild/latest/userguide/create-project.html#create-project-cli](http://docs.aws.amazon.com/codebuild/latest/userguide/create-project.html#create-project-cli) field in the *AWS CodeBuild User Guide*\.  
*Required: *Yes  
*Type*: String