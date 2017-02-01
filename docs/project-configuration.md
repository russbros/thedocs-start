# Project configuration
Basically you need to configure two things:
* How to checkout a project
* Who can access the project

## How to checkout a project
You've got following checkout options:
* Remote URL - GIT url. Please use SSH styled urls (don't use `https://` urls).
* Branch - GIT branch. Leave empty to use `master` branch.
* Documents directory - this directory will be used as the root for docs. Leave empty to use root directory.
This option is useful when you mix sources and docs in the same repository.
* Files filter extensions - we will filter all files except if the extension is not in the list.
By default `jpg`, `png`. Set as empty to not filter files at all.

In addition to this options you have to configure your git repository:
* You have to provide access to theDocs.io
* You have to configure git hook on every push. In this case we will rebuild index on each push.

## Who can access the project
You've got following access options:
* Visibility - public / private - public projects visible for everybody,
private projects visible for the owner and members of manage/read teams
* Manage access teams - these members can change project settings, and get access to read what is on the project
* Read access teams - members of these teams are able to read project documents
