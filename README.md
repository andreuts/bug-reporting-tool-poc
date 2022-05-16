# bug-reporting-tool-poc

This is a proof of concept project to test bug management tools. This project has two different ways of creating tools:
- Using the end user bug reporting tool [marker.io](https://app.marker.io/destinations) which opens issues in the Github project.
- Internally reporting bugs using templates in the github project.

Using the [Github kanbanize integration](https://zapier.com/apps/github/integrations/kanbanize) all reported issues in this project will be reflected in Kanbanize. 

## Launch
Branch ``gh-pages`` automatically serves the html in [https://andreuts.github.io/bug-reporting-tool-poc/](https://andreuts.github.io/bug-reporting-tool-poc/)

## Analysis
On reporting bugs on Github:

### Pros
- Reporting bugs using Github issues opens a wide window of opportunities to integrate third party tools to manage bugs/report bugs.
- All bugs will be automatically reported in Kanbanize. Kanbanize KPIs will keep aplying.
- Changes on Github issues will be automatically propagated to the correspondent Kanbanize card.
- Easier for developers to coordinate their development with bugs.
- Easy to report / track / filter / associate to milestones / assign / create a comments thread. We don't lose any important functionality.

### Cons
- Github bug template has to be commited in the project.
- Changes on Kanbanize bug cards won't be automatically propagated to the correspondent Github issues. Asyncronous, which makes this system prone to misleading information.
- Github is not 100% meant to be a bug tracking system - we might encounter some deficencies after some usage.
- Issues are not associated to any branch.
- Non-dev teams won't be able to easily access the project and watch the open bugs. (Altough bugs would still be on KB, this might be necessary at some point for some reason)
