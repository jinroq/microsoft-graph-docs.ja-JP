---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: アイテムにアクセスするための招待状を送信する
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 129e94aef36e9779dd114848880ddba5243b218e
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35890855"
---
# <a name="send-a-sharing-invitation"></a><span data-ttu-id="4c461-102">共有の招待状を送信する</span><span class="sxs-lookup"><span data-stu-id="4c461-102">Send a sharing invitation</span></span>

<span data-ttu-id="4c461-103">**ドライブ項目**の共有への招待を送信します。</span><span class="sxs-lookup"><span data-stu-id="4c461-103">Sends a sharing invitation for a **DriveItem**.</span></span>
<span data-ttu-id="4c461-104">共有への招待では、受信者にアクセス許可が与えられ、必要に応じて[共有リンク][]を使用して電子メールを送信します。</span><span class="sxs-lookup"><span data-stu-id="4c461-104">A sharing invitation provides permissions to the recipients and optionally sends them an email with a [sharing link][].</span></span>

## <a name="permissions"></a><span data-ttu-id="4c461-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="4c461-105">Permissions</span></span>

<span data-ttu-id="4c461-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4c461-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4c461-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4c461-108">Permission type</span></span>      | <span data-ttu-id="4c461-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="4c461-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4c461-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4c461-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4c461-111">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c461-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="4c461-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4c461-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4c461-113">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c461-113">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="4c461-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4c461-114">Application</span></span> | <span data-ttu-id="4c461-115">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c461-115">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4c461-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4c461-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{drive-id}/items/{item-id}/invite
POST /groups/{group-id}/drive/items/{item-id}/invite
POST /me/drive/items/{item-id}/invite
POST /sites/{siteId}/drive/items/{itemId}/invite
POST /users/{userId}/drive/items/{itemId}/invite
```

## <a name="request-body"></a><span data-ttu-id="4c461-117">要求本文</span><span class="sxs-lookup"><span data-stu-id="4c461-117">Request body</span></span>

<span data-ttu-id="4c461-118">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="4c461-118">In the request body, provide a JSON object with the following parameters.</span></span>

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

| <span data-ttu-id="4c461-119">パラメーター</span><span class="sxs-lookup"><span data-stu-id="4c461-119">Parameter</span></span>        | <span data-ttu-id="4c461-120">型</span><span class="sxs-lookup"><span data-stu-id="4c461-120">Type</span></span>                           | <span data-ttu-id="4c461-121">説明</span><span class="sxs-lookup"><span data-stu-id="4c461-121">Description</span></span>
|:-----------------|:-------------------------------|:-------------------------
| <span data-ttu-id="4c461-122">Recipients</span><span class="sxs-lookup"><span data-stu-id="4c461-122">recipients</span></span>       | <span data-ttu-id="4c461-123">Collection([DriveRecipient][])</span><span class="sxs-lookup"><span data-stu-id="4c461-123">Collection([DriveRecipient][])</span></span> | <span data-ttu-id="4c461-124">アクセスおよび共有の招待状を受信する、受信者のコレクション。</span><span class="sxs-lookup"><span data-stu-id="4c461-124">A collection of recipients who will receive access and the sharing invitation.</span></span>
| <span data-ttu-id="4c461-125">message</span><span class="sxs-lookup"><span data-stu-id="4c461-125">message</span></span>          | <span data-ttu-id="4c461-126">String</span><span class="sxs-lookup"><span data-stu-id="4c461-126">String</span></span>                         | <span data-ttu-id="4c461-p103">共有の招待状に含まれるプレーンテキスト形式のメッセージ。最大の長さは 2000 文字です。</span><span class="sxs-lookup"><span data-stu-id="4c461-p103">A plain text formatted message that is included in the sharing invitation. Maximum length 2000 characters.</span></span>
| <span data-ttu-id="4c461-129">requireSignIn</span><span class="sxs-lookup"><span data-stu-id="4c461-129">requireSignIn</span></span>    | <span data-ttu-id="4c461-130">Boolean</span><span class="sxs-lookup"><span data-stu-id="4c461-130">Boolean</span></span>                        | <span data-ttu-id="4c461-131">共有アイテムを表示するために、招待状の受信者がサインインする必要があるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="4c461-131">Specifies whether the recipient of the invitation is required to sign-in to view the shared item.</span></span>
| <span data-ttu-id="4c461-132">sendInvitation</span><span class="sxs-lookup"><span data-stu-id="4c461-132">sendInvitation</span></span>   | <span data-ttu-id="4c461-133">ブール値</span><span class="sxs-lookup"><span data-stu-id="4c461-133">Boolean</span></span>                        | <span data-ttu-id="4c461-134">True の場合、[共有リンク][]は受信者に送信されます。</span><span class="sxs-lookup"><span data-stu-id="4c461-134">If true, a [sharing link][] is sent to the recipient.</span></span> <span data-ttu-id="4c461-135">それ以外の場合は、通知を送信することなく、直接アクセス許可が付与されます。</span><span class="sxs-lookup"><span data-stu-id="4c461-135">Otherwise, a permission is granted directly without sending a notification.</span></span>
| <span data-ttu-id="4c461-136">roles</span><span class="sxs-lookup"><span data-stu-id="4c461-136">roles</span></span>            | <span data-ttu-id="4c461-137">Collection(String)</span><span class="sxs-lookup"><span data-stu-id="4c461-137">Collection(String)</span></span>             | <span data-ttu-id="4c461-138">共有への招待の受信者に付与する役割を指定します。</span><span class="sxs-lookup"><span data-stu-id="4c461-138">Specify the roles that are to be granted to the recipients of the sharing invitation.</span></span>

## <a name="example"></a><span data-ttu-id="4c461-139">例</span><span class="sxs-lookup"><span data-stu-id="4c461-139">Example</span></span>

<span data-ttu-id="4c461-140">この例では、電子メールアドレスが "ryan@contoso.com" のユーザーに、共同作業中のファイルに関するメッセージを含む共有への招待を送信します。</span><span class="sxs-lookup"><span data-stu-id="4c461-140">This example sends a sharing invitation to a user with email address "ryan@contoso.com" with a message about a file being collaborated on.</span></span>
<span data-ttu-id="4c461-141">この招待により、Ryan にはファイルへの読み取り/書き込みアクセス権が付与されます。</span><span class="sxs-lookup"><span data-stu-id="4c461-141">The invitation grants Ryan read-write access to the file.</span></span>

### <a name="http-request"></a><span data-ttu-id="4c461-142">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4c461-142">HTTP Request</span></span>

<span data-ttu-id="4c461-143">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で[アクセス許可](../resources/permission.md)コレクション オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="4c461-143">If successful, this method returns `200 OK` response code and [permission](../resources/permission.md) collection object in the response body.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="4c461-144">プロトコル</span><span class="sxs-lookup"><span data-stu-id="4c461-144">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="4c461-145">C#</span><span class="sxs-lookup"><span data-stu-id="4c461-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/send-sharing-invite-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4c461-146">Javascript</span><span class="sxs-lookup"><span data-stu-id="4c461-146">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/send-sharing-invite-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4c461-147">目的-C</span><span class="sxs-lookup"><span data-stu-id="4c461-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/send-sharing-invite-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="4c461-148">Java</span><span class="sxs-lookup"><span data-stu-id="4c461-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/send-sharing-invite-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4c461-149">応答</span><span class="sxs-lookup"><span data-stu-id="4c461-149">Response</span></span>

<span data-ttu-id="4c461-150">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="4c461-150">Here is an example of the response.</span></span>

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

## <a name="remarks"></a><span data-ttu-id="4c461-151">備考</span><span class="sxs-lookup"><span data-stu-id="4c461-151">Remarks</span></span>

* <span data-ttu-id="4c461-152">`personal` (OneDrive 個人用) の **driveType** を持つ[ドライブ](../resources/drive.md)は、ルートの DriveItem でアクセス許可を作成したり、変更したりすることはできません。</span><span class="sxs-lookup"><span data-stu-id="4c461-152">[Drives](../resources/drive.md) with a **driveType** of `personal` (OneDrive personal) cannot create or modify permissions on the root DriveItem.</span></span>
* <span data-ttu-id="4c461-153">使用可能なロールの一覧は、「[ロール列挙](../resources/permission.md#roles-enumeration)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4c461-153">For a list of available roles, see [Roles enumeration](../resources/permission.md#roles-enumeration).</span></span>

## <a name="error-responses"></a><span data-ttu-id="4c461-154">エラー応答</span><span class="sxs-lookup"><span data-stu-id="4c461-154">Error Responses</span></span>

<span data-ttu-id="4c461-155">エラーがどのような形で返されるかについては、「[エラー応答][error-response]」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4c461-155">Read the [Error Responses][error-response] topic for more information about how errors are returned.</span></span>


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
  ]
} -->
