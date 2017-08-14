<span data-ttu-id="a1716-p102">共有の招待状に含まれるプレーンテキスト形式のメッセージ。最大の長さは 2000 文字です。</span><span class="sxs-lookup"><span data-stu-id="a1716-p102">A plain text formatted message that is included in the sharing invitation. Maximum length 2000 characters.</span></span>                                          | 共有の招待状に含まれるプレーンテキスト形式のメッセージ。最大の長さは 2000 文字です。 |
| <span data-ttu-id="a1716-122">requireSignIn</span><span class="sxs-lookup"><span data-stu-id="a1716-122">requireSignIn</span></span>    | <span data-ttu-id="a1716-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="a1716-123">Boolean</span></span>                                         | <span data-ttu-id="a1716-124">共有アイテムを表示するために、招待状の受信者がサインインする必要のある場所を指定します。</span><span class="sxs-lookup"><span data-stu-id="a1716-124">Specifies where the recipient of the invitation is required to sign-in to view the shared item.</span></span>            |
| <span data-ttu-id="a1716-125">sendInvitation</span><span class="sxs-lookup"><span data-stu-id="a1716-125">sendInvitation</span></span>   | <span data-ttu-id="a1716-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="a1716-126">Boolean</span></span>                                         | <span data-ttu-id="a1716-127">電子メールまたは投稿が生成されるのか (false)、アクセス許可のみが作成されるのか (true) を指定します。</span><span class="sxs-lookup"><span data-stu-id="a1716-127">Specifies if an email or post is generated (false) or if the permission is just created (true).</span></span>            |
| <span data-ttu-id="a1716-128">roles</span><span class="sxs-lookup"><span data-stu-id="a1716-128">roles</span></span>            | <span data-ttu-id="a1716-129">Collection(String)</span><span class="sxs-lookup"><span data-stu-id="a1716-129">Collection(String)</span></span>                              | <span data-ttu-id="a1716-130">共有の招待状の受信者に付与されるロールを指定します。</span><span class="sxs-lookup"><span data-stu-id="a1716-130">Specify the roles that are be granted to the recipients of the sharing invitation.</span></span>                         |

## <a name="response"></a><span data-ttu-id="a1716-131">応答</span><span class="sxs-lookup"><span data-stu-id="a1716-131">Response</span></span>

<span data-ttu-id="a1716-132">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で[アクセス許可](../resources/permission.md)コレクション オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="a1716-132">If successful, this method returns `200 OK` response code and [permission](../resources/permission.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a1716-133">例</span><span class="sxs-lookup"><span data-stu-id="a1716-133">Example</span></span>
<span data-ttu-id="a1716-134">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="a1716-134">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="a1716-135">要求</span><span class="sxs-lookup"><span data-stu-id="a1716-135">Request</span></span>
<span data-ttu-id="a1716-136">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a1716-136">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "item_invite"
}-->
```http
POST https://graph.microsoft.com/v1.0/drive/items/{item-id}/invite
Content-type: application/json

{
  "recipients": [
    {
      "email": "ryan@contoso.org"
    }
  ],
  "message": "Here's the file that we're collaborating on.",
  "requireSignIn": true,
  "sendInvitation": true,
  "roles": [ "write" ]
}
```

##### <a name="response"></a><span data-ttu-id="a1716-137">応答</span><span class="sxs-lookup"><span data-stu-id="a1716-137">Response</span></span>
<span data-ttu-id="a1716-138">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="a1716-138">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.permission",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "grantedTo": {
        "user": {
          "displayName": "Ryan Gregg",
          "id": "42F177F1-22C0-4BE3-900D-4507125C5C20"
        }
      },
      "id": "CCFC7CA3-7A19-4D57-8CEF-149DB9DDFA62",
      "invitation": {
        "email": "ryan@contoso.com",
        "signInRequired": true
      },
      "roles": [ "write" ]
    }
  ]
}
```

## <a name="remarks"></a><span data-ttu-id="a1716-139">備考</span><span class="sxs-lookup"><span data-stu-id="a1716-139">Remarks</span></span>

* <span data-ttu-id="a1716-140">`personal` (OneDrive Personal) の **driveType** を持つ[ドライブ](../resources/drive.md)は、ルートの DriveItem でアクセス許可を作成したり、変更したりすることはできません。</span><span class="sxs-lookup"><span data-stu-id="a1716-140">[Drives](../resources/drive.md) with a **driveType** of `personal` (OneDrive Personal) cannot create or modify permissions on the root DriveItem.</span></span> 
* <span data-ttu-id="a1716-141">使用可能なロールの一覧は、「[ロール列挙](../resources/permission.md#roles-enumeration)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a1716-141">For a list of available roles, see [Roles enumeration](../resources/permission.md#roles-enumeration).</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!-- {
  "type": "#page.annotation",
  "description": "item: invite",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
