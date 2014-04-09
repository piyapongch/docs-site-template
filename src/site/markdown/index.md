## Welcome to docs-site-template

This is a project template for documents generator. It is using [Apache Maven Site Plugin](http://maven.apache.org/plugins-archives/maven-site-plugin-3.3/)
to generate a project document site. The site can be configured with a simple [site.xml](http://maven.apache.org/plugins-archives/maven-site-plugin-3.3/examples/sitedescriptor.html)
configuration. The document can be written in [markdown](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet) syntax.
The site plugin is using [Apache Maven Fluido Skin](https://maven.apache.org/skins/maven-fluido-skin/) built on top of (Twitter's Bootstrap 2.2.2)
(http://bootstrapdocs.com/v2.2.2/docs/) web front end framework. [Click here](http://ualbertalib.github.io/docs-site-template) to see a sample site.


### System Requirements

* Java 6 <http://www.oracle.com/technetwork/java/javase/overview/index.html>
* Apache Maven 3 <http://maven.apache.org/>
* Git <http://git-scm.com/>

### Usage

#### Generate project documents 


```shell
# clone template project
$ git clone https://github.com/ualbertalib/docs-site-template.git

# change directory and edit your documents
$ cd docs-site-template

# generate project documents
$ mvn site -Dsite.output.dir=${site.output.dir}

# initailize git repository for project documents branch
$ cd ${site.output.dir}
$ git init
$ git remote add gh-pages ${your.git.project.url}

# commit and push to gh-pages branch
$ git commit -m "Update project documents"
$ git push
```

#### View project documents

* Point your browser to https://ualbertalib.github.io/docs-site-template
