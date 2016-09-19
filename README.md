## Install

	cd ~/Desktop/openFrameworks
	git clone https://github.com/reginaflores/AlgoSims2016_students.git
	cd AlgoSims2016_students
	git pull && git submodule init && git submodule update && git submodule status
	git submodule foreach git checkout master
	git submodule foreach git pull
	
Note to teacher (not for student use):

	git submodule add https://github.com/casta828/casta828_bootcamp_code
	cat .gitmodules
	git diff --cached —submodule
	git commit -am 'added module’
	git add *
	git push -u origin master

## Use

Every time you want to update all the repos, just do:

	git submodule foreach git pull

And check the projects of other students.

### NOTES FOR YOUR HOMEWORK REPO

* Your homework repo should be inside ```openFrameworks/app``` folder. Inside to maintain the “3 levels down rule“ your homework should be all in the same folder. NO SUBFOLDERS. You can organize it by ```[WEEK_NUMBER]_[HOMEWORK_NUMBER]_[NAME]```. For Example:

```
	openFrameworks/
		addons/
		app/
			[your_NID]_AlgoSims2016/
				w01_h01_blabla/
				w01_h02_blabla/
				w02_h01_blabla/ 
				w03_h01_blabla/ 
				…/
				…/
		libs/
		examples/
		AlgoSims2016/
		AlgoSims2016_students/
 ```

* Remember to add a [```.gitignore```](https://gist.github.com/ofZach/3707086). This will tells git to avoid certain files, such as compiled object code, .app / .exes, etc. It keeps your repos slim and lightweight and helps you avoid committing unnecessary things. (Beside [Zach’s gitignore](https://gist.github.com/ofZach/3707086 you can make your using [this site](http://www.gitignore.io/) ). Also you can use the one from the sims repo. For example, inside your private homework folder do:

	cp ../../sims2014/.gitignore .


