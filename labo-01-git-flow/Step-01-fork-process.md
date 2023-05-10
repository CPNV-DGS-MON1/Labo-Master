# Fork process

[Source](https://docs.github.com/en/get-started/quickstart/fork-a-repo)

<figure><img src="../../.gitbook/assets/image (4).png" alt=""><figcaption><p>Git-flow scenario to master</p></figcaption></figure>

* [x] Fork the "upstream" repository in your github organisation

```
//TODO
Screenshot of Github
```

![image-20230509112128829](assets/image-20230509112128829.png)

* [ ] Clone "teacher" repo in your local machine

```
[INPUT]
git clone https://github.com/AlmirRazic/LABO-MASTER.git

[OUTPUT]
Cloning into 'Labo-Master'...
remote: Enumerating objects: 12, done.
remote: Counting objects: 100% (12/12), done.
remote: Compressing objects: 100% (11/11), done.
remote: Total 12 (delta 0), reused 12 (delta 0), pack-reused 0
Receiving objects: 100% (12/12), 4.28 KiB | 547.00 KiB/s, done.
```

* [ ] Init Git flow (with standard settings)

```
[INPUT]
git flow init

[OUTPUT]
No branches exist yet. Base branches must be created now.
Branch name for production releases: [master]
Branch name for "next release" development: [develop]
Author identity unknown

*** Please tell me who you are.

Run

  git config --global user.email "you@example.com"
  git config --global user.name "Your Name"

to set your account's default identity.
Omit --global to set the identity only in this repository.

fatal: unable to auto-detect email address (got 'Almir@DESKTOP-LEVK5OI.(none)')
fatal: not a valid object name: 'master'
error: pathspec 'develop' did not match any file(s) known to git
Fatal: Could not check out branch 'develop'.

2nd[OUTPUT]
git flow init
No branches exist yet. Base branches must be created now.
Branch name for production releases: [master]
Branch name for "next release" development: [develop]

How to name your supporting branch prefixes?
Feature branches? [feature/]
Bugfix branches? [bugfix/]
Release branches? [release/]
Hotfix branches? [hotfix/]
Support branches? [support/]
Version tag prefix? []
Hooks and filters directory? [D:/GIT/.git/hooks]
```

* [ ] Update your develop branch directly to the upstream (main branch)

```
[INPUT]
git remote add upstream https://github.com/CPNV-MON1/Labo-Master.git
git remote -v

[OUTPUT]
origin  https://github.com/AlmirRazic/Labo-Master (fetch)
origin  https://github.com/AlmirRazic/Labo-Master (push)
upstream        https://github.com/CPNV-MON1/Labo-Master.git (fetch)
upstream        https://github.com/CPNV-MON1/Labo-Master.git (push)
```

* [ ] Create a branch feature called "feat:add terraform basic  script"

```
[INPUT]
//TODO

[OUTPUT]
//TODO
```

* [ ] Add this code and commit it

```
terraform {
  required_providers {
    aws = {
      source  = "hashicorp/aws"
      version = "~> 4.16"
    }
  }

  required_version = ">= 1.2.0"
}

provider "aws" {
  region  = "us-west-2"
}

resource "aws_instance" "app_server" {
  ami           = "ami-830c94e3"
  instance_type = "t2.micro"

  tags = {
    Name = "ExampleAppServerInstance"
  }
}
```

```
[INPUT]
//TODO

[OUTPUT]
//TODO
```

* [ ] Finish the feature

```
[INPUT]
//TODO

[OUTPUT]
//TODO
```

* Push this modification on your repository

```
[INPUT]
//TODO

[OUTPUT]
//TODO
```

* What happens to the feature/branch ?

```
//TODO
Add your answer with command line used to validate your analysis.
```

* Open a pull request comparing your develop branch to your main
* Assign the pull request to your partner

```
//TODO
Screenshot pull request on github
```

* Notify him using a issue "Could you please review my pull request ?"

```
//TODO
Screenshot issue on github
```

