# GitHub identity adoption — WNT-164

Tracking: https://linear.app/wastingnotime/issue/WNT-164/refresh-the-github-organization-identity-and-profile

## Asset provenance

Forward W v1.0.0, approved in WNT-160. Exact upstream revision and SHA-256
hashes are in `profile/identity/v1.0.0/provenance.json`. Copies are byte-for-byte
exports from wnt-design. The README uses an immutable public upstream URL for
the opaque dark lockup, so its mint mark and paper lettering retain contrast in
both GitHub themes. The upload is the original 800 × 800 avatar, with the full
square crop and intentional padding preserved.

## Organization settings (separate from this PR)

Applied 2026-10-15 at https://github.com/organizations/wastingnotime/settings/profile:

- Uploaded `profile/identity/v1.0.0/avatar.png`; GitHub confirmed the update.
- Description: “Practical software, shared engineering foundations, and experiments built in the open.”
- Website: https://wastingnotime.org/
- YouTube: https://www.youtube.com/@wastingnotime
- Public pins: Sliding Tasks, Wishlist, wnt-design, wnt-contracts, wnt-web, wnt-go.
  These foreground products and shared foundations within GitHub's six-pin limit.
  Android remains linked in the README. GitHub confirmed the pins update.

No repository visibility was changed. All named repositories were verified public
with GitHub's API and anonymous HTTP requests. The website is linked directly;
its implementation repository is not linked from the public README.

## Repository change

`profile/README.md` replaces the archived-project-led introduction with current
products, shared foundations, website/YouTube links, and an ideas/request link.
Contacts, HireFlow, Game Hub and MRL Starter remain accessible under “Earlier
experiments.” No claims are made that archived templates are active work.

All 15 distinct external page destinations returned HTTP 200 anonymously on
2026-10-15. The lockup uses the approved opaque background rather than relying on
theme-specific transparent text. Repository changes become the organization README
only after this PR is merged to main; live settings changes already took effect.

## Rollback

Revert the profile commit to restore the previous README. Organization settings
are independent: restore the previous avatar and description (“how to build
software wasting no time?”), clear the website/social fields, and clear these six
pins to restore the previous automatic popular-repositories list. Historical
repositories remain archived and available throughout.

## Visual evidence

- [Live anonymous organization](evidence/wnt-164/organization-public.jpg): approved
  square avatar, public bio/links and six public pins. The old README is still
  visible here because the PR has not merged.
- [GitHub README, dark](evidence/wnt-164/readme-dark.jpg).
- [GitHub README, light](evidence/wnt-164/readme-light.jpg): anonymous browser with
  temporary prefers-color-scheme emulation, cleared after capture.

Both theme renders were visually inspected. The history disclosure was expanded
on GitHub and exposed all four archive links. The approved kit's square/circular
avatar specimen was inspected alongside GitHub's full-square upload preview:
all four panels retain clear space inside either crop. The 100px public avatar
remains distinguishable. The exact upstream specimen is
`wnt-design/docs/identity/v1.0.0-specimen.png` at the recorded source revision.

PR: https://github.com/wastingnotime/.github/pull/2

WNT-164 remains in review until the README is merged and the deployed organization
README is captured. WNT-166 retains responsibility for the cross-channel audit.
