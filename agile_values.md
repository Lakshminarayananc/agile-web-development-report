
### Agile values

Agile software development is a fuzzy term that encompasses a lot of different methodologies. The different methodologies can differ a lot in practice. They do, however, share values: a core set of beliefs about what is important in software development. The difference between agile methodologies and traditional software development is the stress agile methodologies put on these values. The most widely cited description of agile values is [Agile Manifesto](TODO).

The first goal of the course was to teach the students agile values. We stressed the following three principles.

* **Minimality**: The price of a project as a function of its requirements grows faster than linearly. Besides requirements, the same holds true with the number of developers, the amount of documentation, and the size of the code base. The project should include just what is needed and nothing more. 
* **Change**: Customer's understanding of his own needs is always lacking, and thus requirements will always change. The project should prepare for this change. 
* **Understanding**: Work done without understanding it leads to trouble. Developer should always understand (a) what he is trying to achieve and (b) why is he trying to achieve it and (c) how he is trying to achieve it.

Combined, there are a few consequences from these values:

* **Minimality+Change**: Preparation for future enlarges the project. Often the plans end up outdated. It is very important that plans are lightweight and easily thrown away when outdated.
* **Minimality+Understanding**: It is important to understand e.g. the domain area and document that understanding somehow. On the other hand, the amount of documentation should be minimized. One document we cannot work without is the program code. Thus, whenever possible, we should store our understanding in the code, not in external documentation. A high priority should be given to keeping the code as readable and as descriptive as possible.
* **Change+Understanding**: The developers' and customer's understanding of the software should keep improving throughout the project. Much of this comes from the dialogue between them. Customer should have a concrete understanding of what is the status of the project, and where it is heading. Because the future is very uncertain, the basis for the feedback should be a working prototype of the system. Thus, project iterations should be short and result in a working software that the customer can evaluate.
