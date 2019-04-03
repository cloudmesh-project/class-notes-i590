Opscode Chef

Functional Area: Cluster Resource Management

Overview:

Chef is a tool for configuring and managing systems and cluster
environments. It can be used to maintain physical computing
environments, and can also work with cloud platforms such as OpenStack,
Amazon EC2 and Microsoft Azure. Chef is available from the company
formerly known as Opscode (now simply called Chef) in either Enterprise
or Open Source versions. Either version supports a client/server mode as
well as a local chef-solo mode. While not an Apache Foundation project
like many of the other packages included here, it is open source and is
covered by the Apache license model.

The Chef client software is written in Ruby, and configuration
instructions to support a user's environment are also written as Ruby
scripts, in this case called "recipes". These recipes define the desired
system configuration, and by running them Chef configures the
environment and software as requested. One key feature of Chef is
referred to by its developers as "idempotence", which simply means a
script will produce an identical environment regardless of how many
times it is run. In other words, it will not break if told to install
something already installed.
