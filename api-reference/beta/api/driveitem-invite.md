---
author: JeremyKelley
description: ドライブ項目の共有への招待を送信します。
ms.date: 09/10/2017
title: アイテムにアクセスするための招待状を送信する
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: ccd80a31ade0be6fc5e63002d02dd7e8f2235e87
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36324358"
---
# <a name="send-a-sharing-invitation"></a><span data-ttu-id="c6086-103">共有の招待状を送信する</span><span class="sxs-lookup"><span data-stu-id="c6086-103">Send a sharing invitation</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c6086-p101">**DriveItem** の共有の招待状を送信します。共有の招待状は受信者にアクセス許可を提供します。また、任意で受信者に、アイテムが共有されたことを通知する電子メールを送信します。</span><span class="sxs-lookup"><span data-stu-id="c6086-p101">Sends a sharing invitation for a **DriveItem**. A sharing invitation provides permissions to the recipients and optionally sends an email to the recipients to notify them the item was shared.</span></span>

## <a name="permissions"></a><span data-ttu-id="c6086-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c6086-106">Permissions</span></span>

<span data-ttu-id="c6086-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c6086-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c6086-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c6086-109">Permission type</span></span>      | <span data-ttu-id="c6086-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c6086-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c6086-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c6086-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c6086-112">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c6086-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="c6086-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c6086-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c6086-114">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c6086-114">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="c6086-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c6086-115">Application</span></span> | <span data-ttu-id="c6086-116">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c6086-116">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c6086-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c6086-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{drive-id}/items/{item-id}/invite
POST /groups/{group-id}/drive/items/{item-id}/invite
POST /me/drive/items/{item-id}/invite
POST /sites/{siteId}/drive/items/{itemId}/invite
POST /users/{userId}/drive/items/{itemId}/invite
```

## <a name="request-body"></a><span data-ttu-id="c6086-118">要求本文</span><span class="sxs-lookup"><span data-stu-id="c6086-118">Request body</span></span>

<span data-ttu-id="c6086-119">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="c6086-119">In the request body, provide a JSON object with the following parameters.</span></span>

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

| <span data-ttu-id="c6086-120">パラメーター</span><span class="sxs-lookup"><span data-stu-id="c6086-120">Parameter</span></span>        | <span data-ttu-id="c6086-121">型</span><span class="sxs-lookup"><span data-stu-id="c6086-121">Type</span></span>                                            | <span data-ttu-id="c6086-122">説明</span><span class="sxs-lookup"><span data-stu-id="c6086-122">Description</span></span>                                                                                                |
|:-----------------|:------------------------------------------------|:-----------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="c6086-123">Recipients</span><span class="sxs-lookup"><span data-stu-id="c6086-123">recipients</span></span>       | <span data-ttu-id="c6086-124">Collection([DriveRecipient](../resources/driverecipient.md))</span><span class="sxs-lookup"><span data-stu-id="c6086-124">Collection([DriveRecipient](../resources/driverecipient.md))</span></span> | <span data-ttu-id="c6086-125">アクセスおよび共有の招待状を受信する、受信者のコレクション。</span><span class="sxs-lookup"><span data-stu-id="c6086-125">A collection of recipients who will receive access and the sharing invitation.</span></span>                                            |
| <span data-ttu-id="c6086-126">message</span><span class="sxs-lookup"><span data-stu-id="c6086-126">message</span></span>          | <span data-ttu-id="c6086-127">String</span><span class="sxs-lookup"><span data-stu-id="c6086-127">String</span></span>                                          | <span data-ttu-id="c6086-p103">共有の招待状に含まれるプレーンテキスト形式のメッセージ。最大の長さは 2000 文字です。</span><span class="sxs-lookup"><span data-stu-id="c6086-p103">A plain text formatted message that is included in the sharing invitation. Maximum length 2000 characters.</span></span> |
| <span data-ttu-id="c6086-130">requireSignIn</span><span class="sxs-lookup"><span data-stu-id="c6086-130">requireSignIn</span></span>    | <span data-ttu-id="c6086-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6086-131">Boolean</span></span>                                         | <span data-ttu-id="c6086-132">共有アイテムを表示するために、招待状の受信者がサインインする必要のある場所を指定します。</span><span class="sxs-lookup"><span data-stu-id="c6086-132">Specifies where the recipient of the invitation is required to sign-in to view the shared item.</span></span>            |
| <span data-ttu-id="c6086-133">sendInvitation</span><span class="sxs-lookup"><span data-stu-id="c6086-133">sendInvitation</span></span>   | <span data-ttu-id="c6086-134">ブール値</span><span class="sxs-lookup"><span data-stu-id="c6086-134">Boolean</span></span>                                         | <span data-ttu-id="c6086-135">電子メールまたは投稿が生成されるのか (false)、アクセス許可のみが作成されるのか (true) を指定します。</span><span class="sxs-lookup"><span data-stu-id="c6086-135">Specifies if an email or post is generated (false) or if the permission is just created (true).</span></span>            |
| <span data-ttu-id="c6086-136">roles</span><span class="sxs-lookup"><span data-stu-id="c6086-136">roles</span></span>            | <span data-ttu-id="c6086-137">Collection(String)</span><span class="sxs-lookup"><span data-stu-id="c6086-137">Collection(String)</span></span>                              | <span data-ttu-id="c6086-138">共有の招待状の受信者に付与されるロールを指定します。</span><span class="sxs-lookup"><span data-stu-id="c6086-138">Specify the roles that are be granted to the recipients of the sharing invitation.</span></span>                         |
| <span data-ttu-id="c6086-139">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="c6086-139">expirationDateTime</span></span> | <span data-ttu-id="c6086-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c6086-140">DateTimeOffset</span></span>                       | <span data-ttu-id="c6086-141">アクセス許可の有効期限が切れる日時を指定します。</span><span class="sxs-lookup"><span data-stu-id="c6086-141">Specify the DateTime after which the permission expires.</span></span> <span data-ttu-id="c6086-142">OneDrive for business、SharePoint、プレミアム個人用 OneDrive のアカウントで利用できます。</span><span class="sxs-lookup"><span data-stu-id="c6086-142">Available on OneDrive for Business, SharePoint, and premium personal OneDrive accounts.</span></span>
| <span data-ttu-id="c6086-143">パスワード</span><span class="sxs-lookup"><span data-stu-id="c6086-143">password</span></span>           | <span data-ttu-id="c6086-144">String</span><span class="sxs-lookup"><span data-stu-id="c6086-144">String</span></span>                         | <span data-ttu-id="c6086-145">作成者による招待に設定されたパスワード。</span><span class="sxs-lookup"><span data-stu-id="c6086-145">The password set on the invite by the creator.</span></span> <span data-ttu-id="c6086-146">省略可能および OneDrive 個人用のみ</span><span class="sxs-lookup"><span data-stu-id="c6086-146">Optional and OneDrive Personal only</span></span>

## <a name="example"></a><span data-ttu-id="c6086-147">例</span><span class="sxs-lookup"><span data-stu-id="c6086-147">Example</span></span>

<span data-ttu-id="c6086-148">この例では、"ryan@contoso.org" というメール アドレスを持つユーザーに共有の招待状を、共同作業中のファイルについてのメッセージと共に送信します。</span><span class="sxs-lookup"><span data-stu-id="c6086-148">This example sends a sharing invitation to a user with email address "ryan@contoso.org" with a message about a file being collaborated on.</span></span>
<span data-ttu-id="c6086-149">この招待により、Ryan にはファイルへの読み取り/書き込みアクセス権が付与されます。</span><span class="sxs-lookup"><span data-stu-id="c6086-149">The invitation grants Ryan read-write access to the file.</span></span>

### <a name="http-request"></a><span data-ttu-id="c6086-150">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c6086-150">HTTP request</span></span>

<span data-ttu-id="c6086-151">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で[アクセス許可](../resources/permission.md)コレクション オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="c6086-151">If successful, this method returns `200 OK` response code and [permission](../resources/permission.md) collection object in the response body.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="c6086-152">プロトコル</span><span class="sxs-lookup"><span data-stu-id="c6086-152">HTTP</span></span>](#tab/http)
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
  "roles": [ "write" ],
  "password": "password123",
  "expirationDateTime": "2018-07-15T14:00:00.000Z"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c6086-153">C#</span><span class="sxs-lookup"><span data-stu-id="c6086-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/send-sharing-invite-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c6086-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c6086-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/send-sharing-invite-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c6086-155">目的-C</span><span class="sxs-lookup"><span data-stu-id="c6086-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/send-sharing-invite-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c6086-156">Java</span><span class="sxs-lookup"><span data-stu-id="c6086-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/send-sharing-invite-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c6086-157">応答</span><span class="sxs-lookup"><span data-stu-id="c6086-157">Response</span></span>

<span data-ttu-id="c6086-158">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="c6086-158">Here is an example of the response.</span></span>

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
      "hasPassword": true,
      "id": "CCFC7CA3-7A19-4D57-8CEF-149DB9DDFA62",
      "invitation": {
        "email": "ryan@contoso.com",
        "signInRequired": true
      },
      "roles": [ "write" ],
      "expirationDateTime": "2018-07-15T14:00:00.000Z"
    }
  ]
}
```
### <a name="partial-success-response"></a><span data-ttu-id="c6086-159">正常な応答の一部</span><span class="sxs-lookup"><span data-stu-id="c6086-159">Partial success response</span></span>

