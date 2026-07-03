# Triple-store Configuration

Your {{site.opva}} can run with multiple RDF triple-stores as backend storage.

Starting with version 4.0, the virtual appliance ships with AllegroGraph as the default RDF store. To fully configure it, visit the <a href="{{site.baseurl}}/administration-guide/steps/allegrograph_configuration">AllegroGraph Configuration</a> page before you begin uploading content.

If you want to switch to using 4store instead (**not recommended**), visit the <a href="{{site.baseurl}}/administration-guide/steps/4store_configuration">4store Configuration</a> page for detailed instructions.

OntoPortal can also run with [Virtuoso](https://virtuoso.openlinksw.com/) as its triple-store; see the <a href="{{site.baseurl}}/administration-guide/steps/virtuoso_configuration">Virtuoso Configuration</a> page.

Beyond these, OntoPortal can also run with [GraphDB](https://graphdb.ontotext.com/). This option is not yet documented here; in the meantime, see [agroportal/project-management#229](https://github.com/agroportal/project-management/issues/229) for the current status and pointers.

{: .highlight }
If you use the Virtual Appliance 4.0 based on the AgroPortal codebase, it ships with **Virtuoso** as the default triple-store.
