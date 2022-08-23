Info:
=============

Gitbackup is a utils for make backup of all gitlab repositorien of user.

Build:
=============
<pre>
git clone {repo url}
cd {project folder}
gradle build
</pre>
or with docker
<pre>
docker run --rm -u gradle -v "$PWD":/home/gradle/project -w /home/gradle/project gradle gradle build --warning-mode all
</pre>
<pre>
build result location is "./build/lisb/gitbackup.jar"
</pre>
Help:
=============
<pre>
usage: gitbackup
 -f,--folder <arg>     folder for save repositories
 -l,--login <arg>      user login
 -p,--password <arg>   user password
 -u,--url <arg>        url of gitlab server
</pre>
Run:
=============
<pre>
java -jar ./gitbackup.jar -f ./folder -l user -p password -u https://gitlab.com
</pre>
