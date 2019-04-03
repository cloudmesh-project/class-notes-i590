**Simplest Chef Tutorial:**

**[Instruction: Command: ]{.underline}**

Prerequisites (distribution specific):

Install git, curl, rubygem-chef

Go to home directory:

> cd \$HOME

Login as root:

su \<or\> sudo su

Get Apache Bigtop repository (exact command is distribution
specific-listed is Ubuntu):

> wget --O-
> http://www.apache.org/dist/bigtop/bigtop-0.7.0/repos/GPG-KEY-bigtop \|
> apt-key add --
>
> wget -O /etc/apt/sources.list.d/bigtop.list
> [http://www.apache.org/dist
> /bigtop/bigtop-0.7.0/repos/quantal/bigtop.list](http://www.apache.org/dist%20/bigtop/bigtop-0.7.0/repos/quantal/bigtop.list)
>
> apt-get update

Use curl to install Chef:

> curl -L https://www.opscode.com/chef/install.sh \| bash

Use git to retrieve files for example:

> git clone git://github.com/smccaula/SimpleChef.git

Go to tutorial directory:

> cd ./SimpleChef

Edit directories in solo.rb to reflect user home:

nano solo.rb

Run Chef solo to install software:

> chef-solo -c solo.rb -j install.json

\*\*\* see recipes in ./SimpleChef/cookbooks/simple/recipes to install
different packages \*\*\*
