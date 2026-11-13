# OrganisationOS remote engine preparation

This fork preserves the upstream AGPL license and notices. The pinned base is in upstream.json. No proprietary RustDesk Pro source is included. No production server has been replaced by creating this fork.

The OrganisationOS client admission bridge is not implemented or received. Do not disable the upstream password or consent checks. Rendezvous/relay availability does not authorize a remote-control session.

Before a client release, the target must verify a signed, audience-bound, short-lived OrganisationOS capability; atomically consume its nonce; bind it to the exact Windows session and challenge; revalidate revocation; display participants; reject missing sessions without fallback. File transfer, clipboard, input and concurrent control are separately granted. Personal access does not automatically create a ticket. Emergency admission requires verified strong authentication, justification, protected central audit, policy notifications and post-event review.

## Source and license delivery

Keep LICENSE/LICENCE and upstream notices in every distribution. Publish the exact corresponding fork source, submodule pins, patches and reproducible build instructions for each distributed binary. Provide the network source offer where AGPL section 13 applies. A process boundary does not by itself settle whether the integrated work is covered: review linking, IPC contracts, copied code, shared data structures and distribution as a combined product before release. No license compatibility conclusion is claimed here.

## Security updates

Watch upstream security advisories and releases for both repositories. Fetch from upstream, review the diff from the pinned commit and all submodules, qualify authentication/relay restrictions and license notices, then build a new immutable CP package. Record artifact hashes, source commits, backup and rollback. Do not move the production pin or pull latest automatically. Urgent fixes use the same verified delivery path.

## Rollback

Keep the existing RustDesk service, keys and clients unchanged until the new deployment is independently qualified. Retain keys/data when rolling back a server package. Roll back client admission and server protocol as a compatible pair; never fall back to unauthenticated control.
