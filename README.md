Elliot Weiser
=============

Email | GitHub | LinkedIn
----- | ------ | --------
[elliot.weiser@gmail.com](mailto:elliot.weiser@gmail.com) | [https://github.com/elliotweiser](https://github.com/elliotweiser) | [https://www.linkedin.com/in/elliotweiser/](https://www.linkedin.com/in/elliotweiser/)

Education
---------

* Bachelor of Arts from Swarthmore College '14
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

Software Engineer, Comcast NBC Universal (June 2014 - Present Day)
------------------------------------------------------------------

I joined Comcast as a junior engineer after graduating from Swarthmore College.
Administration of various legacy services was my first responsibility.  Those
systems included Anthill Pro, Gerrit Code Review, and Sonatype Nexus. Each
member of the team led training sessions and contributed to best-practices
documentation.

This was not a glamorous phase of my position, but it presented an opportunity
for growth. A "DevOps" culture arose as my team applied development
methodologies to our work. After some much needed maturation, my team
established its charter. Empower engineers to go fast!

I'm currently a Software Engineer II.  I help motivate my team to do the best
work they can do, while encouraging a fun, collaborative atmosphere. We observe
strict code review guidelines, automate any repeatable task, and test
EVERYTHING. We encourage each other to write high-quality code, commit messages,
and documentation. Our team practices AGILE to help manage our workload. Each
member of the team "manages up" by leading scrums and contributing to our
road-map. Furthermore, we've established healthy, collaborative relationships
with other engineering teams.  These teams help assist with beta testing,
providing feedback, and informing our backlog.

Below I describe some of the projects I’ve worked on while at Comcast.

#### Project Mortar

Our mission was to develop the ideal CD-as-a-service platform to replace Anthill
Pro. Together, we designed and implemented a secure, easy-to-use CD solution
based on Jenkins.  Inspired by Travis CI, it utilizes a declarative YAML syntax
to describe the CD pipelines. This was the primary manifestation of our team’s
charter to empower engineers. Project Mortar continues to provide CI/CD to
hundreds of projects and users across Comcast. Below are some of the relevant
components and features to which I contributed:

* Groovy scripts for configuring the Jenkins master
* Curating mkdocs-style user onboarding documentation
* Asymmetric encryption of repository secrets, exposed as Jenkins Masked Passwords
* Development of a Job-DSL seed job for generating other Jenkins jobs
* Optimized agent scheduling and build-time caching with Docker and Jenkins Swarm
* Waffle (declarative pipeline YAML; see below)

#### Waffle

I authored a Groovy library that translates YAML into Jenkins Scripted Pipeline
DSL. This implemented a declarative, simplified, and opinionated interface to
Jenkins. Furthermore, it prevents users from injecting arbitrary Groovy code
into the Jenkins runtime. In response to similar projects, Jenkins finally
released "Declarative Pipeline" the following year. Unfortunately, Waffle has
not been open-sourced (yet). It remains a key component of Project Mortar.

#### CAP Current-Next

This was my first project at Comcast. I wrote a client library and CLI that
orchestrated blue-green (or current-next) deployment. This tool would
communicate with HighWire, a RESTful interface to Brocade load balancers. The
goal? Reduce the minutes-to-hours long deployment window of some of our
state-less applications. For the projects that opted to onboard, we managed to
shrink this to approximately 10 seconds! With the emergence of tooling like
Consul and Docker, we decided to put development on hold. I wasn't discouraged
though-- I gained a love for writing Ruby code. Furthermore, I learned the value
of collaborative relationships that transcends typical team boundaries.

#### Migrate to the Cloud

We migrated our services out of legacy VMWare datacenters into an OpenStack VPC.
To this end, I collaborated with my team to design and deploy immutable
architecture. We used tools like Ansible, Packer, Cloud-Init, and Terraform to
provision infrastructure. We leveraged Testinfra and Goss to verify desire
machine state. We registered our services with externally-managed Consul and
Influx DB clusters. Telegraf would send metrics to InfluxDB, which we visualized
in Grafana dashboards. We used Consul for service discovery and application
health-checking. This undertaking was laborious, but it was also rewarding.

Skills
======

Source Control
--------------

Git is my go-to. I’ve made extensive use of both GitHub (Enterprise) and Gerrit
Code Review. I’m proficient in both the fork/PR workflow and the Gerrit
cherry-picking workflow. I'm also familiar with other merging/rebasing
workflows. On collaborative projects, I write detailed commit messages. I also
GPG-sign my commits and tags.

As an administrator of Gerrit Code Review, I led Git training sessions. This
demanded a thorough understanding of Git’s internal object/reference database.
I’ve assisted with Git migrations and the management of multi-remote
configurations.

I'm familiar with Subversion, Team Foundation Server, and Visual SourceSafe. I
don't like them.

Infrastructure and Configuration as Code
----------------------------------------

Both at work and home, I authored and contributed to various
infrastructure-as-code projects. At work, we targeted an OpenStack VPC, but some
work targeted VMWare and bare metal, on both Linux and Mac OS systems. These are
the tools I have used for those projects.

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

Programming Languages
---------------------

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

System Administration
---------------------

The systems I administered were a combination of Linux (CentOS 6/7) and Mac OS.
Sometimes I needed to configure services, manage user accounts, or troubleshoot
network connectivity. I wrote various Bash, Python, and Ruby scripts to assist
with these efforts. I'm sure there's something I forgetting here, so I'll come
back to it when I remember.

Things I'm excited to learn more about
--------------------------------------

* Programming in Golang and NodeJS
* Container orchestration w/ Kubernetes, OpenShift, DC OS, Mesosphere, etc.

Useless Trivia
--------------

* I rescued, nursed, and adopted an abandoned, newborn kitten. He's now my programming buddy.
* I enjoy talking astrophysics, internet memes, and describing algorithms with Big-O notation.
