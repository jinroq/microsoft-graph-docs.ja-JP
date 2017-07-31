<span data-ttu-id="b2752-p119">これで、Microsoft Graph を呼び出す方法が理解できたため、API リファレンスを使用して、アプリで必要なその他の呼び出しを作成することができます。ただしアプリでは、呼び出しを行うための適切なアクセス許可をアプリ登録で設定する必要がある点に注意してください。</span><span class="sxs-lookup"><span data-stu-id="b2752-p119">Now that you've seen how to make calls to Microsoft Graph, you can use the API reference to construct any other kinds of calls your app needs to make. However, bear in mind that your app needs to have the appropriate permissions configured on the app registration for the calls it makes.</span></span>

```
GET https://graph.microsoft.com/v1.0/me/messages?$select=subject,from,receivedDateTime&$top=25&$orderby=receivedDateTime%20DESC
Accept: application/json
Authorization: Bearer eyJ0eXAi...b66LoPVA
```

これで、Microsoft Graph を呼び出す方法が理解できたため、API リファレンスを使用して、アプリで必要なその他の呼び出しを作成することができます。ただしアプリでは、呼び出しを行うための適切なアクセス許可をアプリ登録で設定する必要がある点に注意してください。

## <a name="next-steps"></a><span data-ttu-id="b2752-189">次の手順</span><span class="sxs-lookup"><span data-stu-id="b2752-189">Next steps</span></span>
- <span data-ttu-id="b2752-190">[Graph エクスプローラー](https://graph.microsoft.io/graph-explorer)を使用してさらに REST API を試してみる。</span><span class="sxs-lookup"><span data-stu-id="b2752-190">Try out more of the REST API using the [Graph explorer](https://graph.microsoft.io/graph-explorer).</span></span>

## <a name="see-also"></a><span data-ttu-id="b2752-191">関連項目</span><span class="sxs-lookup"><span data-stu-id="b2752-191">See also</span></span>
- [<span data-ttu-id="b2752-192">Azure AD v2.0 のプロトコル</span><span class="sxs-lookup"><span data-stu-id="b2752-192">Azure AD v2.0 protocols</span></span>](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-protocols/)
- [<span data-ttu-id="b2752-193">Azure AD v2.0 のトークン</span><span class="sxs-lookup"><span data-stu-id="b2752-193">Azure AD v2.0 tokens</span></span>](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-tokens/)
