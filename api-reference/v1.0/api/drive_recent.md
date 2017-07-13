<span data-ttu-id="11658-p103">**recent** アクションから返された DriveItems の中には、それらが異なるドライブからのアイテムであることを示す **remoteItem** ファセットが含まれるものがあります。元の DriveItem オブジェクトにアクセスするには、**remoteItem** で提供された情報を使用して、以下に示す書式で要求を作成する必要があります。</span><span class="sxs-lookup"><span data-stu-id="11658-p103">Some driveItems returned from the **recent** action will include the **remoteItem** facet which indicates they are items from another drive. To access the original driveItem object, you will need to make a request using the information provided in **remoteItem** in the following format:</span></span>

**recent** アクションから返された DriveItems の中には、それらが異なるドライブからのアイテムであることを示す **remoteItem** ファセットが含まれるものがあります。元の DriveItem オブジェクトにアクセスするには、**remoteItem** で提供された情報を使用して、以下に示す書式で要求を作成する必要があります。

<!-- {"blockType": "ignored"} -->
```http
GET https://graph.microsoft.com/v1.0/drives/{remoteItem.driveId}/items/{remoteItem.id}
```

<!-- {
  "type": "#page.annotation",
  "description": "Retrieve a list of files shared with the signed-in user.",
  "keywords": "sharedWithMe onedrive shared files",
  "section": "documentation",
  "tocPath": "OneDrive/Drive/Shared with me"
} -->
