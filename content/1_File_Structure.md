# File Structure

While it may seem like it would be rather complicated to create a course that has an entire course dedicated to how to do so, it's actually really simple. 

First, you need to make sure your course materials follow the correct file stucture. Here is an example:
```
.
├── README.md
├── content
│   ├── 03_Pytorch.md
│   ├── 1_Solving_Simple_Systems.md
│   ├── 2_unit
│   │   ├── 01_Eigenvectors.md
│   │   ├── 02_practice.md
│   │   └── index.md
│   └── index.md
└── ocw.json
```

* `ocw.json` specifies your course name, description, tags, and other important general information about your course
* All the files you wish to load into course modules must be in the `content\` folder. The modules are structured in sections/subsections through folders
* An optional landing page for each subsection is in `index.md`
* Course modules must contains a number at the start of their filename specifying its order relative to other positions. If they don't, they will be ignored