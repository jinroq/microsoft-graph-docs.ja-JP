<span data-ttu-id="598f4-p107">ローミング プロファイルがもはや不要であるとユーザーが判断する場合、削除できます。オープン拡張機能の値で ```DELETE``` 要求を使用して行えます。</span><span class="sxs-lookup"><span data-stu-id="598f4-p107">The user decides that they don't want a roaming profile anymore, so they delete it. This can be done with a ```DELETE``` request on the open extension value.</span></span>
ローミング プロファイルがもはや不要であるとユーザーが判断する場合、削除できます。オープン拡張機能の値で ```DELETE``` 要求を使用して行えます。

##### <a name="request"></a><span data-ttu-id="598f4-135">要求</span><span class="sxs-lookup"><span data-stu-id="598f4-135">Request</span></span>
```http
DELETE https://graph.microsoft.com/v1.0/me/extensions/com.contoso.roamingSettings
```

##### <a name="response"></a><span data-ttu-id="598f4-136">応答</span><span class="sxs-lookup"><span data-stu-id="598f4-136">Response</span></span>
```
HTTP/1.1 204 No content
```

## <a name="see-also"></a><span data-ttu-id="598f4-137">関連項目</span><span class="sxs-lookup"><span data-stu-id="598f4-137">See also</span></span>

- [<span data-ttu-id="598f4-138">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="598f4-138">Add custom data to resources using extensions</span></span>](extensibility_overview.md)
- [<span data-ttu-id="598f4-139">スキーマ拡張機能を使用したグループへのカスタム データの追加</span><span class="sxs-lookup"><span data-stu-id="598f4-139">Add custom data to groups using schema extensions</span></span>](extensibility_schema_groups.md)
- [<span data-ttu-id="598f4-140">openTypeExtension リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="598f4-140">openTypeExtension resource type</span></span>](../api-reference/v1.0/resources/opentypeextension.md)
- [<span data-ttu-id="598f4-141">オープン拡張機能を作成する</span><span class="sxs-lookup"><span data-stu-id="598f4-141">Create open extension</span></span>](../api-reference/v1.0/api/opentypeextension_post_opentypeextension.md)
- [<span data-ttu-id="598f4-142">オープン拡張機能を取得する</span><span class="sxs-lookup"><span data-stu-id="598f4-142">Get open extension</span></span>](../api-reference/v1.0/api/opentypeextension_get.md)
- [<span data-ttu-id="598f4-143">オープン拡張機能を更新する</span><span class="sxs-lookup"><span data-stu-id="598f4-143">Update open extension</span></span>](../api-reference/v1.0/api/opentypeextension_update.md)
- [<span data-ttu-id="598f4-144">オープン拡張機能を削除する</span><span class="sxs-lookup"><span data-stu-id="598f4-144">Delete open extension</span></span>](../api-reference/v1.0/api/opentypeextension_delete.md)