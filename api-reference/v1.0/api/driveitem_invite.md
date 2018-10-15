---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: アイテムにアクセスするために招待状を送信する
ms.openlocfilehash: c68289049503e70e04b2e403ca09cfc1f67e4096
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/21/2018
ms.locfileid: "23268733"
---
# <a name="send-a-sharing-invitation"></a><span data-ttu-id="87827-102">共有の招待状を送信する</span><span class="sxs-lookup"><span data-stu-id="87827-102">Send a sharing invitation</span></span>

<span data-ttu-id="87827-103">**DriveItem**の共有の招待状を送信します。</span><span class="sxs-lookup"><span data-stu-id="87827-103">Sends a sharing invitation for a **DriveItem**.</span></span>
<span data-ttu-id="87827-104">共有の招待では、受信者へのアクセス許可を提供し、オプションで [共有リンク][]を記載した電子メールが招待状の受信者に送信されます。</span><span class="sxs-lookup"><span data-stu-id="87827-104">A sharing invitation provides permissions to the recipients and optionally sends them an email with a [sharing link][].</span></span>

## <a name="permissions"></a><span data-ttu-id="87827-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="87827-105">Permissions</span></span>

<span data-ttu-id="87827-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="87827-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="87827-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="87827-108">Permission type</span></span>      | <span data-ttu-id="87827-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="87827-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="87827-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="87827-110">Delegated (work or school account)</span></span> | <span data-ttu-id="87827-111">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87827-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="87827-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="87827-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="87827-113">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87827-113">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="87827-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="87827-114">Application</span></span> | <span data-ttu-id="87827-115">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87827-115">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="87827-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="87827-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{drive-id}/items/{item-id}/invite
POST /groups/{group-id}/drive/items/{item-id}/invite
POST /me/drive/items/{item-id}/invite
POST /sites/{siteId}/drive/items/{itemId}/invite
POST /users/{userId}/drive/items/{itemId}/invite
```

## <a name="request-body"></a><span data-ttu-id="87827-117">要求本文</span><span class="sxs-lookup"><span data-stu-id="87827-117">Request body</span></span>

<span data-ttu-id="87827-118">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="87827-118">In the request body, provide a JSON object with the following parameters.</span></span>

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

| <span data-ttu-id="87827-119">パラメーター</span><span class="sxs-lookup"><span data-stu-id="87827-119">Parameter</span></span>        | <span data-ttu-id="87827-120">型</span><span class="sxs-lookup"><span data-stu-id="87827-120">Type</span></span>                           | <span data-ttu-id="87827-121">説明</span><span class="sxs-lookup"><span data-stu-id="87827-121">Description</span></span>
|:-----------------|:-------------------------------|:-------------------------
| <span data-ttu-id="87827-122">Recipients</span><span class="sxs-lookup"><span data-stu-id="87827-122">recipients</span></span>       | <span data-ttu-id="87827-123">コレクション ([DriveRecipient][])</span><span class="sxs-lookup"><span data-stu-id="87827-123">Collection([DriveRecipient][])</span></span> | <span data-ttu-id="87827-124">アクセスおよび共有の招待状を受信する、受信者のコレクション。</span><span class="sxs-lookup"><span data-stu-id="87827-124">A collection of recipients who will receive access and the sharing invitation.</span></span>
| <span data-ttu-id="87827-125">message</span><span class="sxs-lookup"><span data-stu-id="87827-125">message</span></span>          | <span data-ttu-id="87827-126">文字列</span><span class="sxs-lookup"><span data-stu-id="87827-126">String</span></span>                         | <span data-ttu-id="87827-p103">共有の招待状に含まれるプレーンテキスト形式のメッセージ。最大の長さは 2000 文字です。</span><span class="sxs-lookup"><span data-stu-id="87827-p103">A plain text formatted message that is included in the sharing invitation. Maximum length 2000 characters.</span></span>
| <span data-ttu-id="87827-129">requireSignIn</span><span class="sxs-lookup"><span data-stu-id="87827-129">requireSignIn</span></span>    | <span data-ttu-id="87827-130">ブール値</span><span class="sxs-lookup"><span data-stu-id="87827-130">Boolean</span></span>                        | <span data-ttu-id="87827-131">共有アイテムを表示するために、招待状の受信者がサインインする必要のあるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="87827-131">Specifies where the recipient of the invitation is required to sign-in to view the shared item.</span></span>
| <span data-ttu-id="87827-132">sendInvitation</span><span class="sxs-lookup"><span data-stu-id="87827-132">sendInvitation</span></span>   | <span data-ttu-id="87827-133">ブール値</span><span class="sxs-lookup"><span data-stu-id="87827-133">Boolean</span></span>                        | <span data-ttu-id="87827-134">True の場合、 [共有リンク][] が、受信者に送信されます。</span><span class="sxs-lookup"><span data-stu-id="87827-134">If true, a [sharing link][] is sent to the recipient.</span></span> <span data-ttu-id="87827-135">それ以外の場合、通知を送信せずに直接アクセス許可が与えられます。</span><span class="sxs-lookup"><span data-stu-id="87827-135">Otherwise, a permission is granted directly without sending a notification.</span></span>
| <span data-ttu-id="87827-136">roles</span><span class="sxs-lookup"><span data-stu-id="87827-136">roles</span></span>            | <span data-ttu-id="87827-137">コレクション (文字列)</span><span class="sxs-lookup"><span data-stu-id="87827-137">Collection(String)</span></span>             | <span data-ttu-id="87827-138">共有の招待状の受信者に付与されるロールを指定します。</span><span class="sxs-lookup"><span data-stu-id="87827-138">Specify the roles that are be granted to the recipients of the sharing invitation.</span></span>

## <a name="example"></a><span data-ttu-id="87827-139">例</span><span class="sxs-lookup"><span data-stu-id="87827-139">Example</span></span>

<span data-ttu-id="87827-140">この例では、"ryan@contoso.com" というメール アドレスを持つユーザーに共有の招待状を、共同作業中のファイルについてのメッセージと共に送信します。</span><span class="sxs-lookup"><span data-stu-id="87827-140">This example sends a sharing invitation to a user with email address "ryan@contoso.org" with a message about a file being collaborated on.</span></span>
<span data-ttu-id="87827-141">この招待により、Ryan にはファイルへの読み取り/書き込みアクセス権が付与されます。</span><span class="sxs-lookup"><span data-stu-id="87827-141">The invitation grants Ryan read-write access to the file.</span></span>

### <a name="http-request"></a><span data-ttu-id="87827-142">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="87827-142">HTTP Request</span></span>

<span data-ttu-id="87827-143">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で[アクセス許可](../resources/permission.md)コレクション オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="87827-143">If successful, this method returns `200 OK` response code and [permission](../resources/permission.md) collection object in the response body.</span></span>

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

### <a name="response"></a><span data-ttu-id="87827-144">応答</span><span class="sxs-lookup"><span data-stu-id="87827-144">Response</span></span>

<span data-ttu-id="87827-145">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="87827-145">Here is an example of the response.</span></span>

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

## <a name="remarks"></a><span data-ttu-id="87827-146">備考</span><span class="sxs-lookup"><span data-stu-id="87827-146">Remarks</span></span>

* <span data-ttu-id="87827-147">(OneDrive 個人用) の **driveType** を持つ[ドライブ](../resources/drive.md)は、ルートの DriveItem でアクセス許可を作成したり、変更したりすることはできません。`personal`</span><span class="sxs-lookup"><span data-stu-id="87827-147">[Drives](../resources/drive.md) with a **driveType** of `personal` (OneDrive personal) cannot create or modify permissions on the root DriveItem.</span></span>
* <span data-ttu-id="87827-148">使用可能なロールの一覧は、「[ロール列挙](../resources/permission.md#roles-enumeration)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="87827-148">For a list of available roles, see [Roles enumeration](../resources/permission.md#roles-enumeration).</span></span>

## <a name="error-responses"></a><span data-ttu-id="87827-149">エラー応答</span><span class="sxs-lookup"><span data-stu-id="87827-149">Error Responses</span></span>

<span data-ttu-id="87827-150">エラーがどのような形で返されるかについては、「[エラー応答][error-response]」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="87827-150">Read the [Error Responses][error-response] topic for more information about how errors are returned.</span></span>


[driveRecipient]: ../resources/driverecipient.md
[DriveRecipient]: ../resources/driverecipient.md
[error-response]: ../../../concepts/errors.md
[共有リンク]: ../resources/permission.md#sharing-links
[Create sharing link]: ../resources/permission.md#sharing-links

<!-- {
  "type": "#page.annotation",
  "description": "Add permissions to an item and optionally send a sharing notification.",
  "keywords": "retrieve,item,metadata",
  "section": "documentation",
  "tocPath": "Sharing/Add permissions"
} -->
