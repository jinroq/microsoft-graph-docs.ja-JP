---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: アイテムにアクセスするための招待状を送信する
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: cc88297c1848e9b66195f9a07ac96167d096a762
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/08/2019
ms.locfileid: "30481210"
---
# <a name="send-a-sharing-invitation"></a><span data-ttu-id="6bb56-102">共有の招待状を送信する</span><span class="sxs-lookup"><span data-stu-id="6bb56-102">Send a sharing invitation</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6bb56-p101">**DriveItem** の共有の招待状を送信します。共有の招待状は受信者にアクセス許可を提供します。また、任意で受信者に、アイテムが共有されたことを通知する電子メールを送信します。</span><span class="sxs-lookup"><span data-stu-id="6bb56-p101">Sends a sharing invitation for a **DriveItem**. A sharing invitation provides permissions to the recipients and optionally sends an email to the recipients to notify them the item was shared.</span></span>

## <a name="permissions"></a><span data-ttu-id="6bb56-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="6bb56-105">Permissions</span></span>

<span data-ttu-id="6bb56-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6bb56-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6bb56-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6bb56-108">Permission type</span></span>      | <span data-ttu-id="6bb56-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="6bb56-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6bb56-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6bb56-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6bb56-111">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6bb56-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="6bb56-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6bb56-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6bb56-113">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6bb56-113">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="6bb56-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6bb56-114">Application</span></span> | <span data-ttu-id="6bb56-115">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6bb56-115">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6bb56-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6bb56-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{drive-id}/items/{item-id}/invite
POST /groups/{group-id}/drive/items/{item-id}/invite
POST /me/drive/items/{item-id}/invite
POST /sites/{siteId}/drive/items/{itemId}/invite
POST /users/{userId}/drive/items/{itemId}/invite
```

## <a name="request-body"></a><span data-ttu-id="6bb56-117">要求本文</span><span class="sxs-lookup"><span data-stu-id="6bb56-117">Request body</span></span>

<span data-ttu-id="6bb56-118">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="6bb56-118">In the request body, provide a JSON object with the following parameters.</span></span>

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

| <span data-ttu-id="6bb56-119">パラメーター</span><span class="sxs-lookup"><span data-stu-id="6bb56-119">Parameter</span></span>        | <span data-ttu-id="6bb56-120">型</span><span class="sxs-lookup"><span data-stu-id="6bb56-120">Type</span></span>                                            | <span data-ttu-id="6bb56-121">説明</span><span class="sxs-lookup"><span data-stu-id="6bb56-121">Description</span></span>                                                                                                |
|:-----------------|:------------------------------------------------|:-----------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="6bb56-122">Recipients</span><span class="sxs-lookup"><span data-stu-id="6bb56-122">recipients</span></span>       | <span data-ttu-id="6bb56-123">Collection([DriveRecipient](../resources/driverecipient.md))</span><span class="sxs-lookup"><span data-stu-id="6bb56-123">Collection([DriveRecipient](../resources/driverecipient.md))</span></span> | <span data-ttu-id="6bb56-124">アクセスおよび共有の招待状を受信する、受信者のコレクション。</span><span class="sxs-lookup"><span data-stu-id="6bb56-124">A collection of recipients who will receive access and the sharing invitation.</span></span>                                            |
| <span data-ttu-id="6bb56-125">message</span><span class="sxs-lookup"><span data-stu-id="6bb56-125">message</span></span>          | <span data-ttu-id="6bb56-126">String</span><span class="sxs-lookup"><span data-stu-id="6bb56-126">String</span></span>                                          | <span data-ttu-id="6bb56-p103">共有の招待状に含まれるプレーンテキスト形式のメッセージ。最大の長さは 2000 文字です。</span><span class="sxs-lookup"><span data-stu-id="6bb56-p103">A plain text formatted message that is included in the sharing invitation. Maximum length 2000 characters.</span></span> |
| <span data-ttu-id="6bb56-129">requireSignIn</span><span class="sxs-lookup"><span data-stu-id="6bb56-129">requireSignIn</span></span>    | <span data-ttu-id="6bb56-130">ブール型</span><span class="sxs-lookup"><span data-stu-id="6bb56-130">Boolean</span></span>                                         | <span data-ttu-id="6bb56-131">共有アイテムを表示するために、招待状の受信者がサインインする必要のある場所を指定します。</span><span class="sxs-lookup"><span data-stu-id="6bb56-131">Specifies where the recipient of the invitation is required to sign-in to view the shared item.</span></span>            |
| <span data-ttu-id="6bb56-132">sendInvitation</span><span class="sxs-lookup"><span data-stu-id="6bb56-132">sendInvitation</span></span>   | <span data-ttu-id="6bb56-133">ブール値</span><span class="sxs-lookup"><span data-stu-id="6bb56-133">Boolean</span></span>                                         | <span data-ttu-id="6bb56-134">電子メールまたは投稿が生成されるのか (false)、アクセス許可のみが作成されるのか (true) を指定します。</span><span class="sxs-lookup"><span data-stu-id="6bb56-134">Specifies if an email or post is generated (false) or if the permission is just created (true).</span></span>            |
| <span data-ttu-id="6bb56-135">roles</span><span class="sxs-lookup"><span data-stu-id="6bb56-135">roles</span></span>            | <span data-ttu-id="6bb56-136">Collection(String)</span><span class="sxs-lookup"><span data-stu-id="6bb56-136">Collection(String)</span></span>                              | <span data-ttu-id="6bb56-137">共有の招待状の受信者に付与されるロールを指定します。</span><span class="sxs-lookup"><span data-stu-id="6bb56-137">Specify the roles that are be granted to the recipients of the sharing invitation.</span></span>                         |

## <a name="example"></a><span data-ttu-id="6bb56-138">例</span><span class="sxs-lookup"><span data-stu-id="6bb56-138">Example</span></span>

<span data-ttu-id="6bb56-139">この例では、"ryan@contoso.org" というメール アドレスを持つユーザーに共有の招待状を、共同作業中のファイルについてのメッセージと共に送信します。</span><span class="sxs-lookup"><span data-stu-id="6bb56-139">This example sends a sharing invitation to a user with email address "ryan@contoso.org" with a message about a file being collaborated on.</span></span>
<span data-ttu-id="6bb56-140">この招待により、Ryan にはファイルへの読み取り/書き込みアクセス権が付与されます。</span><span class="sxs-lookup"><span data-stu-id="6bb56-140">The invitation grants Ryan read-write access to the file.</span></span>

### <a name="http-request"></a><span data-ttu-id="6bb56-141">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6bb56-141">HTTP Request</span></span>

<span data-ttu-id="6bb56-142">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で[アクセス許可](../resources/permission.md)コレクション オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="6bb56-142">If successful, this method returns `200 OK` response code and [permission](../resources/permission.md) collection object in the response body.</span></span>

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

### <a name="response"></a><span data-ttu-id="6bb56-143">応答</span><span class="sxs-lookup"><span data-stu-id="6bb56-143">Response</span></span>

<span data-ttu-id="6bb56-144">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="6bb56-144">Here is an example of the response.</span></span>

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

## <a name="remarks"></a><span data-ttu-id="6bb56-145">備考</span><span class="sxs-lookup"><span data-stu-id="6bb56-145">Remarks</span></span>

* <span data-ttu-id="6bb56-146">`personal` (OneDrive 個人用) の **driveType** を持つ[ドライブ](../resources/drive.md)は、ルートの DriveItem でアクセス許可を作成したり、変更したりすることはできません。</span><span class="sxs-lookup"><span data-stu-id="6bb56-146">[Drives](../resources/drive.md) with a **driveType** of `personal` (OneDrive personal) cannot create or modify permissions on the root DriveItem.</span></span>
* <span data-ttu-id="6bb56-147">使用可能なロールの一覧は、「[ロール列挙](../resources/permission.md#roles-enumeration-values)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6bb56-147">For a list of available roles, see [Roles enumeration](../resources/permission.md#roles-enumeration-values).</span></span>

## <a name="error-responses"></a><span data-ttu-id="6bb56-148">エラー応答</span><span class="sxs-lookup"><span data-stu-id="6bb56-148">Error Responses</span></span>

<span data-ttu-id="6bb56-149">エラーがどのような形で返されるかについては、「[エラー応答][error-response]」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6bb56-149">Read the [Error Responses][error-response] topic for more information about how errors are returned.</span></span>


[error-response]: /graph/errors

<!--
{
  "type": "#page.annotation",
  "description": "Add permissions to an item and optionally send a sharing notification.",
  "keywords": "retrieve,item,metadata",
  "section": "documentation",
  "tocPath": "Sharing/Add permissions",
  "suppressions": [
    "Error: /api-reference/beta/api/driveitem-invite.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
