# CampusNotes

CampusNotes is a web app where Yıldız Technical University (YTÜ) students share and find course notes, past exam questions and solutions, organized by course and upvoted by other students.

Today, course materials are scattered across department WhatsApp groups and passed down from upper-year students. Files get lost in chat history and are hard to find before exams. CampusNotes puts them in one searchable place.

> Status: planning phase (Week 4). Final demo planned for Week 12.

## Team

| Member | Role |
| --- | --- |
| Gökay Mızrak | Project lead, backend (Flask routes, login, uploads) |
| İbrahim Muhsin Yıldırım | Frontend (HTML templates, Bootstrap) |
| Yasin Buğra Tolu | Database and testing |

## Tech stack

- **Backend:** Python + Flask
- **Pages:** Jinja2 HTML templates + Bootstrap
- **Database:** SQLite
- **Login:** Flask-Login
- **Tests:** pytest

The app runs locally; there is no public deployment in the first release.

## Planned features

- Sign up and log in
- List courses and their materials
- Upload PDFs or images (notes, past exams, solutions)
- Search by course name or title
- Upvote materials
- Report a material; an admin can delete reported items

## Running locally

> Setup instructions will be completed once the first code is added (Week 6).

```bash
git clone https://github.com/campusnotes4/campusnotes.git
cd campusnotes
python -m venv venv
venv\Scripts\activate          # macOS/Linux: source venv/bin/activate
pip install -r requirements.txt
flask run
```

## Contributing

- Create a branch per issue: `feature/<issue-number>-short-name`
- Open a pull request that links the issue (`Closes #<number>`)
- One other team member reviews before merging
