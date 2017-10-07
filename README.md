Elliot Weiser
=============

Email | GitHub | LinkedIn
----- | ------ | --------
elliot.weiser@gmail.com | [https://github.com/elliotweiser](https://github.com/elliotweiser) | [https://www.linkedin.com/in/elliotweiser/](https://www.linkedin.com/in/elliotweiser/)

Education
---------

* Bachelor of Arts from Swarthmore College '17
  * Major: Computer Science
  * Minor: Mathematics

Open Source Work (on GitHub)
----------------------------

Authored:
* [elliotweiser/ansible-osx-command-line-tools](https://github.com/elliotweiser/ansible-osx-command-line-tools)
* [Comcast/ansible-sdkman](https://github.com/Comcast/ansible-sdkman)

Contributed:
* [geerlingguy/ansible-role-homebrew](https://github.com/geerlingguy/ansible-role-homebrew)
* [metacloud/molecule](https://github.com/metacloud/molecule)
* [aelsabbahy/goss](https://github.com/aelsabbahy/goss)

Public Talks
------------

* [Ansible for MacOS @ MacAdmins Jan 2017](https://apple.lib.utah.edu/jan-2017-mac-managers-meeting/)
* [Automating MacOS VM Creation @ MacAdmins Feb 2017](https://apple.lib.utah.edu/feb-2017-mac-managers-meeting/)

Certifications
--------------
* [Jenkins Engineer](https://certificates.cloudbees.com/10297911)

Work Experience
===============

Comcast NBC Universal (June 2014 - Present Day)
-----------------------------------------------

I joined Comcast as a junior engineer after graduating from Swarthmore College.
My initial core responsibilities included system administration and operation
of Anthill Pro (a legacy CI system), Gerrit Code Review, and Sonatype Nexus.
In the following months, I gradually applied my software development skills to
this role and began practicing "DevOps". As time passed, my team established its
charter: Empower engineers to go fast!

I've since moved up in the ranks. I help motivate my team to do the best work
they can do, while encouraging a fun, collaborative atmosphere. We observe
strict code review guidelines, automate any repeatable task, and test
EVERYTHING. We encourage and remind each other to care about the quality of the
code we write (and that also applies to documentation). We use the AGILE
methodology to manage our workload and to facilitate communication of our
priorities/roadmap to our stakeholders. Our customers are other Comcast
engineers, so we've built strong collaborative relationships with other teams.
This establishes a feedback loop for transparent testing and delivery of
high-demand features to our own software.

Below I describe some of the projects I've worked on while at Comcast.

#### Project Mortar

I collaborated with my team to develop and release a CD-as-a-service platform
for empowering Comcast engineers, based on Jenkins. It was designed to be secure
and easy to use. It integrated with GitHub and used a declarative YAML
specification to describe the entire CD pipeline (similar to Travis CI). This
was the manifestation of our team's charter to empower engineers. Below are
some of the relevant components and features I worked on.

* Groovy scripts for configuring the Jenkins master
* Curating mkdocs-style user onboarding documentation
* Asymmetrically encrypted repository secrets as Jenkins Masked Passwords
* Development of a Job-DSL seed job for generating other Jenkins jobs
* Optimized agent scheduling and build-time caching with Docker and Jenkins Swarm
* Waffle (declarative pipeline YAML; see below)

#### Waffle

I authored a Groovy library for translating a declarative YAML specification
into Jenkins Scripted Pipeline DSL. This was a component of Project Mortar,
which aided in its mission to create a simplifed, opionated interface to CD so
that users could spend less time learning Jenkins internals and more time
building and developing software. This has not been open-sourced (yet).

#### CAP Current-Next

This was my first project at Comcast. I wrote a client library and CLI
(first in Python, then in Ruby) that talked to a service called HighWire, a
RESTful interfact to Brocade load balancers. The goal was to use Blue-Green
(or Current-Next) style deployment to eliminate the risky minutes-to-hours long
deployment window of some of our state-less applications. We successfully
managed to get this down to less than 10 seconds for the projects that opted to
onboard. Though the project was ultimately put on hold, I gained a love for
writing Ruby code, and more importantly, I learned the importance of building
strong, collaborative relationships within my team and across teams.

#### Migrate to the Cloud

I collaborated with my team to design and implement immutable architecture for
our existing service offerings. Using tools like Ansible, Packer, Cloud-Init,
and Terraform, we migrated our services out of VMWare datacenters into
an OpenStack VPC. Testing was performed with Testinfra, and eventually we
converted to Goss. I learned about using service discovery tools like Consul for
health-check monitoring and runtime-configuration management in response to
certain events. We sent system (and sometimes JVM/application) metrics to an
InfluxDB cluster with Telegraf and created Grafana dashboards (which was so much
fun!). Overall, this undertaking was laborious and sometimes painful, but it was
also extremely rewarding.

Skills
------

#### Source Control

Git is my go-to. I've used both GitHub and Gerrit extensively, so I'm proficient
in both the fork/PR workflow and the Gerrit cherry-picking workflow, but I've
also worked with other merging and rebasing workflows. I also GPG-sign my
commits and tags. In my role as a Gerrit administrator, I've also taught Git to
new users, which required a thorough understanding of the internals of Git's
object and reference database. I've assisted with Git migrations and managing
multi-remote configurations.

I've also worked with Subversion, Team Foundation Server, and Visual SourceSafe,
but I don't like using them.

#### Infrastructure and Configuration as Code

I have substantial experience writing code for/using the tools enumerated below.
Most of this experience targed an OpenStack-based cloud environment, but some
has targeted VMWare and bare metal, on both Linux and Mac OS systems.

Configuration Management/Automation:
* Ansible
* Cloud-init

Virtual/Container Image Building:
* Packer
* Docker

Infastructure Life-Cycle Management
* Terraform

Infrastructure testing:
* Testinfra
* Goss

Metrics Gathering, Dashboards, and Alerting:
* Telegraf
* InfluxDB (as a client user)
* Grafana

Service Discovery and Monitoring
* Consul (as a client user)
* Consul Template

#### Programming Languages

Below are the programming languages with which I have extensive experience:

Ruby:
* Writing specification-based unit tests w/ RSpec
* Mutation-based test coverage checking (ask me about it!)
* Static analysis w/ the MetricFu toolbox
* Scripting for System Administration

Groovy:
* Specification-based testing w/ Spock
* Code coverage w/ Cobertura and Jacoco
* GMetrics for analyzing cyclomatic/ABC complexity
* Scripting against the Jenkins Script Console for configuration and maintenance
* Jenkins Scripted Pipeline DSL (ask me about it!)
* Jenkins Job DSL (ask me about it!)

Python:
* I've used py.test and nosetests for writing unit tests
* I've used coverage.py for code coverage checking
* Scripting for System Administration

Bash:
* Scripting for System Administration on UNIX-based systems

I've also contributed small code changes to Java, Golang, and NodeJS projects.
My go-to language in college was C++, but it's been a while.

#### System Administration

I won't say too much about this. Most of the system administration skills I
learned were incidental to my other responsibilities. Sometimes I needed to
reconfigure SSHD, manage user accounts, or troubleshoot network connectivity
with `traceroute` and `nc`. I wrote various Bash scripts which used some fun
GNU tools like `find`, `sed`, and `awk`. I mostly administered Linux systems,
specifically CentOS 6 and 7, but I also managed a cluster of Mac Minis
responible for building iOS applications.

Things I'm excited to learn more about
--------------------------------------

* Programming in Golang and NodeJS
* Container orchestration w/ Kubernetes, OpenShift, DC OS, Mesosphere, etc.

Useless Trivia
--------------

* I rescued, nursed, and adopted an abandoned baby kitten. He's my programming buddy.
* I enjoy talking astrophysics, internet memes, and describing algorithms with Big-O notation.
