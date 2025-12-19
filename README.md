# v8-r: Arch Linux Package Sources

This repository contains the build sources for the `v8-r` Arch Linux package, which was actively maintained on the Arch Linux User Repository (AUR) from **September 22, 2019, to December 19, 2025**. [#20](https://github.com/JanMarvin/v8-R/issues/20)

### Project History & Mission
The project began as an experiment to provide a stable V8 library to be used with the R package of the same name for Arch Linux. (Thank you Jeroen for the name that makes it so tricky to know what one is talking about! :) ) To prevent breaking changes in the upstream R package from affecting users, I maintained a rigorous weekly workflow:

1. **Build:** Compiling the latest available V8 tag.
2. **Test:** Verifying that the R package `V8` remained operational (and providing upstream fixes when necessary).
3. **Deploy:** Pushing the tested commits to the AUR.
4. **Distribute:** Providing the binary package in a custom Arch Linux repository.

Over the course of six years and roughly 250 commits, this project has been a rewarding journey in C++, Docker, and the Arch Linux packaging ecosystem. I am grateful for the 10 AUR votes, 8 GitHub stars, and the community engagement provided via helpful feedback received in online discussions along the way.

### Status & Handover
**This is the final regular update for the `v8-r` package.** Out of respect for the security and trust developed over the last six years, I do not want to leave the package unmaintained for general pickup. To ensure the best interests of the users are protected, I am seeking a **controlled handover**. 

If you are interested in taking over development, please reach out via email. I am open to a period of co-maintainership to ensure a smooth transition while I phase out my involvement.