<span data-ttu-id="c6086-160">複数の受信者への招待では、一部の受信者に対して通知が成功する可能性があります。</span><span class="sxs-lookup"><span data-stu-id="c6086-160">When inviting multiple recipients, it's possible for the notification to succeed for some and fail for others.</span></span>
<span data-ttu-id="c6086-161">この場合、サービスは、HTTP 状態コードが207である部分的な成功応答を返します。</span><span class="sxs-lookup"><span data-stu-id="c6086-161">In this case, the service returns a partial success response with an HTTP status code of 207.</span></span>
<span data-ttu-id="c6086-162">部分的な成功が返された場合は、失敗した各`error`受信者の応答に、発生した問題とその修正方法に関する情報を持つオブジェクトが含まれます。</span><span class="sxs-lookup"><span data-stu-id="c6086-162">When partial success is returned, the response for each failed recipient will contain an `error` object with information about what went wrong and how to fix it.</span></span>

<span data-ttu-id="c6086-163">部分的な応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c6086-163">Here is an example of the partial response.</span></span>  

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.permission)", "truncated": true } -->

```json
HTTP/1.1 207 Multi-Status
Content-type: application/json

{
  "value": [
    {
      "grantedTo": {
        "user": {
          "displayName": "John Adams",
          "id": "5D8CA5D0-FFF8-4A97-B0A6-8F5AEA339681"
        }
      },
      "id": "1EFG7CA3-7A19-4D57-8CEF-149DB9DDFA62",
      "invitation": {
        "email": "adams@contoso.com",
        "signInRequired": true
      },
      "roles": [ "write" ],
      "error": {
        "code":"notAllowed",
        "message":"Account verification needed to unblock sending emails.",
        "localizedMessage": "Kontobestätigung erforderlich, um das Senden von E-Mails zu entsperren.",
        "fixItUrl":"http://g.live.com/8SESkydrive/VerifyAccount",
        "innererror":{  
          "code":"accountVerificationRequired" 
        }
      }
    },
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
      "roles": [ "write" ],
      "expirationDateTime": "2018-07-15T14:00:00.000Z"
    }
  ]
}
```
### <a name="sendnotification-errors"></a><span data-ttu-id="c6086-164">SendNotification エラー</span><span class="sxs-lookup"><span data-stu-id="c6086-164">SendNotification errors</span></span>
<span data-ttu-id="c6086-165">通知の送信が失敗した場合に、入れ子になっ`innererror`たオブジェクト内でアプリに発生する可能性があるその他のエラーを次に示します。</span><span class="sxs-lookup"><span data-stu-id="c6086-165">The following are some additional errors that your app might encounter within the nested `innererror` objects when sending notification fails.</span></span> <span data-ttu-id="c6086-166">アプリでは、これらを処理する必要はありません。</span><span class="sxs-lookup"><span data-stu-id="c6086-166">Apps are not required to handle these.</span></span>

