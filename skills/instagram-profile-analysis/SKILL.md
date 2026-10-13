---
name: instagram-profile-analysis
description: "Analyze a public Instagram profile from its accessible bio, posts, reels, captions, and highlights when the user asks what the person is like, does, knows, or projects online. Separate direct evidence from inference and do not turn aesthetics into unsupported claims."
---

# Instagram Profile Analysis

Needs: browser control

Inspect the actual profile before answering. Use the signed-in browser session when available, but do not message, follow, like, save, or otherwise interact unless the user asked for that action.

## Evidence standard

- Read the bio, counts, links, highlight labels, and the accessible feed.
- Open enough posts and reels to understand their contents; captions and thumbnails alone are insufficient when the user asks for a thorough analysis.
- If the user explicitly asks for every post or highlight, review all accessible items and state what could not be opened or read.
- Distinguish among:
  - **Explicit:** stated by the account owner or directly shown.
  - **Strong inference:** repeatedly supported by multiple posts.
  - **Weak inference:** plausible but uncertain; label it clearly or omit it.
- Never describe an inference as a discovered fact.

## Analysis boundaries

- Analyze the online persona and demonstrated behavior, not an unknowable complete private personality.
- Do not infer exact location, ethnicity, nationality, religion, medical conditions, criminality, military affiliation, or technical access from language, clothing, aesthetics, jokes, or usernames. Report these only when explicitly self-disclosed, and preserve that attribution.
- Do not diagnose mental health, intelligence, or personality disorders. Intelligence may be discussed only through demonstrated skills such as writing, reasoning, technical work, or artistic judgment.
- Cybersecurity imagery, terminals, code screenshots, or the word "hacker" do not establish hacking capability. Examine what the code or workflow actually does.
- Keep different people in separate evidence bins. Do not transfer traits, claims, or relationship information between profiles.
- Avoid doxxing and location triangulation. Broad regional ties may be noted only when repeatedly and publicly self-disclosed; do not derive private addresses, routines, or precise whereabouts.

## Output

Lead with the most defensible overall read, then cover whichever of these the user requested:

- what the person appears to do;
- demonstrated skills and technical depth;
- projected personality and communication style;
- interests and recurring themes;
- explicit biographical or religious claims;
- notable contradictions or image-management choices;
- what cannot be established.

Be direct about thin evidence. Use phrases such as "the account projects," "she explicitly says," or "the posts demonstrate" instead of pretending certainty. Mention the reviewed scope, including inaccessible captions, private material, deleted items, or unreviewed highlights.

## Rule examples

- Valid: review accessible reels and name the highlights that could not be opened.
- Invalid: claim all posts reviewed from grid thumbnails.
- Valid: the account explicitly states its hobby; repeated posts support an interest inference.
- Invalid: diagnose a disorder or infer private whereabouts from imagery.
- Valid: inspect the claimed code activity before describing demonstrated skill.
- Invalid: treat a terminal screenshot as proof of technical capability.
