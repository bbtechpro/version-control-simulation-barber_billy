
Project Reflection: Version Control Simulation


Branch Management and Workflow

To begin the simulation, I set up a clean Git repository locally and linked it to GitHub. I structured my development workflow by isolating distinct tasks into dedicated feature branches: feature/header and feature/footer. By utilizing commands like git checkout -b, I transitioned between these context-specific environments. This isolated approach prevents developers from accidentally overwriting one another's work and allows for concurrent feature development.

Handling the Merge Conflict

After successfully merging feature/footer into main, attempting to merge feature/header triggered a standard Git conflict. Git flagged the overlapping lines, inserting conflict markers (<<<<<<<, =======, >>>>>>>) directly into the file. To resolve it, I opened index.html, analyzed the conflicting structural elements, and manually edited the file to preserve the intended layout of both the header and the footer. After cleaning up the markers, I used git status to verify the state of the repository, staged the clean file with git add, and finalized the resolution with a merge commit.

Pull Requests and Collaboration

The final phase demonstrated how Pull Requests (PRs) act as a vital quality assurance gatekeeper in a collaborative environment. Proposing changes from main to review/main provided a transparent forum for peer review before final integration. PRs ensure that code is never merged blindly; they allow team members to leave inline comments, catch syntax bugs, and enforce design guidelines. Reviewing a peer’s work reinforced this collaborative loop, proving that collective oversight inherently elevates overall code health and limits production errors.

