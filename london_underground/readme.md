

# LONDON MULTIPLEX TRANSPORTATION NETWORK

    coordinates = []
    with open('london_transport_nodes.txt', 'r') as fd:
        lines = fd.readlines()
        for line in lines:
            x = line.split(' ')[2]
            y = line.split(' ')[3][:-1]
            coords = tuple((float(x), float(y)))
            coordinates.append(coords)

I'm copying and pasting the below readme from the original dataset. I'm omitting parts that aren't relevant to your network. 

Your metadata for this network is a list of station names. You can upload the station names by typing

    Names = []
    with open('london_underground_names.txt', 'r') as fd:
    lines = fd.readlines()
    for line in lines:
        name = line.split('\n')[0]
        Names.append(name)
	
I also have metadata indicating the geographical coordinates of each node in the network. It's optional, but let me know if you want these and I can send them-- we'll figure out how to make a pretty plot with them!
###### Last update: 1 July 2014

### Reference and Acknowledgments

This README file accompanies the dataset representing the multiplex transportation network of London (UK). 
If you use this dataset in your work either for analysis or for visualization, you should acknowledge/cite the following paper:

	“Navigability of interconnected networks under random failures”
	Manlio De Domenico, Albert Solé-Ribalta, Sergio Gómez, and Alex Arenas
	PNAS 2014 111 (23) 8351-8356

that can be found at the following URL:

<http://www.pnas.org/content/111/23/8351.abstract>

This work has been supported by European Commission FET-Proactive project PLEXMATH (Grant No. 317614), the European project devoted to the investigation of multi-level complex systems and has been developed at the Alephsys Lab. 

Visit

PLEXMATH: <http://www.plexmath.eu/>

ALEPHSYS: <http://deim.urv.cat/~alephsys/>

for further details.



### Description of the dataset

Data was collected in 2013 from the official website of Transport for London (<https://www.tfl.gov.uk/>) and manually cross-checked.

### License

This LONDON MULTIPLEX TRANSPORTATION NETWORK DATASET is made available under the Open Database License: <http://opendatacommons.org/licenses/odbl/1.0/>. Any rights in individual contents of the database are licensed under the Database Contents License: <http://opendatacommons.org/licenses/dbcl/1.0/>

You should find a copy of the above licenses accompanying this dataset. If it is not the case, please contact us (see below).

A friendly summary of this license can be found here:

<http://opendatacommons.org/licenses/odbl/summary/>

and is reported in the following.

======================================================
ODC Open Database License (ODbL) Summary

This is a human-readable summary of the ODbL 1.0 license. Please see the disclaimer below.

You are free:

*    To Share: To copy, distribute and use the database.
*    To Create: To produce works from the database.
*    To Adapt: To modify, transform and build upon the database.

As long as you:
    
*	Attribute: You must attribute any public use of the database, or works produced from the database, in the manner specified in the ODbL. For any use or redistribution of the database, or works produced from it, you must make clear to others the license of the database and keep intact any notices on the original database.
    
*	Share-Alike: If you publicly use any adapted version of this database, or works produced from an adapted database, you must also offer that adapted database under the ODbL.
    
*	Keep open: If you redistribute the database, or an adapted version of it, then you may use technological measures that restrict the work (such as DRM) as long as you also redistribute a version without such measures.

======================================================


### Contacts

If you find any error in the dataset or you have questions, please contact

	Manlio De Domenico
	Universitat Rovira i Virgili 
	Tarragona (Spain)

email: <manlio.dedomenico@urv.cat>

web: <http://deim.urv.cat/~manlio.dedomenico/>
