Heavily experimental, want to see what will happen if a Rails style code generator existed for Erlang web projects. Expect this to either be abandoned or to shift direction.

prerequisites:

requires rebar to be installed on your system. If you use a mac I suggest homebrew

	 brew install rebar

see https://github.com/basho/rebar for more options.

installation:

	git clone git://github.com/chrisduesing/wherl.git

setup:
	
	rebar get-deps
	
	rebar compile

usage: 

create a new application
	
	wherl new <application name>

create a new model

	wherl generate model <name> <attribute1> <attribute2> <etc.>

create a new controller

	wherl generate controller <name>

create a model and controller together (coming soon)

       wherl generate scaffold <name> <attribute1> <attribute2> <etc.>