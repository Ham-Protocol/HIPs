# Ham Improvement Proposals (HIPs)

Ham Improvement Proposals (HIPs) describe modifications or proposals made for the HAM protocol, including piggy bank (treasury) decisions, and any changes we wish to make from the YAM base.

# Contributing

 1. Review [HIP-1](HIPS/hip-1.md).
 2. Fork the repository by clicking "Fork" in the top right.
 3. Add your HIP to your fork of the repository. There is a [template HIP here](hip-template.md).
 4. Submit a Pull Request to HAM's [HIPs repository](https://github.com/ham-protocol/HIPs).

Your first PR should be a first draft of the final HIP. It must meet the formatting criteria enforced by the build (largely, correct metadata in the header). An editor will manually review the first PR for a new HIP and assign it a number before merging it. Make sure you include a `discussions-to` header with the URL to a discussion forum or open GitHub issue where people can discuss the HIP as a whole.

If your HIP requires images, the image files should be included in a subdirectory of the `assets` folder for that HIP as follows: `assets/hip-N` (where **N** is to be replaced with the HIP number). When linking to an image in the HIP, use relative links such as `../assets/hip-1/image.png`.

Once your first PR is merged, we have a bot that helps out by automatically merging PRs to draft HIPs. For this to work, it has to be able to tell that you own the draft being edited. Make sure that the 'author' line of your HIP contains either your GitHub username or your email address inside <triangular brackets>. If you use your email address, that address must be the one publicly shown on [your GitHub profile](https://github.com/settings/profile).

When you believe your HIP is mature and ready to progress past the draft phase, you should do one of two things:

 - **For a Standards Track HIP of type Core**, ensure you issue is brought up to the lead devs and contributors, where it can be discussed for inclusion in a future upgrade or vote. If implementers agree to include it, the HIP editors will update the state of your HIP to 'Accepted'.
 - **For all other HIPs**, open a PR changing the state of your HIP to 'Final'. An editor will review your draft and ask if anyone objects to its being finalised. If the editor decides there is no rough consensus - for instance, because contributors point out significant issues with the HIP - they may close the PR and request that you fix the issues in the draft before trying again.

# HIP Status Terms

* **Draft** - an HIP that is undergoing rapid iteration and changes.
* **Last Call** - an HIP that is done with its initial iteration and ready for review by a wide audience.
* **Accepted** - a core HIP that has been in Last Call for at least 2 weeks and any technical changes that were requested have been addressed by the author. The process for Core Devs to decide whether to encode an HIP into their clients as part of a hard fork is not part of the HIP process. If such a decision is made, the HIP will move to final.
* **Final (non-Core)** - an HIP that has been in Last Call for at least 2 weeks and any technical changes that were requested have been addressed by the author.
* **Final (Core)** - an HIP that the Core Devs have decided to implement and release in a future hard fork or has already been released in a hard fork. 
