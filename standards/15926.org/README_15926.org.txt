* 15926.org template modifications to fit into this project

1) Download XML from : http://15926.org/15926_template_specs.php?sid=acd7e991665e5f59001196071f27fe05&mode=owl

The URI of the "data model" must be changed to work with this project.

Edit the file replacing all uses of : http://standards.iso.org/iso/15926/dm

with this : http://rds.posccaesar.org/2008/02/OWL/ISO-15926-2_2003 (which is dereferenceable).

making sure the dm prefix is set to the changed URI too. The ISO-15926-2_2003 URI is the one that is used as the basis for
the PCA RDL library (if you download from PCA that's what you get). 

As understood at the time of this project, the intent of the EDRC and MMT teams is to use that
ontology as the data model for exchange, but it is unclear why a different URI is used for that ontology as the real
one is dereferenceable and the modified one is not.

Note that in the official 15926-8 (see http://www.iso.org/iso/home/store/catalogue_tc/catalogue_detail.htm?csnumber=52456)
there is a different "data model" OWL ontology, but the EDRC and MMT team decided not
to use that as part of their base specification for template-based exchange.

2) The base namespace when downloaded is : http://15926.org/templates-test/templates
but the base for the templates used in this project is : http://data.posccaesar.org/tpl/

To repair this replace the use of : http://15926.org/templates-test/templates#

with : http://data.posccaesar.org/tpl/

in the URIs of all templates. For example this : http://15926.org/templates-test/templates#AssemblyOfAnIndividual

would become this : http://data.posccaesar.org/tpl/AssemblyOfAnIndividual

3) The graph name of the downloaded templates is : http://15926.org/templates-test/templates
but the test cases in this project use : http://data.posccaesar.org/tpl/

To repair this either also change the graph name in the downloaded template RDF
from : http://15926.org/templates-test/templates
to : http://data.posccaesar.org/tpl/
or change the OWL imports in all test case exchange files to use  : http://15926.org/templates-test/templates

to manage versions of templates is it accepted practice to use graph names that are different from the
base of the classed and properties defined in the graph. It is unclear if that is the approach being used
in 15926.org templates.