# Garden
A data model to represent the garden of the mind. Tools that help the gardener with gardening are created seperately. The garden also parallels traditional website use and early internet culture but with a design distinctly focused on private use through a streamlined data model. However, this doesn't mean that data has to remain private.

Zettel people can be picky about their tools and so may the best tools win!

## Data Model
All the entities are unique and should be immutable when implemented.
### Notes
There is the note and it should be a string that contains only itself and it should not be able to link to anyting else in it's text.
### Nodes
Nodes are have a note they represent. Nodes can also link to other nodes. Nodes can also have multiple tags.
### Tags
Tags are metadata about nodes that help with grouping nodes

## Potential Applications
- Graph Viewers
- Tag Viewers (Set Theory)
- HUGO theme
- PWA
- Editor integrations
- Cooking Based Gardens
- Colaborative Cooking Based Gardens
- SOLID pod?

## Design Priniciples
0. cards are simple and should be limited as much as possible with word count, formatting, etc. (it is possible rules for limiting the extensibility of an individual card should be set)
1. interacting with the zettel should be textualar
2. card files should be named with a uuid based on creation time (I like unix time stamps)
3. zettels should be immutable at a system level such that rich metal data on the state of zettel updates can be maintained
4. tags are use to create heirarchical knowledge i.e. venn diagrams that individiaul cards fall into
5. links can arbitrarily be created between cards
