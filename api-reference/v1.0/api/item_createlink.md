<span data-ttu-id="aecfc-p110">リンクの種類で `embed` を使用する場合、返される webUrl は `<iframe>` HTML 要素に埋め込むことができます。埋め込みリンクが作成されると、`webHtml` プロパティに `<iframe>` がコンテンツをホストするための HTML コードが含まれます。</span><span class="sxs-lookup"><span data-stu-id="aecfc-p110">When using the `embed` link type, the webUrl returned can be embedded in an `<iframe>` HTML element. When an embed link is created the `webHtml` property contains the HTML code for an `<iframe>` to host the content.</span></span>

リンクの種類で `embed` を使用する場合、返される webUrl は `<iframe>` HTML 要素に埋め込むことができます。埋め込みリンクが作成されると、`webHtml` プロパティに `<iframe>` がコンテンツをホストするための HTML コードが含まれます。

<span data-ttu-id="aecfc-164">**注:**埋め込みリンクは **driveType** が `personal` である[ドライブ](../resources/drive.md)でのみ、サポートされます。</span><span class="sxs-lookup"><span data-stu-id="aecfc-164">**Note:** Embed links are only supported in [Drives](../resources/drive.md) where the **driveType** is `personal`.</span></span>

## <span data-ttu-id="aecfc-165">注釈</span><span class="sxs-lookup"><span data-stu-id="aecfc-165">Remarks</span></span>
<a id="remarks" class="xliff"></a>

* <span data-ttu-id="aecfc-166">組織に既定の有効期限ポリシーが適用されている場合を除き、このアクションを使用して作成されたリンクに期限はありません。</span><span class="sxs-lookup"><span data-stu-id="aecfc-166">Links created using this action do not expire unless a default expiration policy is enforced for the organization.</span></span>
* <span data-ttu-id="aecfc-167">リンクはそのアイテムの共有アクセス許可に表示され、アイテムの所有者はそれを削除できます。</span><span class="sxs-lookup"><span data-stu-id="aecfc-167">Links are visible in the sharing permissions for the item and can be removed by an owner of the item.</span></span>
* <span data-ttu-id="aecfc-168">リンクは、そのアイテムがチェックアウトされない限り、常にアイテムの現在のバージョンをポイントします (SharePoint の場合のみ)。</span><span class="sxs-lookup"><span data-stu-id="aecfc-168">Links always point to the current version of a item unless the item is checked out (SharePoint only).</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "item: createLink",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Item/Create sharing link"
} -->
