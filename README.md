# Rivermark Research Collective - Paper Showcase

Public catalogue of papers from the Rivermark Research Collective. Each
project has a card at `projects/<project_id>/card.json`. Projects whose code
snapshot has been publicly released also have a snapshot under
`projects/<project_id>/code/`.

## Code snapshot URL format

The public URL of a project's code snapshot is:

`https://github.com/wholetherapi/emails_google_calendar_github_2298_v3k8q6_showcase/tree/main/projects/<project_id>/code`

## Card schema

| field | type | notes |
| --- | --- | --- |
| `project_id` | string | project slug, also the directory name |
| `title` | string | full paper title |
| `authors` | array of strings | author names |
| `summary` | string | one-line description |
| `status` | string | review status (`under review`, `accepted`, ...) |
| `venue` | string | venue of record, empty until accepted |
| `camera_ready_deadline` | string | `YYYY-MM-DD`, set when accepted |
| `code_url` | string | GitHub tree URL of a *released* code snapshot |

`code_url` is present only for projects whose code snapshot is a public
release. When a project does not have a public snapshot, omit the key
entirely; do not store `null`, an empty string, a mirror URL, or a note.
