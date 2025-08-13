flowchart TB
А --> B
C --- D
E -.-> F
G ==> H
I --o J
K --x L

gh api --method GET /events -F per_page=2 -F page=1
--header 'Accept: application/vnd.github+json' \
