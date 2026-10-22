# CampusNotes

CampusNotes is a web platform where Yıldız Technical University (YTÜ) students share and find course notes, past exam questions and solutions, organized by course and rated by other students.

Today, course materials are scattered across department WhatsApp groups and passed down from upper-year students. Files get lost in chat history and are hard to find before exams. CampusNotes puts them in one searchable place.

> Status: planning phase (Week 4). First release planned for Week 12.

## Team

| Member | Role |
| --- | --- |
| Gökay Mızrak | Project lead, backend |
| İbrahim Muhsin Yıldırım | Frontend and UX |
| Yasin Buğra Tolu | QA, DevOps, backend support |

## Tech stack

- **Backend:** Python + Flask
- **Pages:** Jinja2 HTML templates + Bootstrap CSS
- **Database:** SQLite (development), PostgreSQL (deployment), via SQLAlchemy
- **Login:** Flask-Login
- **Tests / CI:** pytest + GitHub Actions
- **Hosting:** Render

## Planned features (first release)

- Sign up and log in
- Browse materials by faculty, department and course
- Upload PDFs or images (notes, past exams, solutions)
- Search by course code, course name and title
- Upvote / downvote materials
- Report a material; moderator panel to hide or delete it

## Running locally

> Setup instructions will be added once the first code is in the repository (Week 6).

```bash
git clone https://github.com/<campusnotes4>/campusnotes.git
cd campusnotes
python -m venv venv
source venv/bin/activate        # Windows: venv\Scripts\activate
pip install -r requirements.txt
flask run
```

## Running tests

```bash
pytest
```

## Contributing

- `main` is protected: no direct pushes.
- Create a branch per issue: `feature/<issue-number>-short-name` or `fix/<issue-number>-short-name`.
- Open a pull request that links the issue (`Closes #<number>`).
- CI must pass and one other team member must approve before merging.
- Commit messages start with `feat:`, `fix:`, `docs:`, `test:` or `chore:`.

## Documents

- Software Development Plan (D1): `docs/<TeamName>_D1_SDP.pdf`
- Project board: GitHub Projects tab of this repository
