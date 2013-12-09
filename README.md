Add ABC MimeType
================

This demontrates how to enable any file extension support in Azure WebSites.

  1. Clone this repository.
  2. Run `build.cmd`.  This will zip the extension files in `artifacts\Release\zip` folder.
  3. Copy `Deployment Trigger Url` from Azure portal for your website (in CONFIGURE TAB).
  4. Upload extension to your website by `artifacts\Release\zip\DeployExtension.cmd "<deploy-trigger-url>"`.
  5. Enable private extension by adding an AppSetting `WEBSITE_PRIVATE_EXTENSIONS = 1` to your website.
  6. You can now try to access your file with `.abc` extension.

That's it.
  
