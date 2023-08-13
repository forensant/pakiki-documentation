# Match/replace

It is possible to modify requests/responses as they are in transit to/from the browser automatically. These modifications will be taken into account before they are sent from any areas of the proxy.

Many bug bounty programs require that specific headers are sent with each request, this can be used to ensure that happens.

<!-- tabs:start -->

#### **Linux**

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="../_media/Linux/Dark/MatchReplace.png">
  <img alt="Match/Replace" src="../_media/Linux/Light/MatchReplace.png">
</picture>

#### **MacOS**

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="../_media/Mac/Dark/MatchReplace.png">
  <img alt="Match/Replace" src="../_media/Mac/Light/MatchReplace.png">
</picture>

<!-- tabs:end -->

The following types of actions can be taken:
  * Adding headers
  * Modifying headers
  * Modifying a request/response's body

Matches are done with regular expressions, and the match/replace rules are executed in-order.

Match/Replace can be accessed via the Project Options from the top right-hand three bar/hamburger menu on Linux, or via Match/Replace on the left-hand sidebar on MacOS.