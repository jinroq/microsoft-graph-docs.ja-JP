---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: アイテムにアクセスするために招待状を送信する
ms.openlocfilehash: 3dc4d4a9c06b5e969476da2aa842db51f61346b2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068652"
---
# <a name="send-a-sharing-invitation"></a><span data-ttu-id="7f812-102">共有の招待状を送信する</span><span class="sxs-lookup"><span data-stu-id="7f812-102">Send a sharing invitation</span></span>

> <span data-ttu-id="7f812-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="7f812-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7f812-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7f812-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7f812-p102">**DriveItem** の共有の招待状を送信します。共有の招待状は受信者にアクセス許可を提供します。また、任意で受信者に、アイテムが共有されたことを通知する電子メールを送信します。</span><span class="sxs-lookup"><span data-stu-id="7f812-p102">Sends a sharing invitation for a **DriveItem**. A sharing invitation provides permissions to the recipients and optionally sends an email to the recipients to notify them the item was shared.</span></span>

## <a name="permissions"></a><span data-ttu-id="7f812-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="7f812-107">Permissions</span></span>

<span data-ttu-id="7f812-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7f812-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7f812-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7f812-110">Permission type</span></span>      | <span data-ttu-id="7f812-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="7f812-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7f812-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7f812-112">Delegated (work or school account)</span></span> | <span data-ttu-id="7f812-113">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f812-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="7f812-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7f812-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7f812-115">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f812-115">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="7f812-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7f812-116">Application</span></span> | <span data-ttu-id="7f812-117">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f812-117">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7f812-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7f812-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{drive-id}/items/{item-id}/invite
POST /groups/{group-id}/drive/items/{item-id}/invite
POST /me/drive/items/{item-id}/invite
POST /sites/{siteId}/drive/items/{itemId}/invite
POST /users/{userId}/drive/items/{itemId}/invite
```

## <a name="request-body"></a><span data-ttu-id="7f812-119">要求本文</span><span class="sxs-lookup"><span data-stu-id="7f812-119">Request body</span></span>

<span data-ttu-id="7f812-120">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="7f812-120">In the request body, provide a JSON object with the following parameters.</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.inviteParameters", "scopes": "files.readwrite" } -->

```json
{
  "requireSignIn": false,
  "sendInvitation": false,
  "roles": [ "read | write"],
  "recipients": [
    { "@odata.type": "microsoft.graph.driveRecipient" },
    { "@odata.type": "microsoft.graph.driveRecipient" }
  ],
  "message": "string"
}
```

| <span data-ttu-id="7f812-121">パラメーター</span><span class="sxs-lookup"><span data-stu-id="7f812-121">Parameter</span></span>        | <span data-ttu-id="7f812-122">型</span><span class="sxs-lookup"><span data-stu-id="7f812-122">Type</span></span>                                            | <span data-ttu-id="7f812-123">説明</span><span class="sxs-lookup"><span data-stu-id="7f812-123">Description</span></span>                                                                                                |
|:-----------------|:------------------------------------------------|:-----------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="7f812-124">Recipients</span><span class="sxs-lookup"><span data-stu-id="7f812-124">recipients</span></span>       | <span data-ttu-id="7f812-125">Collection([DriveRecipient](../resources/driverecipient.md))</span><span class="sxs-lookup"><span data-stu-id="7f812-125">Collection([DriveRecipient](../resources/driverecipient.md))</span></span> | <span data-ttu-id="7f812-126">アクセスおよび共有の招待状を受信する、受信者のコレクション。</span><span class="sxs-lookup"><span data-stu-id="7f812-126">A collection of recipients who will receive access and the sharing invitation.</span></span>                                            |
| <span data-ttu-id="7f812-127">message</span><span class="sxs-lookup"><span data-stu-id="7f812-127">message</span></span>          | <span data-ttu-id="7f812-128">String</span><span class="sxs-lookup"><span data-stu-id="7f812-128">String</span></span>                                          | <span data-ttu-id="7f812-p104">共有の招待状に含まれるプレーンテキスト形式のメッセージ。最大の長さは 2000 文字です。</span><span class="sxs-lookup"><span data-stu-id="7f812-p104">A plain text formatted message that is included in the sharing invitation. Maximum length 2000 characters.</span></span> |
| <span data-ttu-id="7f812-131">requireSignIn</span><span class="sxs-lookup"><span data-stu-id="7f812-131">requireSignIn</span></span>    | <span data-ttu-id="7f812-132">ブール値</span><span class="sxs-lookup"><span data-stu-id="7f812-132">Boolean</span></span>                                         | <span data-ttu-id="7f812-133">共有アイテムを表示するために、招待状の受信者がサインインする必要のある場所を指定します。</span><span class="sxs-lookup"><span data-stu-id="7f812-133">Specifies where the recipient of the invitation is required to sign-in to view the shared item.</span></span>            |
| <span data-ttu-id="7f812-134">sendInvitation</span><span class="sxs-lookup"><span data-stu-id="7f812-134">sendInvitation</span></span>   | <span data-ttu-id="7f812-135">ブール値</span><span class="sxs-lookup"><span data-stu-id="7f812-135">Boolean</span></span>                                         | <span data-ttu-id="7f812-136">電子メールまたは投稿が生成されるのか (false)、アクセス許可のみが作成されるのか (true) を指定します。</span><span class="sxs-lookup"><span data-stu-id="7f812-136">Specifies if an email or post is generated (false) or if the permission is just created (true).</span></span>            |
| <span data-ttu-id="7f812-137">roles</span><span class="sxs-lookup"><span data-stu-id="7f812-137">roles</span></span>            | <span data-ttu-id="7f812-138">Collection(String)</span><span class="sxs-lookup"><span data-stu-id="7f812-138">Collection(String)</span></span>                              | <span data-ttu-id="7f812-139">共有の招待状の受信者に付与されるロールを指定します。</span><span class="sxs-lookup"><span data-stu-id="7f812-139">Specify the roles that are be granted to the recipients of the sharing invitation.</span></span>                         |

## <a name="example"></a><span data-ttu-id="7f812-140">例</span><span class="sxs-lookup"><span data-stu-id="7f812-140">Example</span></span>

<span data-ttu-id="7f812-141">この例では、"ryan@contoso.org" というメール アドレスを持つユーザーに共有の招待状を、共同作業中のファイルについてのメッセージと共に送信します。</span><span class="sxs-lookup"><span data-stu-id="7f812-141">This example sends a sharing invitation to a user with email address "ryan@contoso.org" with a message about a file being collaborated on.</span></span>
<span data-ttu-id="7f812-142">この招待により、Ryan にはファイルへの読み取り/書き込みアクセス権が付与されます。</span><span class="sxs-lookup"><span data-stu-id="7f812-142">The invitation grants Ryan read-write access to the file.</span></span>

### <a name="http-request"></a><span data-ttu-id="7f812-143">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7f812-143">HTTP Request</span></span>

<span data-ttu-id="7f812-144">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で[アクセス許可](../resources/permission.md)コレクション オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="7f812-144">If successful, this method returns `200 OK` response code and [permission](../resources/permission.md) collection object in the response body.</span></span>

<!-- { "blockType": "request", "name": "send-sharing-invite", "@odata.type": "microsoft.graph.inviteParameters", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /me/drive/items/{item-id}/invite
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

### <a name="response"></a><span data-ttu-id="7f812-145">応答</span><span class="sxs-lookup"><span data-stu-id="7f812-145">Response</span></span>

<span data-ttu-id="7f812-146">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="7f812-146">Here is an example of the response.</span></span>

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.permission)", "truncated": true } -->

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

## <a name="remarks"></a><span data-ttu-id="7f812-147">備考</span><span class="sxs-lookup"><span data-stu-id="7f812-147">Remarks</span></span>

* <span data-ttu-id="7f812-148">`personal` (OneDrive 個人用) の **driveType** を持つ[ドライブ](../resources/drive.md)は、ルートの DriveItem でアクセス許可を作成したり、変更したりすることはできません。</span><span class="sxs-lookup"><span data-stu-id="7f812-148">[Drives](../resources/drive.md) with a **driveType** of `personal` (OneDrive personal) cannot create or modify permissions on the root DriveItem.</span></span>
* <span data-ttu-id="7f812-149">使用可能なロールの一覧は、「[ロール列挙](../resources/permission.md#roles-enumeration-values)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7f812-149">For a list of available roles, see [Roles enumeration](../resources/permission.md#roles-enumeration-values).</span></span>

## <a name="error-responses"></a><span data-ttu-id="7f812-150">エラー応答</span><span class="sxs-lookup"><span data-stu-id="7f812-150">Error Responses</span></span>

<span data-ttu-id="7f812-151">エラーがどのような形で返されるかについては、「[エラー応答][error-response]」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7f812-151">Read the [Error Responses][error-response] topic for more information about how errors are returned.</span></span>


[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Add permissions to an item and optionally send a sharing notification.",
  "keywords": "retrieve,item,metadata",
  "section": "documentation",
  "tocPath": "Sharing/Add permissions"
} -->
