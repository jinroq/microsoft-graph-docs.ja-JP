# <a name="send-a-sharing-invitation"></a><span data-ttu-id="4f4f4-101">共有の招待状を送信する</span><span class="sxs-lookup"><span data-stu-id="4f4f4-101">Send a sharing invitation</span></span>

<span data-ttu-id="4f4f4-p101">**DriveItem** の共有の招待状を送信します。共有の招待状は受信者にアクセス許可を提供します。また、任意で受信者に、アイテムが共有されたことを通知する電子メールを送信します。</span><span class="sxs-lookup"><span data-stu-id="4f4f4-p101">Sends a sharing invitation for a **DriveItem**. A sharing invitation provides permissions to the recipients and optionally sends an email to the recipients to notify them the item was shared.</span></span>

## <a name="permissions"></a><span data-ttu-id="4f4f4-104">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="4f4f4-104">Permissions</span></span>
<span data-ttu-id="4f4f4-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4f4f4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="4f4f4-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4f4f4-107">Permission type</span></span>      | <span data-ttu-id="4f4f4-108">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="4f4f4-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4f4f4-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4f4f4-109">Delegated (work or school account)</span></span> | <span data-ttu-id="4f4f4-110">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f4f4-110">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="4f4f4-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4f4f4-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4f4f4-112">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f4f4-112">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="4f4f4-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4f4f4-113">Application</span></span> | <span data-ttu-id="4f4f4-114">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f4f4-114">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4f4f4-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4f4f4-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{item-id}/invite
POST /drive/items/{item-id}/invite
POST /drives/{drive-id}/items/{item-id}/invite
POST /groups/{group-id}/drive/items/{item-id}/invite
```

## <a name="request-body"></a><span data-ttu-id="4f4f4-116">要求本文</span><span class="sxs-lookup"><span data-stu-id="4f4f4-116">Request body</span></span>
<span data-ttu-id="4f4f4-117">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="4f4f4-117">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="4f4f4-118">パラメーター</span><span class="sxs-lookup"><span data-stu-id="4f4f4-118">Parameter</span></span>        | <span data-ttu-id="4f4f4-119">型</span><span class="sxs-lookup"><span data-stu-id="4f4f4-119">Type</span></span>                                            | <span data-ttu-id="4f4f4-120">説明</span><span class="sxs-lookup"><span data-stu-id="4f4f4-120">Description</span></span>                                                                                                |
|:-----------------|:------------------------------------------------|:-----------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="4f4f4-121">Recipients</span><span class="sxs-lookup"><span data-stu-id="4f4f4-121">recipients</span></span>       | <span data-ttu-id="4f4f4-122">Collection([DriveRecipient](../resources/driverecipient.md))</span><span class="sxs-lookup"><span data-stu-id="4f4f4-122">Collection([DriveRecipient](../resources/driverecipient.md))</span></span> | <span data-ttu-id="4f4f4-123">アクセスおよび共有の招待状を受信する、受信者のコレクション。</span><span class="sxs-lookup"><span data-stu-id="4f4f4-123">A collection of recipients who will receive access and the sharing invitation.</span></span>                                            |
| <span data-ttu-id="4f4f4-124">message</span><span class="sxs-lookup"><span data-stu-id="4f4f4-124">message</span></span>          | <span data-ttu-id="4f4f4-125">String</span><span class="sxs-lookup"><span data-stu-id="4f4f4-125">String</span></span>                                          | <span data-ttu-id="4f4f4-p103">共有の招待状に含まれるプレーンテキスト形式のメッセージ。最大の長さは 2000 文字です。</span><span class="sxs-lookup"><span data-stu-id="4f4f4-p103">A plain text formatted message that is included in the sharing invitation. Maximum length 2000 characters.</span></span> |
| <span data-ttu-id="4f4f4-128">requireSignIn</span><span class="sxs-lookup"><span data-stu-id="4f4f4-128">requireSignIn</span></span>    | <span data-ttu-id="4f4f4-129">Boolean</span><span class="sxs-lookup"><span data-stu-id="4f4f4-129">Boolean</span></span>                                         | <span data-ttu-id="4f4f4-130">共有アイテムを表示するために、招待状の受信者がサインインする必要のある場所を指定します。</span><span class="sxs-lookup"><span data-stu-id="4f4f4-130">Specifies where the recipient of the invitation is required to sign-in to view the shared item.</span></span>            |
| <span data-ttu-id="4f4f4-131">sendInvitation</span><span class="sxs-lookup"><span data-stu-id="4f4f4-131">sendInvitation</span></span>   | <span data-ttu-id="4f4f4-132">Boolean</span><span class="sxs-lookup"><span data-stu-id="4f4f4-132">Boolean</span></span>                                         | <span data-ttu-id="4f4f4-133">電子メールまたは投稿が生成されるのか (false)、アクセス許可のみが作成されるのか (true) を指定します。</span><span class="sxs-lookup"><span data-stu-id="4f4f4-133">Specifies if an email or post is generated (false) or if the permission is just created (true).</span></span>            |
| <span data-ttu-id="4f4f4-134">roles</span><span class="sxs-lookup"><span data-stu-id="4f4f4-134">roles</span></span>            | <span data-ttu-id="4f4f4-135">Collection(String)</span><span class="sxs-lookup"><span data-stu-id="4f4f4-135">Collection(String)</span></span>                              | <span data-ttu-id="4f4f4-136">共有の招待状の受信者に付与されるロールを指定します。</span><span class="sxs-lookup"><span data-stu-id="4f4f4-136">Specify the roles that are be granted to the recipients of the sharing invitation.</span></span>                         |

## <a name="response"></a><span data-ttu-id="4f4f4-137">応答</span><span class="sxs-lookup"><span data-stu-id="4f4f4-137">Response</span></span>

<span data-ttu-id="4f4f4-138">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で[アクセス許可](../resources/permission.md)コレクション オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="4f4f4-138">If successful, this method returns `200 OK` response code and [permission](../resources/permission.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4f4f4-139">例</span><span class="sxs-lookup"><span data-stu-id="4f4f4-139">Example</span></span>
<span data-ttu-id="4f4f4-140">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="4f4f4-140">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="4f4f4-141">要求</span><span class="sxs-lookup"><span data-stu-id="4f4f4-141">Request</span></span>
<span data-ttu-id="4f4f4-142">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4f4f4-142">Here is an example of the request.</span></span>

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

##### <a name="response"></a><span data-ttu-id="4f4f4-143">応答</span><span class="sxs-lookup"><span data-stu-id="4f4f4-143">Response</span></span>
<span data-ttu-id="4f4f4-144">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="4f4f4-144">Here is an example of the response.</span></span>
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

## <a name="remarks"></a><span data-ttu-id="4f4f4-145">備考</span><span class="sxs-lookup"><span data-stu-id="4f4f4-145">Remarks</span></span>

* <span data-ttu-id="4f4f4-146">`personal` (OneDrive Personal) の **driveType** を持つ[ドライブ](../resources/drive.md)は、ルートの DriveItem でアクセス許可を作成したり、変更したりすることはできません。</span><span class="sxs-lookup"><span data-stu-id="4f4f4-146">[Drives](../resources/drive.md) with a **driveType** of `personal` (OneDrive Personal) cannot create or modify permissions on the root DriveItem.</span></span> 
* <span data-ttu-id="4f4f4-147">使用可能なロールの一覧は、「[ロール列挙](../resources/permission.md#roles-enumeration)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4f4f4-147">For a list of available roles, see [Roles enumeration](../resources/permission.md#roles-enumeration).</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!-- {
  "type": "#page.annotation",
  "description": "item: invite",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