| <span data-ttu-id="c6086-167">コード</span><span class="sxs-lookup"><span data-stu-id="c6086-167">Code</span></span>                           | <span data-ttu-id="c6086-168">説明</span><span class="sxs-lookup"><span data-stu-id="c6086-168">Description</span></span>
|:-------------------------------|:--------------------------------------------------------------------------------------
| <span data-ttu-id="c6086-169">accountVerificationRequired</span><span class="sxs-lookup"><span data-stu-id="c6086-169">accountVerificationRequired</span></span>    | <span data-ttu-id="c6086-170">通知の送信のブロックを解除するには、アカウントの確認が必要です。</span><span class="sxs-lookup"><span data-stu-id="c6086-170">Account verification is required to unblock sending notifications.</span></span>
| <span data-ttu-id="c6086-171">hipCheckRequired</span><span class="sxs-lookup"><span data-stu-id="c6086-171">hipCheckRequired</span></span>               | <span data-ttu-id="c6086-172">HIP を解決する必要があります。 [通知の送信をブロック解除する] チェックボックスをオンにします。</span><span class="sxs-lookup"><span data-stu-id="c6086-172">Need to solve HIP (Host Intrusion Prevention) check to unblock sending notifications.</span></span>
| <span data-ttu-id="c6086-173">exchangeInvalidUser</span><span class="sxs-lookup"><span data-stu-id="c6086-173">exchangeInvalidUser</span></span>            | <span data-ttu-id="c6086-174">現在のユーザーのメールボックスが見つかりませんでした。</span><span class="sxs-lookup"><span data-stu-id="c6086-174">Current user's mailbox was not found.</span></span>
| <span data-ttu-id="c6086-175">exchangeOutOfMailboxQuota</span><span class="sxs-lookup"><span data-stu-id="c6086-175">exchangeOutOfMailboxQuota</span></span>      | <span data-ttu-id="c6086-176">クォータが不足しています。</span><span class="sxs-lookup"><span data-stu-id="c6086-176">Out of quota.</span></span>
| <span data-ttu-id="c6086-177">exchangeMaxRecipients</span><span class="sxs-lookup"><span data-stu-id="c6086-177">exchangeMaxRecipients</span></span>          | <span data-ttu-id="c6086-178">一度に通知を送信できる受信者の最大数を超過しました。</span><span class="sxs-lookup"><span data-stu-id="c6086-178">Exceeded maximum number of recipients that can be sent notifications at the same time.</span></span>

