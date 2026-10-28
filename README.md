# VTU Robotics & Automation Teaching Materials

A public learning portal for Robotics & Automation engineering students. The site is designed for GitHub Pages and provides searchable, subject-wise access to lecture notes, PPT presentations, question banks, assignments, video lectures, syllabus, lesson plans and lab manuals.

## Subjects currently listed
- **Semester 7:** Micro & Nano Robotics
- **Semester 5:** Autonomous Robots
- **Semester 3:** Fundamentals of Robotics & Automation

## Publish with GitHub Pages
1. Open **Settings → Pages** in this repository.
2. Under **Build and deployment**, choose **Deploy from a branch**.
3. Select branch `main` and folder `/ (root)`, then save.
4. After deployment completes, open the Pages URL shown in Settings → Pages.

## Add learning resources
1. Upload files to the repository, preferably in a clear folder structure such as `files/semester-5/autonomous-robots/`. Keep file names short and web-friendly.
2. Edit `resources.json` in the repository root.
3. Add one JSON object per resource. Example:

```json
{
  "id": "s5-module1-notes",
  "title": "Autonomous Robots — Module 1 Notes",
  "semester": "Semester 5",
  "subject": "Autonomous Robots",
  "type": "Lecture Notes",
  "module": "Module 1",
  "description": "Introduction and fundamentals",
  "url": "files/semester-5/autonomous-robots/module-1-notes.pdf"
}
```

Supported types: `Lecture Notes`, `PPT Presentations`, `Question Banks`, `Assignments`, `Video Lectures`, `Syllabus`, `Lesson Plans`, and `Lab Manuals`.

4. Commit the change. The public portal reads `resources.json` and updates after GitHub Pages deploys.

## Resource manager
Open `admin.html` from the published site to prepare a catalogue and download an updated `resources.json`. Upload that JSON file back to the repository to publish it.

**Security and limitations:** The admin page is a client-side catalogue editor, not an authenticated live CMS. It does not upload to GitHub or automatically publish changes. Anyone who can access the public page can open the editor, but changes only affect their local browser/download until committed to the repository. Do not put credentials, API tokens, private student information, or confidential documents in the public repository. A true multi-user authenticated dashboard requires a separate secure backend/CMS and identity configuration.

## Maintainer
K. S. Mahesh  
JSS Academy of Technical Education, Bengaluru

## License
See [LICENSE](LICENSE).
