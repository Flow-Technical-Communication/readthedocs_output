---
keyword: [bookmeta, bookid, booknumber, bookpartno, maintainer, volume, edition, isbn, bookrights, copyrfirst, copyrlast, bookrestriction, bookowner, bookchangehistory, approved, edited, reviewed, tested, bookevent, bookeventtype, summary, revisionid, publisherinformation, published, pusblishtype, printlocation, organization, person, started, completed, day, month, year]
---

# Bookmap metadata

The `bookmeta` element contains all information that is not considered book content:

-   Publisher's identification numbers \(`bookid`\)
-   Copyright information \(`bookrights`\)
-   History of the creation and publishing of the book \(`bookchangehistory`\)
-   Publishing information \(`publisherinformation`\)

## `bookid`

The publisher's identification numbers \(`bookid`\) can contain the following elements:

-   The form number \(`booknumber`\)
-   The book's part number \(`bookpartno`\)
-   The maintainer of the document \(`maintainer`\)
-   The volume number \(`volume`\)
-   The edition number \(`edition`\)
-   The ISBN number \(`isbn`\)

## `bookrights`

The copyright information \(`bookrights`\) can contain the following elements:

-   The first copyright year \(`copyrfirst`\)
-   The last copyright year \(`copyrlast`\)
-   Restrictions \(`bookrestriction`\)
-   The owner of the copyright \(`bookowner`\)

## `bookchangehistory`

The history of the creation and publishing of the book \(`bookchangehistory`\) can contain the following events:

-   When and by whom the book was approved \(`approved`\)
-   When and by whom the book was edited \(`edited`\)
-   When and by whom the book was reviewed \(`reviewed`\)
-   When and by whom the book was tested \(`tested`\)
-   General events and their type \(`bookevent` and `bookeventtype`\)

`bookchangehistory` can contain some additional elements:

-   A text summary associated with a book event or list of copyrights \(`summary`\)
-   The revision number \(`revisionid`\)

## `publisherinformation`

The publishing information \(`publisherinformation`\) contains the `published` element, which contains the following elements:

-   Availability from the publisher \(`publishtype`\)
-   Location where the book was printed \(`printlocation`\)
-   Name of the organization publishing the book \(`organization`\)
-   Name of the person publishing the book \(`person`\)
-   Date information: start date of a book event \(`started`\) and completion date of a book event \(`completed`\) containing day \(`day`\), month \(`month`\) and year \(`year`\) elements

**Related information**  


[What is a bookmap?](co_what_is_a_bookmap.md)

[What are the main components of a bookmap?](co_bookmap_main_components.md)

[Bookmap elements](co_creating_bookmap.md)

