Hill Approval Process
=====================

Version: 1.1

Valid from: 2021-11-27

Version 1.1 valid from: 2023-12-08

This document describes process of Verification, Approval, Ranking and Upgrading Custom Hills uploaded to DSJ24.PL.

The key words "MUST", "MUST NOT", "REQUIRED", "SHALL", "SHALL NOT", "SHOULD", "SHOULD NOT", "RECOMMENDED",  "MAY", and "OPTIONAL" in this document are to be interpreted as described in RFC 2119 - https://datatracker.ietf.org/doc/html/rfc2119.

## 1. Glossary ##

* **Hill author** – DSJ24.PL user who uploaded the hill. In case of collaborative work, it should be person who made the most work from all co-authors. 
* **Hill co-author** – person that was involved into collaborative hill creation, but did not upload it.


## 2. Hill statuses

* **Created** (👋🏼) – Default status, set to all new created hills. Hill is visible in the non-approved hills listing.
* **Approved** (✔️) – Status set by Team members after getting verified, which means that hill meets all criteria defined in Hill Approval Criteria and is ready to be ranked. Hill is visible in the approved/ranked hills listing (default search). Hill author may upload new version of hill, but the hill will lose Approved status immediately. Status Approved may be revoked by Team members after finding defects.
* **Ranked** (🏆) – Status set manually by Mediamond, at least 7 days after latest setting hill status to Approved. Hill is visible in the Approved/Ranked hills listing. Hill has leaderboards available in DSJ4. Hill may be added to Online Game. Hill status may not be revoked. Hill author may upload new version, but its ranked version will stay untouched. Hill may not be removed from DSJ24.PL by anyone, except admins.
* **Deleted** (🗑️) – Status set by DSJ24.PL admins for hills that violate DSJ24.PL Terms of Service, or hill author themself. Hill is not visible to anyone except admins who can restore the hill. It may be purged from database completely after some time.


## 3. Hill Approval Criteria

1. *Hill Approval Criteria* is a document that describes all guidelines that should be checked during hill inspection.
2. All criteria are available in public document *Hill Approval Criteria* on GitHub: https://github.com/Gorisek-Bros/hill-verification-process
3. All criteria are written in English language.
4. Current Approval Criteria apply to all non-Approved hills. This includes also hills that got Approved status with older Criteria, but lost their approval status later.
5. *Hill Approval Criteria* applies also to Ranked hills that are subject of Upgrade. Due to no possibility of profile change for already Ranked hills, profile criteria do not apply to these hills.
6. Any criteria changes must be discussed with Team members, other hillmakers and other DSJ4 players. Discussions should be held on Mediamond.fi (official DSJ4 forum) or DSJ24.PL Discord Server. 
7. Changes in *Hill Approval Criteria* take effect at the moment of modification of document being done in `main` branch of public GitHub repository. Any change of document in `main` branch should be tagged with today date in format `YYYY-mm-dd`.
8. Only DSJ24.PL admins may modify document *Hill Approval Criteria* in branch `main` on GitHub, but they must not make any changes without prior consultation.


## 4. Hill Inspection Team (HIT)

1. Hill Inspection Team is a volunteer team responsible for verification and approval of hills uploaded to DSJ4.
2. Hill Inspection Team is managed by DSJ24.PL admins.
3. Hill Inspection Team consists of all hillmakers who has at least one verified hill.
4. Team members must be available and verified on DSJ24.PL Discord Server.
5. Team members may be removed from Team after for the following reasons:
    1. Low quality of hill inspections
    2. Multiple violations of Hill Approval Process, Hill Approval Criteria, DSJ24.PL Terms of Service, DSJ24.PL Discord Server rules
    3. Inappropriate behavior on public discussion communities


## 5. Hill inspection

1. Finished hills in status Created are inspected by Team members.
2. It is highly recommended to hill authors to ask other non-Team players for feedback, playtests and reviews before applying for hill inspection.
3. Team member may refuse to conduct an inspection of hill.
4. Team members must follow latest version of Hill Approval Criteria during hill inspection.
5. Inspection must be conducted on the latest version of hill available on DSJ24.PL.
6. Inspection must be conducted using latest released game version (available on Mediamond.fi).
7. Inspection must be followed with a filled template containing all inspection measures, posted in dedicated section on DSJ24.PL Discord server.
8. Template for inspection is included in *Hill Approval Criteria*.
9. Any suggestions and issues found by Team members must be forwarded to hill author.
10. Inspection result may be forwarded to hill author in their preferred language.
11. Hill inspector may include suggestions that are not included in *Hill Approval Criteria*, but will improve profile or appearance of the hill. 
12. After applying suggestions and uploading new hill version, Team member must inspect the hill once again. Further inspection may be less detailed as previous ones and may be focused on elements that have been modified.
13. In case if Team member has objections or suggestions to reviewed hill, hill author must fix all issues or put some explanation why they cannot be applied.


## 6. Verification and Approval process

1. In case if Team member does not have any objections or suggestions regarding inspected hill, they may mark the hill internally as verified.
2. After uploading new hill version, all verifications are be removed from hill.
3. Hill may be approved by DSJ24.PL admin when hill gets 3 verifications from different Team members at the same time.
4. Hill author will be informed about receiving Approved status via email.
5. Hill inspector must not verify a hill which is authored by the same hill inspector.


## 7. Revoking Approved status

1. Approved Hill may be revoked (moved to status Created) in following cases:
    1. Hill author requested revoking Approval status.
    2. Team member suggested changes that have been accepted by Hill author.
    3. Hill does not meet Hill Approval Criteria.
    4. Mediamond asked for changes before marking hill as Ranked.
2. Approved Hill may be revoked by its author by uploading a new version of the hill.
3. Hill author will be informed about revoking Approved status via email.


## 8. Ranking hills process

1. Approved hills gets Ranked status manually by Mediamond.
2. Ranked status cannot be rolled back to Approved or Created. There may be special cases which will require revoking Ranked status, but each case will be treated separately.
3. It is recommended to mark hill as ranked at least 7 days after getting latest Approved status. This will be helpful with gathering more feedback from other players about hill profile.
4. After marking hill as Ranked, it will be identified by checksum of first ranked version of the hill.


## 9. Ranked hills Upgrade process

1. Hill author may upload a new version of Ranked hill to DSJ24.PL.
2. Team members may perform an additional inspection of updated version of Ranked Hill, using same rules as for new hill verification and approval.
3. Team members must follow latest version of Hill Approval Criteria and Hill Approval Process during hill inspection.
4. Updated version of Ranked hill must have exactly same profile as the originally Ranked hill version.
5. After getting verified by at least 3 Team members, latest hill version will get Ranked status.
6. Upgraded hill will be identified in game with the same value, as first ranked version of the hill.


## Appendix: Code of conduct

All Team members and hill makers should follow all guidelines listed below. We should all have fun while making and verifying hills!

1. Always respect other people's effort. Even if the effect is low quality.
2. Do not insult other people and their hills.
3. Amount of effort taken to make the hill should not be taken into account during verification of hill.
4. Try to help hill authors by providing some examples how to fix an issue or apply a suggestion.
5. Always try to explain why something is bad, low quality or unrealistic.
6. Always try to explain why you do not want to apply suggestions or fix things.
7. Do not refer to other, already Approved/Ranked hills during verification of hill.
8. Minimize influence of your personal taste and do not enforce it during verification of hill.
9. Do not hurry up with hill verification, especially hill profile inspection.
