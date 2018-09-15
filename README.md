# xitudatang
hebiye
document
  prefix ex <http://example.com/>
  prefix wd <http://www.wikidata.org/entity/>
  prefix wdt <http://www.wikidata.org/prop/direct/>
  prefix rdfs <http://www.w3.org/2000/01/rdf-schema#>
  prefix skos <http://www.w3.org/2004/02/skos/core#>
  prefix scheme <http://schema.org/description#>
  prefix rdf <http://www.w3.org/1999/02/22-rdf-syntax-ns#>
  
  entity(ex:revisionitem_172, [prov:value="National Taiwan University of Arts", prov:wasQuotedFrom="<https://zh.wikipedia.org/>"])
  agent(ex:Aoa, [prov:type="Person", ex:givenName="Aoa"])
  activity(ex:add_revision, -, -)
  entity(ex:revisionitem_173, [wdt:P31="wd:Q1062083", skos:altLabel="zhoudong", prov:label="Jay Chou[en]"])
  agent(ex:Bob, [prov:type="Person", ex:givenName="Bob"])
  activity(ex:remove_revision, -, -)
  entity(ex:revisionitem_174, [rdf:description="direator"])
  agent(ex:CocBot, [prov:type="softwareAgent", ex:givenName="CocBot"])
  activity(ex:changed_revision, -, -)
  entity(ex:revisionitem_172, [prov:generatedAtTime="2016-12-01T07:57:00"])
  entity(ex:revisionitem_173, [prov:generatedAtTime="2015-12-01T07:57:00"])
  entity(ex:revisionitem_174, [prov:generatedAtTime="2014-12-01T07:57:00"])
  used(ex:add_revision, ex:revisionitem_172, -)
  used(ex:remove_revision, ex:revisionitem_173, -)
  used(ex:changed_revision, ex:revisionitem_174, -)
  wasGeneratedBy(ex:revisionitem_173, ex:add_revision, -)
  wasGeneratedBy(ex:revisionitem_174, ex:remove_revision, -)
endDocument
