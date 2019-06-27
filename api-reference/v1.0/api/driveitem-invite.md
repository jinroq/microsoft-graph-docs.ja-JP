---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: アイテムにアクセスするための招待状を送信する
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 37e2bc8a383f5078c413ccc37f369442f55b597c
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35272864"
---
# <a name="send-a-sharing-invitation"></a><span data-ttu-id="48199-102">共有の招待状を送信する</span><span class="sxs-lookup"><span data-stu-id="48199-102">Send a sharing invitation</span></span>

<span data-ttu-id="48199-103">**ドライブ項目**の共有への招待を送信します。</span><span class="sxs-lookup"><span data-stu-id="48199-103">Sends a sharing invitation for a **DriveItem**.</span></span>
<span data-ttu-id="48199-104">共有への招待では、受信者にアクセス許可が与えられ、必要に応じて[共有リンク][]を使用して電子メールを送信します。</span><span class="sxs-lookup"><span data-stu-id="48199-104">A sharing invitation provides permissions to the recipients and optionally sends them an email with a [sharing link][].</span></span>

## <a name="permissions"></a><span data-ttu-id="48199-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="48199-105">Permissions</span></span>

<span data-ttu-id="48199-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="48199-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="48199-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="48199-108">Permission type</span></span>      | <span data-ttu-id="48199-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="48199-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="48199-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="48199-110">Delegated (work or school account)</span></span> | <span data-ttu-id="48199-111">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48199-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="48199-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="48199-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="48199-113">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48199-113">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="48199-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="48199-114">Application</span></span> | <span data-ttu-id="48199-115">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48199-115">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="48199-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="48199-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{drive-id}/items/{item-id}/invite
POST /groups/{group-id}/drive/items/{item-id}/invite
POST /me/drive/items/{item-id}/invite
POST /sites/{siteId}/drive/items/{itemId}/invite
POST /users/{userId}/drive/items/{itemId}/invite
```

## <a name="request-body"></a><span data-ttu-id="48199-117">要求本文</span><span class="sxs-lookup"><span data-stu-id="48199-117">Request body</span></span>

<span data-ttu-id="48199-118">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="48199-118">In the request body, provide a JSON object with the following parameters.</span></span>

<!-- { "blockType": "ignored", "scopes": "files.readwrite" } -->

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

| <span data-ttu-id="48199-119">パラメーター</span><span class="sxs-lookup"><span data-stu-id="48199-119">Parameter</span></span>        | <span data-ttu-id="48199-120">型</span><span class="sxs-lookup"><span data-stu-id="48199-120">Type</span></span>                           | <span data-ttu-id="48199-121">説明</span><span class="sxs-lookup"><span data-stu-id="48199-121">Description</span></span>
|:-----------------|:-------------------------------|:-------------------------
| <span data-ttu-id="48199-122">Recipients</span><span class="sxs-lookup"><span data-stu-id="48199-122">recipients</span></span>       | <span data-ttu-id="48199-123">Collection([DriveRecipient][])</span><span class="sxs-lookup"><span data-stu-id="48199-123">Collection([DriveRecipient][])</span></span> | <span data-ttu-id="48199-124">アクセスおよび共有の招待状を受信する、受信者のコレクション。</span><span class="sxs-lookup"><span data-stu-id="48199-124">A collection of recipients who will receive access and the sharing invitation.</span></span>
| <span data-ttu-id="48199-125">message</span><span class="sxs-lookup"><span data-stu-id="48199-125">message</span></span>          | <span data-ttu-id="48199-126">String</span><span class="sxs-lookup"><span data-stu-id="48199-126">String</span></span>                         | <span data-ttu-id="48199-p103">共有の招待状に含まれるプレーンテキスト形式のメッセージ。最大の長さは 2000 文字です。</span><span class="sxs-lookup"><span data-stu-id="48199-p103">A plain text formatted message that is included in the sharing invitation. Maximum length 2000 characters.</span></span>
| <span data-ttu-id="48199-129">requireSignIn</span><span class="sxs-lookup"><span data-stu-id="48199-129">requireSignIn</span></span>    | <span data-ttu-id="48199-130">Boolean</span><span class="sxs-lookup"><span data-stu-id="48199-130">Boolean</span></span>                        | <span data-ttu-id="48199-131">共有アイテムを表示するために、招待状の受信者がサインインする必要があるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="48199-131">Specifies whether the recipient of the invitation is required to sign-in to view the shared item.</span></span>
| <span data-ttu-id="48199-132">sendInvitation</span><span class="sxs-lookup"><span data-stu-id="48199-132">sendInvitation</span></span>   | <span data-ttu-id="48199-133">ブール値</span><span class="sxs-lookup"><span data-stu-id="48199-133">Boolean</span></span>                        | <span data-ttu-id="48199-134">True の場合、[共有リンク][]は受信者に送信されます。</span><span class="sxs-lookup"><span data-stu-id="48199-134">If true, a [sharing link][] is sent to the recipient.</span></span> <span data-ttu-id="48199-135">それ以外の場合は、通知を送信することなく、直接アクセス許可が付与されます。</span><span class="sxs-lookup"><span data-stu-id="48199-135">Otherwise, a permission is granted directly without sending a notification.</span></span>
| <span data-ttu-id="48199-136">roles</span><span class="sxs-lookup"><span data-stu-id="48199-136">roles</span></span>            | <span data-ttu-id="48199-137">Collection(String)</span><span class="sxs-lookup"><span data-stu-id="48199-137">Collection(String)</span></span>             | <span data-ttu-id="48199-138">共有への招待の受信者に付与する役割を指定します。</span><span class="sxs-lookup"><span data-stu-id="48199-138">Specify the roles that are to be granted to the recipients of the sharing invitation.</span></span>

## <a name="example"></a><span data-ttu-id="48199-139">例</span><span class="sxs-lookup"><span data-stu-id="48199-139">Example</span></span>

<span data-ttu-id="48199-140">この例では、電子メールアドレスが "ryan@contoso.com" のユーザーに、共同作業中のファイルに関するメッセージを含む共有への招待を送信します。</span><span class="sxs-lookup"><span data-stu-id="48199-140">This example sends a sharing invitation to a user with email address "ryan@contoso.com" with a message about a file being collaborated on.</span></span>
<span data-ttu-id="48199-141">この招待により、Ryan にはファイルへの読み取り/書き込みアクセス権が付与されます。</span><span class="sxs-lookup"><span data-stu-id="48199-141">The invitation grants Ryan read-write access to the file.</span></span>

### <a name="http-request"></a><span data-ttu-id="48199-142">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="48199-142">HTTP Request</span></span>

<span data-ttu-id="48199-143">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で[アクセス許可](../resources/permission.md)コレクション オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="48199-143">If successful, this method returns `200 OK` response code and [permission](../resources/permission.md) collection object in the response body.</span></span>

<!-- { "blockType": "request", "name": "send-sharing-invite", "scopes": "files.readwrite", "target": "action" } -->

```json
POST /me/drive/items/{item-id}/invite
Content-type: application/json

