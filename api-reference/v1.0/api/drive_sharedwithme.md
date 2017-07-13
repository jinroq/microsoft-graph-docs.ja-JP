<span data-ttu-id="43d9c-p103">**sharedWithMe** アクションから返された DriveItems には、それらが異なるドライブからのアイテムであることを示す [**remoteItem**](../resources/remoteitem.md) ファセットが必ず含まれます。共有された DriveItem リソースにアクセスするには、**remoteItem** で提供された情報を使用して、以下に示す書式で要求を作成する必要があります。</span><span class="sxs-lookup"><span data-stu-id="43d9c-p103">DriveItems returned from the **sharedWithMe** action will always include the [**remoteItem**](../resources/remoteitem.md) facet which indicates they are items from a different drive. To access the shared DriveItem resource, you will need to make a request using the information provided in **remoteItem** in the following format:</span></span>

**sharedWithMe** アクションから返された DriveItems には、それらが異なるドライブからのアイテムであることを示す [**remoteItem**](../resources/remoteitem.md) ファセットが必ず含まれます。共有された DriveItem リソースにアクセスするには、**remoteItem** で提供された情報を使用して、以下に示す書式で要求を作成する必要があります。

<!-- {"blockType": "ignored"} -->
```http
GET https://graph.microsoft.com/v1.0/drives/{remoteItem.parentReference.driveId}/items/{remoteItem.id}
```

<!-- {
  "type": "#page.annotation",
  "description": "Retrieve a list of files shared with the signed-in user.",
  "keywords": "sharedWithMe onedrive shared files",
  "section": "documentation",
  "tocPath": "OneDrive/Drive/Shared with me"
} -->
