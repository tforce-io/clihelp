---
title: Adduser
type: docs
bookToC: false
---

NPM-ADDUSER(1)                                                                                                                                                                                       NPM-ADDUSER(1)

NAME
       npm-adduser - Add a registry user account

   Synopsis
         npm adduser

         alias: add-user

       Note: This command is unaware of workspaces.

   Description
       Create a new user in the specified registry, and save the credentials to the .npmrc file. If no registry is specified, the default registry will be used (see npm help registry).

       When using legacy for your auth-type, the username, password, and email are read in from prompts.

   Configuration
   registry
       •   Default: "https://registry.npmjs.org/"

       •   Type: URL

       The base URL of the npm registry.

   scope
       •   Default: the scope of the current project, if any, or ""

       •   Type: String

       Associate an operation with a scope for a scoped registry.

       Useful when logging in to or out of a private registry:

         # log in, linking the scope to the custom registry
         npm login --scope=@mycorp --registry=https://registry.mycorp.com

         # log out, removing the link and the auth token
         npm logout --scope=@mycorp

       This will cause @mycorp to be mapped to the registry for future installation of packages specified according to the pattern @mycorp/package.

       This will also cause npm init to create a scoped package.

         # accept all defaults, and create a package named "@foo/whatever",
         # instead of just named "whatever"
         npm init --scope=@foo --yes

   auth-type
       •   Default: "web"

       •   Type: "legacy" or "web"

       What authentication strategy to use with login. Note that if an otp config is given, this value will always be set to legacy.

   See Also
       •   npm help registry

       •   npm help config

       •   npm help npmrc

       •   npm help owner

       •   npm help whoami

       •   npm help token

       •   npm help profile

NPM@10.8.2                                                                                           July 2024                                                                                       NPM-ADDUSER(1)
