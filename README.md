## docs-site-template

This is a project template for documents generator. It is using [Apache Maven Site Plugin](http://maven.apache.org/plugins-archives/maven-site-plugin-3.3/)
to generate a project document site. The site can be configured with a simple [site.xml](http://maven.apache.org/plugins-archives/maven-site-plugin-3.3/examples/sitedescriptor.html)
configuration. The document can be written in [markdown](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet) syntax.
The site plugin is using [Apache Maven Fluido Skin](https://maven.apache.org/skins/maven-fluido-skin/) built on top of [Twitter's Bootstrap 2.2.2]
(http://bootstrapdocs.com/v2.2.2/docs/) web front end framework. [Click here](http://piyapongch.github.io/docs-site-template) to see a sample site.


### System Requirements

* Java 6 <http://www.oracle.com/technetwork/java/javase/overview/index.html>
* Apache Maven 3 <http://maven.apache.org/>
* Git <http://git-scm.com/>

### Usage

#### Generate project documents 

* create branch gh-pages on your project repository
* clone gh-pages branch
```shell
$ git clone -b gh-pages https://github.com/${username}/${project.name}.git ${project.docs.dir}
```

* clone docs-site-template project
```shell
$ git clone https://github.com/${username}/docs-site-template.git ${docs.site.template.dir}
```

* change directory and edit your documents
```shell
$ cd ${docs.site.template.dir}
```

* generate project documents
```
$ mvn site -Dsite.output.dir=${project.docs.dir}
```

* change directory to ${project.docs.dir}
```
$ cd ${project.docs.dir}
```

* commit and push to gh-pages branch
```
$ git add .
$ git commit -m "Update project documents"
$ git push
```

#### View project documents

* Point your browser to https://${username}.github.io/${project.name}









