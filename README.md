OntoSpy
=======

RDFLIb-based Python toolkit for inspecting ontologies on the Semantic Web.


Description
=======

OntoSpy is a lightweight Python library and command line tool for inspecting and visualizing vocabularies encoded using W3C Semantic Web standards (aka ontologies). 

The basic workflow is simple: load a graph by instantiating the ``Graph`` class with a file containing RDFS, OWL or SKOS definitions. You get back an object that lets you interrogate the ontology. That's all!

The same functionalities are accessible also via a handy command line application (`ontospy`). This is an interactive environment (like a repl) that allows to load ontologies from a local repository, interrogate them and cache them so that they can be quickly reloaded for inspection later on. 


Documentation
---------------
http://ontospy.readthedocs.org/en/latest/

See also: https://pypi.python.org/pypi/ontospy



Changelog
---------------
v 1.6.9
- ontospy -r `uri` => loads an interactive session only with that URI
- improved visualizations; markdown exports bug fix


v 1.6.8
- fixed bugs with Python3
- more visualizations outputs (3 columns, markdown)
- turtle lexer for nice printouts of source code 
- ontospy -o option for exporting viz to a file


v 1.6.7
- added support for Python 3.0 (via pull request)


v 1.6.6 
- fixed bug with ontospy.tests.load_local and ontospy.tests.load_remote
- removed 'display' command
- replaced 'download' command with 'import' [file, uri, repo, starter-pack]
- added 'info' command options: ['toplayer', 'parents', 'children', 'ancestors', 'descendants']
- added incremental search by passing a pattern 
- serialize at ontology level now serializes the whole graph


v.1.6.5.6
- made the caching functionality version-dependent 
- added 'download' command
- json serialization (via rdflib-jsonld)
- added *bootstrap* command for empty repos
 

v.1.6.5.5
- added 'visualize' command
- added delete, rename, shell commands 