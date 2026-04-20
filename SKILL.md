# Common Mistakes on the Job

A short list of the ways an agent with shell access to a populated
sandbox tends to fail. Treat each one as a check before you act,
not a rule to recite.

## "The task surface is obvious from here"

The surface is whatever this sandbox exposes this session, not what
you remember. `curl http://localhost:8090/openapi.json` and
`/workspace/INSTRUCTION.md` are authoritative; everything else is
guess. Services, endpoints, and fixture shapes rotate between runs.

## "This detail is close enough to use"

Every name, identifier, timestamp, number, status, or quoted
string in any output you produce must come from a response you
received this session. Name in your head the exact field you
pulled each one from. If you cannot, remove it — do not
paraphrase, do not round, do not bridge with a plausible value.

## "Urgent items go at the top, the rest afterwards"

Ordering does not protect the urgent thing. If something looks
like a live incident, a regulator-visible deadline, or a
customer-facing outage in progress, pause the rest of the work
and handle it first. A buried P0 inside a tidy summary still
scores as a missed P0.

## "Leadership owns escalation, so they should see everything"

An oversight title does not inherit access to operational
detail. Status belongs to leadership, impact belongs to external
audiences, full detail stays with the peers doing the hands-on
work. Before you add a recipient, a CC, or an attendee, identify
which tier they belong to and whether the message is at that
scope.

## "The send confirmation was the whole job"

A write is not finished until the target endpoint echoes the new
value. After posting, emailing, scheduling, filing, or creating,
re-read the same resource and confirm the change shows up with
the values you intended. This catches the wrong-field,
dropped-write, and partial-update failures that successful
status codes hide.

## "The outside audience will appreciate the extra context"

External and broadcast recipients learn only what affects them:
user-visible symptoms, acknowledgment, the next checkpoint.
Internal system names, ticket numbers, topic labels, attendee
lists, dollar figures, and unreleased plans you learned inside
the sandbox this session stay inside the sandbox.

## "One combined follow-up captures it all"

A bundled note is not follow-through. Each distinct action by
each distinct owner becomes its own task or calendar event: a
verb-first title, the owner populated from observed data, and
one grounded sentence of context. A stranger reading only the
artifact should be able to pick it up cold.

## "'Just a few minutes' is a commitment"

"Soon", "shortly", "ASAP", "we'll circle back" are not
commitments. Replace them with a concrete time, a named
checkpoint, or an explicit "I do not have a timeline yet and
will update at X." A commitment without a time is worse than
no commitment at all.
