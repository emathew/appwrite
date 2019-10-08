Use this endpoint to let user accept an invitation to join a team after he is being redirect back to your app from the invitation email. Use the success and failure URL's to redirect users back to your application after the request completes.

Please notice that in order to avoid a [Redirect Attacks](https://github.com/OWASP/CheatSheetSeries/blob/master/cheatsheets/Unvalidated_Redirects_and_Forwards_Cheat_Sheet.md) the only valid redirect URL's are the once from domains you have set when added your platforms in the console interface.

When not using the success or failure redirect arguments this endpoint will result with a 200 status code on success and with 401 status error on failure. This behavior was applied to help the web clients deal with browsers who don't allow to set 3rd party HTTP cookies needed for saving the account session token.