% GUI Customization

You can modify some display features of the Rundeck GUI by setting
these properties in the [rundeck-config.properties](configuration-file-reference.html#rundeck-config.properties) file:

-------------------------------------------------------------------------------

| **Property**  | **Description**  | **Example** |
| - | - | - |
| `rundeck.gui.logo`                          | Requires staticUserResources to be enabled. Sets the user's logo (e.g. company/org logo) on the login, logout pages and in the header of the application | 'rundeck.png' |
| `rundeck.gui.logoSmall`                     | Requires staticUserResources to be enabled. Sets a small user's logo (e.g. company/org logo) to be used in place of the larger logo in the header of the application. | 'rundeck.small.png' |
| `rundeck.gui.sidebarColor`                  | Sets the background color of the navigation sidebar. | '#2910f8' |
| `rundeck.gui.sidebarTextColor`              | Sets the text color of the navigation sidebar.  | '#fffdfa' |
| `rundeck.gui.sidebarTextActiveColor`        | Sets the active text/link color of the navigation sidebar. | '#000000' |
| `rundeck.gui.instanceName`                  | Sets the instance name | 'Ops Management Console> Prod', 'Ops Staging' |
| `rundeck.gui.instanceNameLabelColor`        | Sets the instance label color | '#2910f8' |
| `rundeck.gui.instanceNameLabelTextColor`    | Sets the instance label text color | '#64fe31' |
| `rundeck.gui.title`                         | Title shown in app header | Test App |
| `rundeck.gui.staticUserResources.enabled`   | Enable serving static files from $RDECK_BASE/user-assets dir. This must be set to true if using a custom logo. | true |
| `rundeck.gui.paginatejobs.enabled`          | Paginate job list when listing project jobs | true |                                  
| `rundeck.gui.paginatejobs.max.per.page`     | Number of jobs per page to display when job pagination is enabled | true |
| `rundeck.gui.titleLink`                     | URL for the link used by the app header icon. | http://rundeck.org |
| `rundeck.gui.helpLink`                      | URL for the "help" link in the app header.  | http://rundeck.org/docs |
| `rundeck.gui.realJobTree`                   | Displaying a real tree in the Jobs overview instead of collapsing empty groups. | false **Default: true** |
| `rundeck.gui.startpage`                     | Change the default page shown after choosing a project. Values: 'adhoc', 'configure', 'createJob', 'events', 'home', 'jobs', 'nodes', 'projectHome' or 'uploadJob'. | **Default: 'projectHome'** |
| `rundeck.gui.execution.tail.lines.default`  | Change the default number of lines shown in the execution page in tail mode view. | **Default: 20** |
| `rundeck.gui.execution.tail.lines.max`      | Change the maximum number of lines shown in the execution page in tail mode view. | **Default: 100** |
| `rundeck.gui.enableJobHoverInfo`            | Shows job information when the user hovers over a job name in various   pages.| **Default: true** |
| `rundeck.gui.login.welcome`                 | Text displayed in the login form pages. | **Default: blank** |
| `rundeck.gui.login.welcomeHtml`             | HTML displayed in the login form pages. The HTML will be sanitized before display. | **Default: blank** |
| `rundeck.gui.login.footerMessageHtml`       | HTML displayed in the login form| pages (below the login form). The HTML will be sanitized before display. | **Default:blank** |
| `rundeck.gui.errorpage.hidestacktrace`      | Hide Java stacktraces from the end   true/false user when an error occurs. | **Default: false**|
| `rundeck.gui.job.description.disableHTML`   | Disable extended Job description true/false and Option description rendering as HTML. | **Default: false**|
| `rundeck.gui.clusterIdentityInHeader`       | When cluster mode is enabled, true/false display server name/ID in header.| **Default: false** |
| `rundeck.gui.clusterIdentityInFooter`       | When cluster mode is enabled, true/false display server name/ID in footer.| **Default: true** |

-------------------------------------------------------------------------------

The `rundeck.gui.errorpage.hidestacktrace` can also be set to true via a Java system property defined at system startup:
`-Dorg.rundeck.gui.errorpage.hidestacktrace=true`.

## Localization

See [Localization](localization.html).
