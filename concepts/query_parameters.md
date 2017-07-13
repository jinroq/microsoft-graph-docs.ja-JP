<span data-ttu-id="a06c8-p117">検索条件は、高度な検索テクニック (AQS) を使用して表現されます。結果は、メッセージが送信された日時で並べ替えられます。</span><span class="sxs-lookup"><span data-stu-id="a06c8-p117">Search criteria are expressed using Advanced Query Syntax (AQS). The results are sorted by the date and time that the message was sent.</span></span>

検索条件は、高度な検索テクニック (AQS) を使用して表現されます。結果は、メッセージが送信された日時で並べ替えられます。

<span data-ttu-id="a06c8-194">`$search` で `message` に対する次のプロパティを指定できます: `attachments`、`bccRecipients`、`body`、`category`、`ccRecipients`、`content`、`from`、`hasAttachments`、`participants`、`receivedDateTime`、`sender`、`subject`、`toRecipients`</span><span class="sxs-lookup"><span data-stu-id="a06c8-194">You can specify the following properties on a `message` in a `$search` criterion: `attachments`, `bccRecipients`, `body`, `category`, `ccRecipients`, `content`, `from`, `hasAttachments`, `participants`, `receivedDateTime`, `sender`, `subject`, `toRecipients`</span></span>

<span data-ttu-id="a06c8-195">メッセージで検索を行うときに値のみ指定した場合、検索は既定の検索プロパティである `from`、`subject` および `body` に基づいて行われます。</span><span class="sxs-lookup"><span data-stu-id="a06c8-195">If you do a search on messages and specify only a value, the search is carried out on the default search properties of `from`, `subject` and `body`.</span></span>

<span data-ttu-id="a06c8-196">次の例は、サインイン中のユーザーの受信トレイにあるメッセージのうち、既定の 3 つの検索プロパティのいずれかに "pizza" が含まれるメッセージをすべて返します。</span><span class="sxs-lookup"><span data-stu-id="a06c8-196">The following example returns all messages in the signed-in user's Inbox that contains "pizza" in any of the three default search properties:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$search="pizza"
```

<span data-ttu-id="a06c8-197">次の例は、ユーザーの受信トレイにあるメッセージのうち、特定のメール アドレスから送信されたメッセージをすべて検索します。</span><span class="sxs-lookup"><span data-stu-id="a06c8-197">The next example searches all messages in the user's Inbox that were sent from a specific email address:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/messages?$search="from:help@contoso.com"
```

[graph-explorer]: https://graph.microsoft.io/en-us/graph-explorer
[odata-filter]: http://docs.oasis-open.org/odata/odata/v4.0/errata03/os/complete/part2-url-conventions/odata-v4.0-errata03-os-part2-url-conventions-complete.html#_Toc453752358
[odata-query]: http://docs.oasis-open.org/odata/odata/v4.0/errata03/os/complete/part2-url-conventions/odata-v4.0-errata03-os-part2-url-conventions-complete.html#_Toc453752356
