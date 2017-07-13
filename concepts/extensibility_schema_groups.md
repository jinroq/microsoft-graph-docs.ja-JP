<span data-ttu-id="a0c33-p109">次の例では、`graphlearn_courses` の拡張機能と `123` に一致する `courseId` のプロパティ値を有するグループを検索し、`graphlearn_courses` 拡張機能のグループのプロパティ、**displayName**、**ID**、**説明**、カスタム データを取得します。(実際のクエリでは、必要に応じて URL エンコードを行ってください。)</span><span class="sxs-lookup"><span data-stu-id="a0c33-p109">The following example looks for the group that has the `graphlearn_courses` extension with a `courseId` property value matching `123`, and gets the group properties **displayName**, **id**, and **description**, and the custom data in the `graphlearn_courses` extension. (In the actual query, make sure you apply URL encoding as necessary.)</span></span>

次の例では、`graphlearn_courses` の拡張機能と `123` に一致する `courseId` のプロパティ値を有するグループを検索し、`graphlearn_courses` 拡張機能のグループのプロパティ、**displayName**、**ID**、**説明**、カスタム データを取得します。(実際のクエリでは、必要に応じて URL エンコードを行ってください。)

#### <span data-ttu-id="a0c33-157">要求</span><span class="sxs-lookup"><span data-stu-id="a0c33-157">Request</span></span>
<a id="request" class="xliff"></a>

```http
GET https://graph.microsoft.com/v1.0/groups?$filter=graphlearn_courses/courseId eq ‘123’&$select=displayName,id,description,graphlearn_courses
```


##### <span data-ttu-id="a0c33-158">応答</span><span class="sxs-lookup"><span data-stu-id="a0c33-158">Response</span></span>
<a id="response" class="xliff"></a>
```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-length: 326
{
  "value": [
    {
      "displayName": "New Managers March 2017",
      "id": "14429ae5-3e74-41a2-9fa8-028fbb984637",
      "description": "New Managers training course for March 2017",
      "graphlearn_courses": {
        "@odata.type": "#microsoft.graph.ComplexExtensionValue",
        "courseId":"123",
        "courseName":"New Managers",
        "courseType":"Online"
      }
    }
  ]
}
```

## <span data-ttu-id="a0c33-159">関連項目</span><span class="sxs-lookup"><span data-stu-id="a0c33-159">See also</span></span>
<a id="see-also" class="xliff"></a>

- [<span data-ttu-id="a0c33-160">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="a0c33-160">Add custom data to resources using extensions</span></span>](extensibility_overview.md)
- [<span data-ttu-id="a0c33-161">オープン拡張機能を使用したユーザーへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="a0c33-161">Add custom data to users using open extensions (preview)</span></span>](extensibility_open_users.md)
- <span data-ttu-id="a0c33-162">
  [Office 365 のドメイン](https://technet.microsoft.com/en-us/library/office-365-domains.aspx)</span><span class="sxs-lookup"><span data-stu-id="a0c33-162">[Office 365 domains](https://technet.microsoft.com/en-us/library/office-365-domains.aspx)</span></span>
- [<span data-ttu-id="a0c33-163">新しい Office 365 のドメインの追加および検証</span><span class="sxs-lookup"><span data-stu-id="a0c33-163">Adding and Verifying a Domain for the NEW Office 365</span></span>](http://office365support.ca/adding-and-verifying-a-domain-for-the-new-office-365/)
- [<span data-ttu-id="a0c33-164">schemaExtension リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="a0c33-164">schemaExtension resource type</span></span>](../api-reference/v1.0/resources/schemaextension.md)
- [<span data-ttu-id="a0c33-165">schemaExtensions を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="a0c33-165">List schemaExtensions</span></span>](../api-reference/v1.0/api/schemaextension_list.md)
- [<span data-ttu-id="a0c33-166">schemaExtension を作成する</span><span class="sxs-lookup"><span data-stu-id="a0c33-166">Create schemaExtension</span></span>](../api-reference/v1.0/api/schemaextension_post_schemaextensions.md)
- [<span data-ttu-id="a0c33-167">schemaExtension を取得する</span><span class="sxs-lookup"><span data-stu-id="a0c33-167">Get schemaExtension</span></span>](../api-reference/v1.0/api/schemaextension_get.md)
- [<span data-ttu-id="a0c33-168">schemaExtension を更新する</span><span class="sxs-lookup"><span data-stu-id="a0c33-168">Update schemaExtension</span></span>](../api-reference/v1.0/api/schemaextension_update.md)
- [<span data-ttu-id="a0c33-169">schemaExtension を削除する</span><span class="sxs-lookup"><span data-stu-id="a0c33-169">Delete schemaExtension</span></span>](../api-reference/v1.0/api/schemaextension_delete.md)
