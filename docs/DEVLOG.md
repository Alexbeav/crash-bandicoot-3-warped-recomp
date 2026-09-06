# Release preparation

2026-09-06: Prepared a portable setup recipe from accepted framework `63446a28111a21a0cb7e8b5106c3614c898fc4b5`.
The release snapshot keeps functional code and title seed bytes, adds the bounded setup backport, and excludes private input/history.
Consulted the local release process, PSX-PUB-016, the accepted title handoff, and [Git orphan-branch documentation](https://git-scm.com/docs/git-checkout).
The shared archive gate now accepts only exact hashes for two intentional SDK path-example files; changed and relocated fixtures still fail.
Native CI and Windows package acceptance are pending.

2026-09-07: Native canaries identified the GCC9 C-label rule and an unconditional OpenBIOS SDK requirement. The pinned correction adds a C empty statement and derives required BIOS assets from the title recipe. Five synthetic production-gate cases and a strict-C11 positive/negative control pass. Package instructions now state the exact accepted BIOS. Redump metadata uses canonical basenames with unchanged accepted first-track hashes. The replacement native run remains build-only.
