# Constitution for collaboration on this essay

This file is the project source of truth for how agents collaborate with Brian
Holman on **AI Is Not a Bubble**. It records the instructions established in this
conversation and is a living document, not a claim that every future decision has
already been made. Follow it within applicable system and developer requirements.
An explicit subsequent instruction from Brian supersedes conflicting project
guidance; update this file to reflect an agreed change. Do not invent approvals
or treat an agent's suggestion as an accepted rule.

## Author and authority

- Brian Holman, founder and CEO of Dezota, is the author and approval authority.
- Agents may create, edit, save, and validate local essay documents as work
  progresses within the authorized task.
- **Git commits and pushes to the server each require Brian's explicit
  authorization.** Permission to save documents locally is not permission to
  commit or push. Permission for one action does not imply permission for the
  other or standing authorization for future actions.
- The earlier phrase allowing documents to be checked in after each step is
  interpreted as permission to save local work, because Brian separately required
  authorization for commits and pushes.

## Commit message review and approval

- Before committing or pushing, inspect the pending changes and present Brian
  with the exact proposed commit message, including its subject and body, plus
  a brief summary of the files and changes to be included.
- Incorporate Brian's requested wording changes and show the revised draft.
  A request to see or revise a draft is not approval to commit or push.
- Wait for Brian's explicit approval of the final message and the actions to be
  taken. Commit and push may be approved together when both are explicitly
  included in that approval; approval of message wording alone authorizes neither.
- Use the approved message exactly. If the message or included changes need to
  change after approval, present the revision for approval before proceeding.
- Keep ignored private documents, passwords, scripts, and working files out of
  the commit unless Brian explicitly changes their inclusion rules.

## Repository boundary

- Make file changes only in this repository:
  `~/Documents/AI-Is-Not-A-Bubble-Essay`.
- Do not modify the WealthProof repository or the Dezota website repository.
- Read relevant WealthProof news-summary guidance when needed to apply Brian's
  requested summary standards. This reference access does not authorize changes,
  imports, or publication in WealthProof.
- Preserve unrelated existing work. Do not broaden a task into changes to another
  application or repository.

## Article research and summaries

- Keep article summaries in `Articles/`.
- Provide a human-readable Markdown summary. If also producing JSON, use the
  same filename stem for the `.md` and `.json` files and keep their shared summary
  and metadata consistent.
- Apply the WealthProof news-summary standards Brian requested, summarized below.
  The reference consulted when establishing these rules was
  `~/Development/WealthProof/client/public/news-curation-task.md`.
  Its app-specific import workflow does not authorize importing this essay's work.
- Read the actual article sufficiently to summarize it. For a request about the
  current Apple News screen, inspect the native app and read the article through
  its conclusion. Do not manufacture a full-article summary from a headline,
  snippet, or inaccessible paywall; report access limitations accurately.
- Record the publication, exact headline, author when displayed, and displayed
  publication date. Distinguish an updated date from the original publication
  date. Never substitute the reading date or saved-story date for the source date.
- Obtain the actual article share URL, preferably its Apple News HTTPS link.
  Preserve its case-sensitive identifier; do not guess a destination.
- Write an original, one-paragraph summary of roughly **80–150 words** in the
  article's language. Explain the central argument, relevant evidence or figures,
  implications, and limitations. Additional clearly separated details may appear
  in the Markdown document.
- Attribute opinions, predictions, and company developments to the article.
  Distinguish source claims from independently verified facts and agent analysis.
  Do not present historical forecasts as current facts or personalized advice.
- Paraphrase rather than reproducing article text or lengthy quotations.
- Assign a content type and **2–6 concise, reusable topic tags**. Use consistent
  spelling and capitalization. Identify sponsorship when relevant.
- State what was actually read and any observed access restriction or uncertainty.
  Do not infer subscription requirements from successful access in an existing
  session.
- For JSON, use a UTF-8 array of article objects with `date`, `source`, `title`,
  `url`, `subject`, `summary`, `content_type`, and `tags`; include `access_status`
  and `date_source` for provenance. Set `date_source` to `null` unless an actual
  HTTPS date reference was checked. Validate the JSON and consistency with the
  Markdown companion before delivery.
- Do not add full article text, credentials, account identifiers, or publication
  commands to the exported files.

## Communication and completion

- Carry out authorized local work without repeatedly asking for permission already
  given. Ask when necessary information or new authorization is actually missing.
- Report the concrete result, relevant limitations, and where the documents were
  saved. Clearly distinguish local saves from commits and server pushes.
- Repository files may be referenced as they appear in Gitea's web interface.
  Prefer repository-relative Markdown links within project documents so they
  remain usable on Gitea. Use verified web URLs when linking directly to the
  server; do not guess its web address from the Git SSH remote.
- Cross-link related essay passages, career vignettes, professional-history
  entries, and article summaries with relative Markdown links. Resolve each link
  from its containing document, encode spaces as `%20`, and verify that its target
  exists. Keep links to private documents out of publication files.
- Write references to documents under the user's home directory with `~/`,
  for example `~/Development/WealthProof/`, rather than a machine-specific
  absolute home-directory prefix. Apply this convention in repository documents
  and user-facing path text. Continue using repository-relative links for files
  within this repository. Expand `~` internally when a tool requires an absolute
  filesystem path.
- Keep editorial choices that Brian has not yet specified open. The essay title
  alone does not establish an approved outline, argument, or treatment of evidence.

## Established record

- **September 30, 2026:** Brian restricted all changes to this essay repository,
  requested an `Articles` folder and the WealthProof news-summary standards,
  required a human-readable Markdown companion for JSON summaries, reserved
  commit and push authorization to himself, requested this constitution, and
  permitted references to repository files as they appear on Gitea's web version.
