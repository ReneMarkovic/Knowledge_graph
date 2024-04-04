# Constructing a Knowledge Graph from Wikipedia's Web of Connections

## Objective

The goal of this project is to build a knowledge graph that represents the interconnectedness of concepts within Wikipedia. You'll start with random Wikipedia articles and perform "random walks" by following links, discovering the relationships between seemingly unrelated topics.

## Understanding Knowledge Graphs

**Knowledge Graphs:** Data structures that represent facts and relationships between entities (things, people, places, concepts). Think of them as maps of knowledge.

- **Nodes:** Individual entities within the graph.
- **Edges:** Connections or relationships between the nodes.
- **Triples:** The basic building blocks of a knowledge graph: (Subject, Predicate, Object). Example: (Leonardo da Vinci, painter of, Mona Lisa)

## Project Steps

**Data Gathering with a Random Walk:** Use the content of an initially random Wikipedia article to find the first substantive link (not a definition, disambiguation, or language link). Follow that link to a new article. Repeat this process several times per random starting point.

**Record:** Keep track of the articles you visit and the links (relationships) between them.

## Knowledge Graph Construction

Select a graph database or a library suitable for knowledge graph representation (like Neo4j or NetworkX).

**Create Nodes:** Make each unique Wikipedia article a node in your graph.

**Establish Edges:** The links you follow during your random walk will become edges representing relationships.

**Advanced option (edge labels):** Label edges with the type of relationship (e.g., "related to", "subject of", "author of").

## Exploration and Analysis

**Visualization:** Create visual representations of your knowledge graph to see the connections emerge.

**Scope:** Start with a focused number of articles or a specific domain within Wikipedia to keep the project manageable.

**Cleaning:** Wikipedia can have disambiguation pages or links to other language versions. Implement some cleaning steps.

**Wikipedia API:** Consider utilizing the official Wikipedia API for more efficient data gathering.
Project Extensions

**Weighted Edges:** Assign weights to connections based on the frequency they appear in walks.

**Natural Language Processing (NLP):** Use NLP techniques to extract more nuanced relationships from the text of Wikipedia articles.

**Inference:** Use graph analysis tools to uncover implicit knowledge not directly stated in the articles.

# Project Goals

1. Scrape Wikipedia articles and create a list of related articles.
2. Use NLP to extract more nuanced relationships from the text of Wikipedia articles (advanced not necessary).
3. Create a knowledge graph of Wikipedia articles.
4. Explore the graph and find interesting connections.
5. Create visualizations of the graph.
6. Make the knowledge graph accessible to others.