{
  "recipients": [
    {
      "email": "ryan@contoso.com"
    }
  ],
  "message": "Here's the file that we're collaborating on.",
  "requireSignIn": true,
  "sendInvitation": true,
  "roles": [ "write" ]
}
```

### <a name="response"></a><span data-ttu-id="48199-144">応答</span><span class="sxs-lookup"><span data-stu-id="48199-144">Response</span></span>

<span data-ttu-id="48199-145">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="48199-145">Here is an example of the response.</span></span>

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.permission)", "truncated": true } -->

```json
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="48199-146">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="48199-146">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="48199-147">C#</span><span class="sxs-lookup"><span data-stu-id="48199-147">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/send-sharing-invite-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="48199-148">Javascript</span><span class="sxs-lookup"><span data-stu-id="48199-148">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/send-sharing-invite-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="48199-149">目的-C</span><span class="sxs-lookup"><span data-stu-id="48199-149">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/send-sharing-invite-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="remarks"></a><span data-ttu-id="48199-150">備考</span><span class="sxs-lookup"><span data-stu-id="48199-150">Remarks</span></span>

* <span data-ttu-id="48199-151">`personal` (OneDrive 個人用) の **driveType** を持つ[ドライブ](../resources/drive.md)は、ルートの DriveItem でアクセス許可を作成したり、変更したりすることはできません。</span><span class="sxs-lookup"><span data-stu-id="48199-151">[Drives](../resources/drive.md) with a **driveType** of `personal` (OneDrive personal) cannot create or modify permissions on the root DriveItem.</span></span>
* <span data-ttu-id="48199-152">使用可能なロールの一覧は、「[ロール列挙](../resources/permission.md#roles-enumeration)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="48199-152">For a list of available roles, see [Roles enumeration](../resources/permission.md#roles-enumeration).</span></span>

## <a name="error-responses"></a><span data-ttu-id="48199-153">エラー応答</span><span class="sxs-lookup"><span data-stu-id="48199-153">Error Responses</span></span>

<span data-ttu-id="48199-154">エラーがどのような形で返されるかについては、「[エラー応答][error-response]」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="48199-154">Read the [Error Responses][error-response] topic for more information about how errors are returned.</span></span>


[driveRecipient]: ../resources/driverecipient.md
[error-response]: /graph/errors
[共有リンク]: ../resources/permission.md#sharing-links
[sharing link]: ../resources/permission.md#sharing-links

<!-- {
  "type": "#page.annotation",
  "description": "Add permissions to an item and optionally send a sharing notification.",
  "keywords": "retrieve,item,metadata",
  "section": "documentation",
  "tocPath": "Sharing/Add permissions",
  "suppressions": [
    "Error: /api-reference/v1.0/api/driveitem-invite.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/driveitem-invite.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/driveitem-invite.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
} -->
