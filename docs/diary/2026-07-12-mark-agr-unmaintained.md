# Diary: Mark agr as unmaintained

Make the project's maintenance status unmistakable and direct users to the
replacement skill-management tool.

## Step 1: Add the maintenance notice

**Author:** main

### Prompt Context

**Verbatim prompt:** let's execute on TODO.md

**Interpretation:** Mark agr as no longer maintained as part of adopting
skills.sh.

**Inferred intent:** Prevent new users from adopting agr and give existing
users a clear replacement.

### What I did

I added a prominent warning near the top of `/README.md` stating that agr is no
longer maintained and linking to skills.sh and its CLI documentation.

### Why

The README is the first place existing and prospective users look for project
status and installation guidance.

### What worked

The notice fits the existing README structure and leaves historical usage
documentation available to existing users.

### What didn't work

Nothing failed during this step.

### What I learned

The repository had no existing deprecation or maintenance-status notice.

### What was tricky

The notice needed to be prominent without rewriting the historical project
documentation.

### What warrants review

Review the warning at the top of `/README.md` and verify both replacement links.

### Future work

No further development is planned for agr.
