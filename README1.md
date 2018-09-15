# xitudatang
hebiye
from prov.model import ProvDocument
d1 = ProvDocument()
d1.add_namespace('ex', 'http://example.com/')
d1.add_namespace('prov', 'http://www.w3.org/ns/prov#')
# Entity: now:employment-article-v1.html
e1 =d1.entity('ex:revisionitem_172')
h1 =d1.agent('ex:Bob')
y1 =d1.activity('ex:add_revision')

e2 =d1.entity('ex:revisionitem_173')
h2 =d1.agent('ex:Aoa')
y2 =d1.activity('ex:remove_revision')

e3 =d1.entity('ex:revisionitem_174')
h3 =d1.agent('ex:Coc')
y3 =d1.activity('ex:changed_revision')

d1.entity('ex:revisionitem_172')


d1.wasAttributedTo(e1,h1)
d1.wasAttributedTo(e2,h2)
d1.wasAttributedTo(e3,h3)

d1.wasAssociatedWith(y1, h1)
d1.wasAssociatedWith(y2, h2)
d1.wasAssociatedWith(y3, h3)

d1.entity('ex:item')

d1.wasDerivedFrom(e1, e1)
d1.wasDerivedFrom(e2, e2)
d1.wasDerivedFrom(e3, e3)


d1.used(y2,e1)
d1.used(y3,e2)


d1.wasGeneratedBy(e1,y2)
d1.wasGeneratedBy(e2,y3)

d1.get_provn()

d1.serialize("di5.ttl",format="rdf",rdf_format="ttl")
print(d1.get_provn())
