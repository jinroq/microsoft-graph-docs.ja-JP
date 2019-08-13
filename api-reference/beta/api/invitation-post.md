---
title: 招待状の作成
description: この API を使用して、新しい招待状を作成します。 招待状によって外部ユーザーが組織に追加されます。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a39c9d3dc04d4370723f988f7213982a5572507f
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36350021"
---
# <a name="create-invitation"></a><span data-ttu-id="26c21-104">招待状の作成</span><span class="sxs-lookup"><span data-stu-id="26c21-104">Create invitation</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="26c21-p102">この API を使用して、新しい [招待状](../resources/invitation.md) を作成します。招待状によって外部ユーザーが組織に追加されます。</span><span class="sxs-lookup"><span data-stu-id="26c21-p102">Use this API to create a new [invitation](../resources/invitation.md). Invitation adds an external user to the organization.</span></span>

<span data-ttu-id="26c21-107">新しい招待状を作成するときに、選択可能ないくつかのオプションがあります。</span><span class="sxs-lookup"><span data-stu-id="26c21-107">When creating a new invitation you have several options available:</span></span>

1. <span data-ttu-id="26c21-p103">招待状の作成に際して、Microsoft Graph は自動的に招待メールを招待ユーザーに直接送信できます。作成応答で返された *inviteRedeemUrl* をアプリが使用して、招待ユーザーへの (任意の通信メカニズムによる) 独自の招待状を作成することもできます。Microsoft Graph によって招待メールが自動的に送信されるようにする場合は、[*invitedUserMessageInfo*](../resources/invitedusermessageinfo.md) を使用してメールの内容と言語を制御できます。</span><span class="sxs-lookup"><span data-stu-id="26c21-p103">On invitation creation, Microsoft Graph can automatically send an invitation email directly to the invited user, or your app can use the *inviteRedeemUrl* returned in the creation response to craft your own invitation (through your communication mechanism of choice) to the invited user. If you decide to have Microsoft Graph send an invitation email automatically, you can control the content and language of the email using [*invitedUserMessageInfo*](../resources/invitedusermessageinfo.md).</span></span>
2. <span data-ttu-id="26c21-p104">ユーザーが招待されると、(userType Guest) のユーザー エンティティが作成され、リソースへのアクセスの制御に使用できるようになります。招待ユーザーは、招待されたリソースにアクセスするためには、引き換え処理を行う必要があります。</span><span class="sxs-lookup"><span data-stu-id="26c21-p104">When the user is invited, a user entity (of userType Guest) is created and can now be used to control access to resources. The invited user has to go through the redemption process to access any resources he has been invited to.</span></span>

