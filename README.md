# Commodore Component: argocd-instance

This is a [Commodore][commodore] Component to render [ArgoCD][argocd] instance
Custom Resources and [AppProjects][appproject] managed by the
[ArgoCD operator](https://github.com/argoproj-labs/argocd-operator).

The component allows teams to take over and operate single ArgoCD instances
without owning the ArgoCD operator installation: the operator itself is managed
by [component-argocd][component-argocd], which also owns the parameter layout
used by this component (`config`, `projectDefaults`, `projects` per instance).

This repository is part of Project Syn.
For documentation on Project Syn and this component, see [syn.tools](https://syn.tools).

## Documentation

The rendered documentation for this component is available on the
[Commodore Components Hub](https://hub.syn.tools/argocd-instance) once published.

Documentation for this component is written using [Asciidoc][asciidoc] and [Antora][antora].
It can be found in the [`docs`](docs) folder.
We use the [Divio documentation structure](https://documentation.divio.com/) to organize our documentation.

Run the `make docs-serve` command in the root of the project, and then browse to http://localhost:2020 to see a preview of the current state of the documentation.

After writing the documentation, please use the `make docs-vale` command and correct any warnings raised by the tool.

## Contributing and license

This library is licensed under [BSD-3-Clause](LICENSE).
For information about how to contribute, see [CONTRIBUTING](CONTRIBUTING.md).

[commodore]: https://syn.tools/commodore/
[asciidoc]: https://asciidoctor.org/
[antora]: https://antora.org/
[argocd]: https://argo-cd.readthedocs.io/
[appproject]: https://argo-cd.readthedocs.io/en/stable/user-guide/projects/
[component-argocd]: https://github.com/projectsyn/component-argocd
