# xitudatang
hebiye
from rdflib import Graph
import rdflib
g = rdflib.Graph()
g.parse("di1030.ttl",format="ttl")
qres = g.query(
    """SELECT   ?a   ?c
       WHERE {
          ?a ex:editorUna ?c .
       }order by desc (?c)  """)
for row in qres:
    print("%s ex:editorUna %s" % row )
