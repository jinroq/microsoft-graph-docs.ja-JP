---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: アイテムにアクセスするために招待状を送信する
ms.openlocfilehash: db089fcd0a3f948d8e43f366a4e6674c2505fa2d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27021172"
---
# <a name="send-a-sharing-invitation"></a><span data-ttu-id="be5c3-102">共有の招待状を送信する</span><span class="sxs-lookup"><span data-stu-id="be5c3-102">Send a sharing invitation</span></span>

<span data-ttu-id="be5c3-103">の**DriveItem**の共有への招待を送信します。</span><span class="sxs-lookup"><span data-stu-id="be5c3-103">Sends a sharing invitation for a **DriveItem**.</span></span>
<span data-ttu-id="be5c3-104">共有への招待は、受信者へのアクセス許可を提供し、オプションで[リンクを共有][]して電子メールを送信します。</span><span class="sxs-lookup"><span data-stu-id="be5c3-104">A sharing invitation provides permissions to the recipients and optionally sends them an email with a [sharing link][].</span></span>

## <a name="permissions"></a><span data-ttu-id="be5c3-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="be5c3-105">Permissions</span></span>

<span data-ttu-id="be5c3-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="be5c3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="be5c3-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="be5c3-108">Permission type</span></span>      | <span data-ttu-id="be5c3-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="be5c3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="be5c3-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="be5c3-110">Delegated (work or school account)</span></span> | <span data-ttu-id="be5c3-111">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be5c3-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="be5c3-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="be5c3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="be5c3-113">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be5c3-113">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="be5c3-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="be5c3-114">Application</span></span> | <span data-ttu-id="be5c3-115">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be5c3-115">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="be5c3-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="be5c3-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{drive-id}/items/{item-id}/invite
POST /groups/{group-id}/drive/items/{item-id}/invite
POST /me/drive/items/{item-id}/invite
POST /sites/{siteId}/drive/items/{itemId}/invite
POST /users/{userId}/drive/items/{itemId}/invite
```

## <a name="request-body"></a><span data-ttu-id="be5c3-117">要求本文</span><span class="sxs-lookup"><span data-stu-id="be5c3-117">Request body</span></span>

<span data-ttu-id="be5c3-118">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="be5c3-118">In the request body, provide a JSON object with the following parameters.</span></span>

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

| <span data-ttu-id="be5c3-119">パラメーター</span><span class="sxs-lookup"><span data-stu-id="be5c3-119">Parameter</span></span>        | <span data-ttu-id="be5c3-120">型</span><span class="sxs-lookup"><span data-stu-id="be5c3-120">Type</span></span>                           | <span data-ttu-id="be5c3-121">説明</span><span class="sxs-lookup"><span data-stu-id="be5c3-121">Description</span></span>
|:-----------------|:-------------------------------|:-------------------------
| <span data-ttu-id="be5c3-122">Recipients</span><span class="sxs-lookup"><span data-stu-id="be5c3-122">recipients</span></span>       | <span data-ttu-id="be5c3-123">Collection([DriveRecipient][])</span><span class="sxs-lookup"><span data-stu-id="be5c3-123">Collection([DriveRecipient][])</span></span> | <span data-ttu-id="be5c3-124">アクセスおよび共有の招待状を受信する、受信者のコレクション。</span><span class="sxs-lookup"><span data-stu-id="be5c3-124">A collection of recipients who will receive access and the sharing invitation.</span></span>
| <span data-ttu-id="be5c3-125">message</span><span class="sxs-lookup"><span data-stu-id="be5c3-125">message</span></span>          | <span data-ttu-id="be5c3-126">String</span><span class="sxs-lookup"><span data-stu-id="be5c3-126">String</span></span>                         | <span data-ttu-id="be5c3-p103">共有の招待状に含まれるプレーンテキスト形式のメッセージ。最大の長さは 2000 文字です。</span><span class="sxs-lookup"><span data-stu-id="be5c3-p103">A plain text formatted message that is included in the sharing invitation. Maximum length 2000 characters.</span></span>
| <span data-ttu-id="be5c3-129">requireSignIn</span><span class="sxs-lookup"><span data-stu-id="be5c3-129">requireSignIn</span></span>    | <span data-ttu-id="be5c3-130">ブール値</span><span class="sxs-lookup"><span data-stu-id="be5c3-130">Boolean</span></span>                        | <span data-ttu-id="be5c3-131">招待の受信者は、共有アイテムを表示するのにはサインインする必要かどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="be5c3-131">Specifies whether the recipient of the invitation is required to sign-in to view the shared item.</span></span>
| <span data-ttu-id="be5c3-132">sendInvitation</span><span class="sxs-lookup"><span data-stu-id="be5c3-132">sendInvitation</span></span>   | <span data-ttu-id="be5c3-133">ブール値</span><span class="sxs-lookup"><span data-stu-id="be5c3-133">Boolean</span></span>                        | <span data-ttu-id="be5c3-134">True の場合、[リンクを共有する][]は、受信者に送信されます。</span><span class="sxs-lookup"><span data-stu-id="be5c3-134">If true, a [sharing link][] is sent to the recipient.</span></span> <span data-ttu-id="be5c3-135">それ以外の場合、通知を送信せずに直接アクセス許可が与えられます。</span><span class="sxs-lookup"><span data-stu-id="be5c3-135">Otherwise, a permission is granted directly without sending a notification.</span></span>
| <span data-ttu-id="be5c3-136">roles</span><span class="sxs-lookup"><span data-stu-id="be5c3-136">roles</span></span>            | <span data-ttu-id="be5c3-137">Collection(String)</span><span class="sxs-lookup"><span data-stu-id="be5c3-137">Collection(String)</span></span>             | <span data-ttu-id="be5c3-138">共有への招待の受信者に許可するロールを指定します。</span><span class="sxs-lookup"><span data-stu-id="be5c3-138">Specify the roles that are to be granted to the recipients of the sharing invitation.</span></span>

## <a name="example"></a><span data-ttu-id="be5c3-139">使用例</span><span class="sxs-lookup"><span data-stu-id="be5c3-139">Example</span></span>

<span data-ttu-id="be5c3-140">次の使用例は、共同作業中のファイルについてのメッセージには、"ryan@contoso.com"の電子メール アドレスを持つユーザーに共有への招待を送信します。</span><span class="sxs-lookup"><span data-stu-id="be5c3-140">This example sends a sharing invitation to a user with email address "ryan@contoso.com" with a message about a file being collaborated on.</span></span>
<span data-ttu-id="be5c3-141">この招待により、Ryan にはファイルへの読み取り/書き込みアクセス権が付与されます。</span><span class="sxs-lookup"><span data-stu-id="be5c3-141">The invitation grants Ryan read-write access to the file.</span></span>

### <a name="http-request"></a><span data-ttu-id="be5c3-142">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="be5c3-142">HTTP Request</span></span>

<span data-ttu-id="be5c3-143">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で[アクセス許可](../resources/permission.md)コレクション オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="be5c3-143">If successful, this method returns `200 OK` response code and [permission](../resources/permission.md) collection object in the response body.</span></span>

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

### <a name="response"></a><span data-ttu-id="be5c3-144">応答</span><span class="sxs-lookup"><span data-stu-id="be5c3-144">Response</span></span>

<span data-ttu-id="be5c3-145">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="be5c3-145">Here is an example of the response.</span></span>

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

## <a name="remarks"></a><span data-ttu-id="be5c3-146">備考</span><span class="sxs-lookup"><span data-stu-id="be5c3-146">Remarks</span></span>

* <span data-ttu-id="be5c3-147">`personal` (OneDrive 個人用) の **driveType** を持つ[ドライブ](../resources/drive.md)は、ルートの DriveItem でアクセス許可を作成したり、変更したりすることはできません。</span><span class="sxs-lookup"><span data-stu-id="be5c3-147">[Drives](../resources/drive.md) with a **driveType** of `personal` (OneDrive personal) cannot create or modify permissions on the root DriveItem.</span></span>
* <span data-ttu-id="be5c3-148">使用可能なロールの一覧は、「[ロール列挙](../resources/permission.md#roles-enumeration)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="be5c3-148">For a list of available roles, see [Roles enumeration](../resources/permission.md#roles-enumeration).</span></span>

## <a name="error-responses"></a><span data-ttu-id="be5c3-149">エラー応答</span><span class="sxs-lookup"><span data-stu-id="be5c3-149">Error Responses</span></span>

<span data-ttu-id="be5c3-150">エラーがどのような形で返されるかについては、「[エラー応答][error-response]」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="be5c3-150">Read the [Error Responses][error-response] topic for more information about how errors are returned.</span></span>


[driveRecipient]: ../resources/driverecipient.md
[error-response]: /graph/errors
[リンクの共有]: ../resources/permission.md#sharing-links
[sharing link]: ../resources/permission.md#sharing-links

<!-- {
  "type": "#page.annotation",
  "description": "Add permissions to an item and optionally send a sharing notification.",
  "keywords": "retrieve,item,metadata",
  "section": "documentation",
  "tocPath": "Sharing/Add permissions"
} -->