><span data-ttu-id="c6086-179">**注:** このサービスは、新しいエラーコードを追加するか、または、いつでも古いものを返すことを停止できます。</span><span class="sxs-lookup"><span data-stu-id="c6086-179">**Note:** The service can add new error codes or stop returning old ones at any time.</span></span>

## <a name="remarks"></a><span data-ttu-id="c6086-180">備考</span><span class="sxs-lookup"><span data-stu-id="c6086-180">Remarks</span></span>

* <span data-ttu-id="c6086-181">`personal` (OneDrive 個人用) の **driveType** を持つ[ドライブ](../resources/drive.md)は、ルートの DriveItem でアクセス許可を作成したり、変更したりすることはできません。</span><span class="sxs-lookup"><span data-stu-id="c6086-181">[Drives](../resources/drive.md) with a **driveType** of `personal` (OneDrive personal) cannot create or modify permissions on the root DriveItem.</span></span>
* <span data-ttu-id="c6086-182">使用可能なロールの一覧は、「[ロール列挙](../resources/permission.md#roles-enumeration-values)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c6086-182">For a list of available roles, see [Roles enumeration](../resources/permission.md#roles-enumeration-values).</span></span>

## <a name="error-responses"></a><span data-ttu-id="c6086-183">エラー応答</span><span class="sxs-lookup"><span data-stu-id="c6086-183">Error responses</span></span>

<span data-ttu-id="c6086-184">エラーがどのような形で返されるかについては、「[エラー応答][error-response]」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c6086-184">Read the [Error Responses][error-response] topic for more information about how errors are returned.</span></span>


[error-response]: /graph/errors

<!--
{
  "type": "#page.annotation",
  "description": "Add permissions to an item and optionally send a sharing notification.",
  "keywords": "retrieve,item,metadata",
  "section": "documentation",
  "tocPath": "Sharing/Add permissions",
  "suppressions": [
  ]
}
-->