## <a name="permissions"></a><span data-ttu-id="26c21-112">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="26c21-112">Permissions</span></span>
<span data-ttu-id="26c21-p105">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="26c21-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="26c21-115">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="26c21-115">Permission type</span></span>      | <span data-ttu-id="26c21-116">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="26c21-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="26c21-117">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="26c21-117">Delegated (work or school account)</span></span> | <span data-ttu-id="26c21-118">User.Invite.All、User.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26c21-118">User.Invite.All, User.ReadWrite.All, Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="26c21-119">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="26c21-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="26c21-120">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="26c21-120">Not supported.</span></span>    |
|<span data-ttu-id="26c21-121">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="26c21-121">Application</span></span> | <span data-ttu-id="26c21-122">User.Invite.All、User.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26c21-122">User.Invite.All, User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="26c21-123">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="26c21-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /invitations
```
## <a name="request-headers"></a><span data-ttu-id="26c21-124">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="26c21-124">Request headers</span></span>
| <span data-ttu-id="26c21-125">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="26c21-125">Header</span></span>       | <span data-ttu-id="26c21-126">値</span><span class="sxs-lookup"><span data-stu-id="26c21-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="26c21-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="26c21-127">Authorization</span></span>  | <span data-ttu-id="26c21-p106">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="26c21-p106">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="26c21-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="26c21-130">Content-Type</span></span>  | <span data-ttu-id="26c21-131">application/json</span><span class="sxs-lookup"><span data-stu-id="26c21-131">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="26c21-132">要求本文</span><span class="sxs-lookup"><span data-stu-id="26c21-132">Request body</span></span>
<span data-ttu-id="26c21-133">要求本文で、[invitation](../resources/invitation.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="26c21-133">In the request body, supply a JSON representation of an [invitation](../resources/invitation.md) object.</span></span>

<span data-ttu-id="26c21-134">次の表に、招待状の作成時に必要になるプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="26c21-134">The following table shows the properties that are required when you create a invitation.</span></span>

| <span data-ttu-id="26c21-135">パラメーター</span><span class="sxs-lookup"><span data-stu-id="26c21-135">Parameter</span></span> | <span data-ttu-id="26c21-136">型</span><span class="sxs-lookup"><span data-stu-id="26c21-136">Type</span></span> | <span data-ttu-id="26c21-137">説明</span><span class="sxs-lookup"><span data-stu-id="26c21-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="26c21-138">invitedUserEmailAddress</span><span class="sxs-lookup"><span data-stu-id="26c21-138">invitedUserEmailAddress</span></span> |<span data-ttu-id="26c21-139">string</span><span class="sxs-lookup"><span data-stu-id="26c21-139">string</span></span> | <span data-ttu-id="26c21-140">招待するユーザーのメール アドレス。</span><span class="sxs-lookup"><span data-stu-id="26c21-140">The email address of the user you are inviting.</span></span>|
|<span data-ttu-id="26c21-141">inviteRedirectUrl</span><span class="sxs-lookup"><span data-stu-id="26c21-141">inviteRedirectUrl</span></span> |<span data-ttu-id="26c21-142">string</span><span class="sxs-lookup"><span data-stu-id="26c21-142">string</span></span> |<span data-ttu-id="26c21-143">引き換え後にユーザーがリダイレクトされる URL。</span><span class="sxs-lookup"><span data-stu-id="26c21-143">The URL that the user will be redirected to after redemption.</span></span>|

## <a name="response"></a><span data-ttu-id="26c21-144">応答</span><span class="sxs-lookup"><span data-stu-id="26c21-144">Response</span></span>

<span data-ttu-id="26c21-145">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [invitation](../resources/invitation.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="26c21-145">If successful, this method returns `201 Created` response code and [invitation](../resources/invitation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="26c21-146">例</span><span class="sxs-lookup"><span data-stu-id="26c21-146">Example</span></span>
##### <a name="request"></a><span data-ttu-id="26c21-147">要求</span><span class="sxs-lookup"><span data-stu-id="26c21-147">Request</span></span>
<span data-ttu-id="26c21-148">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="26c21-148">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="26c21-149">プロトコル</span><span class="sxs-lookup"><span data-stu-id="26c21-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_invitation_post"
}-->
```http
POST https://graph.microsoft.com/beta/invitations
Content-type: application/json
Content-length: 551

{
  "invitedUserEmailAddress": "yyy@test.com",
  "inviteRedirectUrl": "https://myapp.com"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="26c21-150">C#</span><span class="sxs-lookup"><span data-stu-id="26c21-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-invitation-post-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="26c21-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="26c21-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-invitation-post-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="26c21-152">目的-C</span><span class="sxs-lookup"><span data-stu-id="26c21-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-invitation-post-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="26c21-153">Java</span><span class="sxs-lookup"><span data-stu-id="26c21-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-invitation-post-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="26c21-154">応答</span><span class="sxs-lookup"><span data-stu-id="26c21-154">Response</span></span>
<span data-ttu-id="26c21-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="26c21-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.invitation"
} -->
```http
HTTP/1.1 201 OK
Content-type: application/json
Content-length: 551

{
  "id": "7b92124c-9fa9-406f-8b8e-225df8376ba9",
  "inviteRedeemUrl": "https://invitations.microsoft.com/redeem/?tenant=04dcc6ab-388a-4559-b527-fbec656300ea&user=7b92124c-9fa9-406f-8b8e-225df8376ba9&ticket=VV9dmiExBsfRIVNFjb9ITj9VXAd07Ypv4gTg%2f8PiuJs%3d&lc=1033&ver=2.0",
  "invitedUserDisplayName": "yyy",
  "invitedUserEmailAddress": "yyy@test.com",
  "sendInvitationMessage": false,
  "invitedUserMessageInfo": {
     "messageLanguage": null,
     "ccRecipients": [
          {
             "emailAddress": {
                 "name": null,
                 "address": null
              }
          }
     ],
     "customizedMessageBody": null
  },
  "inviteRedirectUrl": "https://myapp.com/",
  "status": "Completed",
  "invitedUser":  [ {  "id": "243b1de4-ad9f-421c-a933-d55305fb165d" } ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
