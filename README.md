# Software Architecture Documentation Template&nbsp;[![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https://dassiorleando.github.io/software-architecture-documentation-template/&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=false)](https://dassiorleando.github.io/software-architecture-documentation-template/)

You can access the generated documentation [here (demo)](https://dassiorleando.github.io/software-architecture-documentation-template/), it's based on a sample you can download at [arc42.org](https://arc42.org/download).

<!--- this diagram will show in GitHub-like Markdown viewer -->
```mermaid
sequenceDiagram
    title Sample Mermaid Diagram
    box Purple Alice & John
    participant A
    participant J
    end
    box Another Group
    participant B
    participant C
    end
    A->>J: Hello John, how are you?
    J->>A: Great!
    A->>B: Hello Bob, how is Charley?
    B->>C: Hello Charley, how are you?
```

## Capabilities

* `Arc42` - the documentation template in place, [link](https://arc42.org/).
* `Mermaid` - used for diagramming to better illustrate your software architecture, [link](https://mermaid.js.org/).
* `C4 Model` - For context and container representation of your systems, [link](https://c4model.com/).
* `Mkdocs  Material` - is being used as the static site generator along with the material template, [link](https://squidfunk.github.io/mkdocs-material/).
* `GitHub Action` - CI/CD in place to deploy the documentation as a GitHub Page site.

## Commands

* `pip install -r requirements.txt` - install the dependencies.
* `mkdocs serve` - Start the live-reloading docs server.
* `mkdocs build` - Build the documentation site.
* `mkdocs -h` - Print help message and exit.


## Project layout

    mkdocs.yml    # The configuration file.
    docs/
        index.md  # The documentation homepage.
        diagrams  # Folder containing your Mermaid and C4 diagrams.
        decisions # The location of your architecture decisions records.
        images    # Images displayed in the pages.
        css/js    # To be used only if you need to customize the site.
        .github   # GitHub Action CI/CD pipeline.
        ...       # Other markdown pages, images and other files.

## TODO

- [x] Fix the GitHub Page link.
- [ ] Generate a PDF version of the software architecture documentation.
