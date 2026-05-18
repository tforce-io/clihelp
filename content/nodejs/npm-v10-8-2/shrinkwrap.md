---
title: Shrinkwrap
type: docs
bookToC: false
---

NPM-SHRINKWRAP(1)                                                                                                                                                                                 NPM-SHRINKWRAP(1)

NAME
       npm-shrinkwrap - Lock down dependency versions for publication

   Synopsis
         npm shrinkwrap

       Note: This command is unaware of workspaces.

   Description
       This command repurposes package-lock.json into a publishable npm-shrinkwrap.json or simply creates a new one. The file created and updated by this command will then take precedence over any other existing
       or future package-lock.json files. For a detailed explanation of the design and purpose of package locks in npm, see npm help package-lock-json.

   See Also
       •   npm help install

       •   npm help run-script

       •   npm help scripts

       •   package.json ⟨/configuring-npm/package-json⟩

       •   package-lock.json ⟨/configuring-npm/package-lock-json⟩

       •   npm-shrinkwrap.json ⟨/configuring-npm/npm-shrinkwrap-json⟩

       •   npm help ls

NPM@10.8.2                                                                                           July 2024                                                                                    NPM-SHRINKWRAP(1)
