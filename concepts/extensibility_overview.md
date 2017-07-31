<span data-ttu-id="a612b-p116">特定のリソース上の拡張機能データに対して読み書きするには、そのリソースに対して読み書きするときに必要となるのと同じ[アクセス許可](./permissions_reference.md)が必要になります。たとえば、サインイン済みのユーザーのプロファイルをカスタム アプリ データで更新できるようにするには、アプリに *User.ReadWrite.All* アクセス許可を付与しておく必要があります。</span><span class="sxs-lookup"><span data-stu-id="a612b-p116">The same [permissions](./permissions_reference.md) that are required to read from or write to a specific resource are also required to read from or write to any extensions data on that resource.  For example, for an app to be able to update the signed-in user's profile with custom app data, the app must have been granted the *User.ReadWrite.All* permission.</span></span>

特定のリソース上の拡張機能データに対して読み書きするには、そのリソースに対して読み書きするときに必要となるのと同じ[アクセス許可](./permissions_reference.md)が必要になります。たとえば、サインイン済みのユーザーのプロファイルをカスタム アプリ データで更新できるようにするには、アプリに *User.ReadWrite.All* アクセス許可を付与しておく必要があります。

<span data-ttu-id="a612b-229">また、スキーマ拡張機能の定義を作成および管理できるようにするには、アプリケーションに *Directory.AccessAsUser.All* アクセス許可を付与しておく必要があります。</span><span class="sxs-lookup"><span data-stu-id="a612b-229">Additionally, to create and manage schema extension definitions, an application must be granted the *Directory.AccessAsUser.All* permission.</span></span>

## <a name="data-limits"></a><span data-ttu-id="a612b-230">データの上限</span><span class="sxs-lookup"><span data-stu-id="a612b-230">Data limits</span></span>

### <a name="open-extension-limits"></a><span data-ttu-id="a612b-231">オープン拡張機能の上限</span><span class="sxs-lookup"><span data-stu-id="a612b-231">Open extension limits</span></span>
<span data-ttu-id="a612b-232">以下に示す上限がディレクトリ リソース (**ユーザー**、**グループ**、**デバイス**など) に適用されます。</span><span class="sxs-lookup"><span data-stu-id="a612b-232">The following limits apply to directory resources (such as **user**, **group**, **device**):</span></span>

- <span data-ttu-id="a612b-233">オープン拡張機能のデータの上限は 2 KB (拡張機能の定義自体を含む) です。</span><span class="sxs-lookup"><span data-stu-id="a612b-233">Each open extension can have up to 2KB of data (including the extension definition itself).</span></span>
- <span data-ttu-id="a612b-234">アプリケーションでは、リソース インスタンスごとに最大 2 つのオープン拡張機能を追加できます。</span><span class="sxs-lookup"><span data-stu-id="a612b-234">An application can add up to two open extensions per resource instance.</span></span>

### <a name="schema-extension-limits"></a><span data-ttu-id="a612b-235">スキーマ拡張機能の上限</span><span class="sxs-lookup"><span data-stu-id="a612b-235">Schema extension limits</span></span>
<span data-ttu-id="a612b-236">アプリケーションで作成できる**スキーマ拡張機能**の定義は最大 5 つです。</span><span class="sxs-lookup"><span data-stu-id="a612b-236">An application may create no more than five **schema extension** definitions.</span></span>

## <a name="known-limitations"></a><span data-ttu-id="a612b-237">既知の制限</span><span class="sxs-lookup"><span data-stu-id="a612b-237">Known limitations</span></span>

<span data-ttu-id="a612b-238">拡張機能の使用に関する既知の制限については、既知の問題に関する記事の[「拡張機能」セクション](known_issues.md#extensions)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a612b-238">For known limitations using extensions, see the [extensions section](known_issues.md#extensions) in the known issues article.</span></span>

## <a name="extension-examples"></a><span data-ttu-id="a612b-239">拡張機能の例</span><span class="sxs-lookup"><span data-stu-id="a612b-239">Extension examples</span></span>

[<span data-ttu-id="a612b-240">オープン拡張機能を使用したユーザーへのカスタム データの追加</span><span class="sxs-lookup"><span data-stu-id="a612b-240">Add custom data to users using open extensions</span></span>](extensibility_open_users.md)

[<span data-ttu-id="a612b-241">スキーマ拡張機能を使用したグループへのカスタム データの追加</span><span class="sxs-lookup"><span data-stu-id="a612b-241">Add custom data to groups using schema extensions</span></span>](extensibility_schema_groups.md)

## <a name="see-also"></a><span data-ttu-id="a612b-242">関連項目</span><span class="sxs-lookup"><span data-stu-id="a612b-242">See also</span></span>

[<span data-ttu-id="a612b-243">Office 365 のドメイン</span><span class="sxs-lookup"><span data-stu-id="a612b-243">Office 365 domains</span></span>](https://technet.microsoft.com/en-us/library/office-365-domains.aspx)

[<span data-ttu-id="a612b-244">Office 365 テナントのドメインの追加および検証</span><span class="sxs-lookup"><span data-stu-id="a612b-244">Adding and verifying a domain for an Office 365 tenant</span></span>](http://office365support.ca/adding-and-verifying-a-domain-for-the-new-office-365/)
