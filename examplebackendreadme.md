_This markdown will show many examples of documentation for a backend project and provide snippets of the markdown for each section_

# Backend Project

- **Creators:** Alex Merced, Other Person
- **Description:** A JSON API for getting data on dogs and owners
- **technologies used**: ExpressJS, Javascript

```markdown
# Backend Project

- **Creators:** Alex Merced, Other Person
- **Description:** A JSON API for getting data on dogs and owners
- **technologies used**: ExpressJS, Javascript
```

## Models

_this section would provide ERD diagrams of the models in your application, could be an image or on github you can use "mermaid" syntax to generate diagrams in your markdown here is the link for the syntax [mermaid erd diagrams](https://mermaid.js.org/syntax/entityRelationshipDiagram.html)_

```mermaid
erDiagram
    OWNER ||--o{ DOG : owns
    OWNER{
    int ID
    string name
    int age}
    DOG {
    int ID
    string name
    int age
    int owner_id
    }

```

```markdown
|```mermaid
erDiagram
    OWNER ||--o{ DOG : owns
    OWNER{
    int ID
    string name
    int age}
    DOG {
    int ID
    string name
    int age
    int owner_id
    }
|```
```
_NOTE: ignore the pipes in the code snippet, those are there so backticks don't end the codeblock prematurely_

## The Route Table

_This should be a list of endpoints, methods and descriptions of each route in the api_

| Endpoint | Method | Description |
|----------|--------|-------------|
| /dog | GET | returns all dogs |
| /dog/:id | GET | returns a single dog by id |
| /dog | POST | creates a new dog|
| /dog/:id | PUT | updates a dog based on id |
| /dog/:id | DELETE | deletes a dog based on id |
| /owner | GET | returns all owner |
| /owner/:id | GET | returns a single owner by id |
| /owner | POST | creates a new owner|
| /owner/:id | PUT | updates a owner based on id |
| /owner/:id | DELETE | deletes a owner based on id |
| /adopt/:owner_id/:dog_id | PUT | associates specified dog with specified owner |

```markdown
| Endpoint | Method | Description |
|----------|--------|-------------|
| /dog | GET | returns all dogs |
| /dog/:id | GET | returns a single dog by id |
| /dog | POST | creates a new dog|
| /dog/:id | PUT | updates a dog based on id |
| /dog/:id | DELETE | deletes a dog based on id |
| /owner | GET | returns all owner |
| /owner/:id | GET | returns a single owner by id |
| /owner | POST | creates a new owner|
| /owner/:id | PUT | updates a owner based on id |
| /owner/:id | DELETE | deletes a owner based on id |
| /adopt/:owner_id/:dog_id | PUT | associates specified dog with specified owner |
```

## Markdown Syntax Reminders

```
LINK: [Link Text](URL)
PICTURE: ![ALT TEXT](URL)
Horizontal Line: ---
```
