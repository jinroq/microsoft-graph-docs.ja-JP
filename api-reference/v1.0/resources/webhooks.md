<span data-ttu-id="a8a9f-p119">Microsoft Graph への応答で、`202 - Accepted` ステータス コードを送信します。Microsoft Graph が 2xx クラス コードを受信しない場合は、通知の再送信を何回でも再試行します。</span><span class="sxs-lookup"><span data-stu-id="a8a9f-p119">Send a `202 - Accepted` status code in your response to Microsoft Graph. If Microsoft Graph doesn't receive a 2xx class code, it will retry resending the notification a number of times.</span></span>
3. Microsoft Graph への応答で、`202 - Accepted` ステータス コードを送信します。Microsoft Graph が 2xx クラス コードを受信しない場合は、通知の再送信を何回でも再試行します。
  > <span data-ttu-id="a8a9f-198">clientState プロパティがサブスクリプション要求のものと一致しない場合でも、`202 - Accepted` ステータス コードを送信する必要があります。</span><span class="sxs-lookup"><span data-stu-id="a8a9f-198">You should send a `202 - Accepted` status code even if the clientState property doesn't match the one submitted with the subscription request.</span></span>

<span data-ttu-id="a8a9f-199">要求内の他の通知について、これらを繰り返します。</span><span class="sxs-lookup"><span data-stu-id="a8a9f-199">Repeat for other notifications in the request.</span></span>

# <span data-ttu-id="a8a9f-200">その他の技術情報</span><span class="sxs-lookup"><span data-stu-id="a8a9f-200">Additional resources</span></span>
<a id="additional-resources" class="xliff"></a>

* [<span data-ttu-id="a8a9f-201">サブスクリプション リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a8a9f-201">Subscription resource type</span></span>](subscription.md)
* [<span data-ttu-id="a8a9f-202">サブスクリプションを取得する</span><span class="sxs-lookup"><span data-stu-id="a8a9f-202">Get subscription</span></span>](../api/subscription_get.md)
* [<span data-ttu-id="a8a9f-203">サブスクリプションを作成する</span><span class="sxs-lookup"><span data-stu-id="a8a9f-203">Create subscription</span></span>](../api/subscription_post_subscriptions.md)
* [<span data-ttu-id="a8a9f-204">Node.js 用 Microsoft Graph Webhooks のサンプル</span><span class="sxs-lookup"><span data-stu-id="a8a9f-204">Microsoft Graph Webhooks Sample for Node.js</span></span>](https://github.com/OfficeDev/Microsoft-Graph-Nodejs-Webhooks)
* [<span data-ttu-id="a8a9f-205">ASP.NET 用 Microsoft Graph Webhooks のサンプル</span><span class="sxs-lookup"><span data-stu-id="a8a9f-205">Microsoft Graph Webhooks Sample for ASP.NET</span></span>](https://github.com/OfficeDev/Microsoft-Graph-ASPNET-Webhooks)
