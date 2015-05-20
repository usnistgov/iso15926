* EDRC Use Case 2 AppendixE–SampleData.ttl

Sample extracted from EDRC Use Case 1 Appendix E.

*EDRC Use Case 2 TechInvestLab Demo
Victor Agroskin
TechInvestLab

Step-by-step guide for UC2 demo together with pattern files used in the mapping can be downloaded 
from http://techinvestlab.ru/EDRCDemo

UC2 project data files were built using mapping to patterns, and these patterns can be easily transformed 
into test queries. For example, a test that pressure property is always used for a stream object contained
in the instrument and is never used for an instrument itself. Or a test for object declaration presence. 

iso15926.fiatech.org/edrc_usecase_2 
the files described below are a copy of the TechInvestLab Demo with no semantic change. 
Some OWL import statements were added and the same template file source as for EDRC Use Case 1 was used.

* pressure_transmitter_rfq_1.ttl and pressure_transmitter_rfq_1_reply.ttl
RFQ information for one pressure transmitter and a reply to it

* pressure_transmitter_rfq_10.ttl and pressure_transmitter_rfq_10_reply.ttl
RFQ information containing RFQ information for all ten pressure transmitters and a reply to it.

* EDRC_UC2_RDL_Extension.rdf 
Reference data entities required for EDRC UC2 models but not found in PCA RDL. 
Only basic information is provided for new entities.

* Emerson_Catalogue.rdf
Dummy corporate RDL with basic instrument catalogue data (IDs only).