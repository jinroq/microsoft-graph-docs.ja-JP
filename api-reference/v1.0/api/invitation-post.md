---
title: 招待状の作成
description: この API を使用して、新しい招待状を作成します。 招待状によって外部ユーザーが組織に追加されます。
localization_priority: Priority
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b89b48bba7374b8f194c7597fe71164dc70caf4b
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35272122"
---
# <a name="create-invitation"></a><span data-ttu-id="3a267-104">招待状の作成</span><span class="sxs-lookup"><span data-stu-id="3a267-104">Create invitation</span></span>

<span data-ttu-id="3a267-p102">この API を使用して、新しい [招待状](../resources/invitation.md) を作成します。招待状によって外部ユーザーが組織に追加されます。</span><span class="sxs-lookup"><span data-stu-id="3a267-p102">Use this API to create a new [invitation](../resources/invitation.md). Invitation adds an external user to the organization.</span></span>

<span data-ttu-id="3a267-107">新しい招待状を作成するときに、選択可能ないくつかのオプションがあります。</span><span class="sxs-lookup"><span data-stu-id="3a267-107">When creating a new invitation you have several options available:</span></span>

1. <span data-ttu-id="3a267-p103">招待状の作成に際して、Microsoft Graph は自動的に招待メールを招待ユーザーに直接送信できます。作成応答で返された *inviteRedeemUrl* をアプリが使用して、招待ユーザーへの (任意の通信メカニズムによる) 独自の招待状を作成することもできます。Microsoft Graph によって招待メールが自動的に送信されるようにする場合は、[*invitedUserMessageInfo*](../resources/invitedusermessageinfo.md) を使用してメールの内容と言語を制御できます。</span><span class="sxs-lookup"><span data-stu-id="3a267-p103">On invitation creation, Microsoft Graph can automatically send an invitation email directly to the invited user, or your app can use the *inviteRedeemUrl* returned in the creation response to craft your own invitation (through your communication mechanism of choice) to the invited user. If you decide to have Microsoft Graph send an invitation email automatically, you can control the content and language of the email using [*invitedUserMessageInfo*](../resources/invitedusermessageinfo.md).</span></span>
2. <span data-ttu-id="3a267-p104">ユーザーが招待されると、(userType Guest) のユーザー エンティティが作成され、リソースへのアクセスの制御に使用できるようになります。招待ユーザーは、招待されたリソースにアクセスするためには、引き換え処理を行う必要があります。</span><span class="sxs-lookup"><span data-stu-id="3a267-p104">When the user is invited, a user entity (of userType Guest) is created and can now be used to control access to resources. The invited user has to go through the redemption process to access any resources he has been invited to.</span></span>

## <a name="permissions"></a><span data-ttu-id="3a267-112">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="3a267-112">Permissions</span></span>
<span data-ttu-id="3a267-p105">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3a267-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="3a267-115">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3a267-115">Permission type</span></span>      | <span data-ttu-id="3a267-116">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="3a267-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3a267-117">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3a267-117">Delegated (work or school account)</span></span> | <span data-ttu-id="3a267-118">User.Invite.All、User.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a267-118">User.Invite.All, User.ReadWrite.All, Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="3a267-119">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3a267-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3a267-120">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3a267-120">Not supported.</span></span>    |
|<span data-ttu-id="3a267-121">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3a267-121">Application</span></span> | <span data-ttu-id="3a267-122">User.Invite.All、User.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a267-122">User.Invite.All, User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3a267-123">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3a267-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /invitations
```
## <a name="request-headers"></a><span data-ttu-id="3a267-124">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3a267-124">Request headers</span></span>
| <span data-ttu-id="3a267-125">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3a267-125">Header</span></span>       | <span data-ttu-id="3a267-126">値</span><span class="sxs-lookup"><span data-stu-id="3a267-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3a267-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="3a267-127">Authorization</span></span>  | <span data-ttu-id="3a267-p106">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="3a267-p106">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="3a267-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3a267-130">Content-Type</span></span>  | <span data-ttu-id="3a267-131">application/json</span><span class="sxs-lookup"><span data-stu-id="3a267-131">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3a267-132">要求本文</span><span class="sxs-lookup"><span data-stu-id="3a267-132">Request body</span></span>
<span data-ttu-id="3a267-133">要求本文で、[invitation](../resources/invitation.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="3a267-133">In the request body, supply a JSON representation of an [invitation](../resources/invitation.md) object.</span></span>

<span data-ttu-id="3a267-134">次の表に、招待状の作成時に必要になるプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="3a267-134">The following table shows the properties that are required when you create a invitation.</span></span>

| <span data-ttu-id="3a267-135">パラメーター</span><span class="sxs-lookup"><span data-stu-id="3a267-135">Parameter</span></span> | <span data-ttu-id="3a267-136">型</span><span class="sxs-lookup"><span data-stu-id="3a267-136">Type</span></span> | <span data-ttu-id="3a267-137">説明</span><span class="sxs-lookup"><span data-stu-id="3a267-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3a267-138">invitedUserEmailAddress</span><span class="sxs-lookup"><span data-stu-id="3a267-138">invitedUserEmailAddress</span></span> |<span data-ttu-id="3a267-139">string</span><span class="sxs-lookup"><span data-stu-id="3a267-139">string</span></span> | <span data-ttu-id="3a267-140">招待するユーザーのメール アドレス。</span><span class="sxs-lookup"><span data-stu-id="3a267-140">The email address of the user you are inviting.</span></span>|
|<span data-ttu-id="3a267-141">inviteRedirectUrl</span><span class="sxs-lookup"><span data-stu-id="3a267-141">inviteRedirectUrl</span></span> |<span data-ttu-id="3a267-142">string</span><span class="sxs-lookup"><span data-stu-id="3a267-142">string</span></span> |<span data-ttu-id="3a267-143">引き換え後にユーザーがリダイレクトされる URL。</span><span class="sxs-lookup"><span data-stu-id="3a267-143">The URL that the user will be redirected to after redemption.</span></span>|

## <a name="response"></a><span data-ttu-id="3a267-144">応答</span><span class="sxs-lookup"><span data-stu-id="3a267-144">Response</span></span>

<span data-ttu-id="3a267-145">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [invitation](../resources/invitation.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="3a267-145">If successful, this method returns `201 Created` response code and [invitation](../resources/invitation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3a267-146">例</span><span class="sxs-lookup"><span data-stu-id="3a267-146">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3a267-147">要求</span><span class="sxs-lookup"><span data-stu-id="3a267-147">Request</span></span>
<span data-ttu-id="3a267-148">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="3a267-148">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_invitation_post"
}-->
```http
POST https://graph.microsoft.com/v1.0/invitations
Content-type: application/json
Content-length: 551

{
  "invitedUserEmailAddress": "yyy@test.com",
  "inviteRedirectUrl": "https://myapp.com"
}
```

##### <a name="response"></a><span data-ttu-id="3a267-149">応答</span><span class="sxs-lookup"><span data-stu-id="3a267-149">Response</span></span>
<span data-ttu-id="3a267-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="3a267-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "invitedUser": { "id": "243b1de4-ad9f-421c-a933-d55305fb165d" }
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="3a267-153">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="3a267-153">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="3a267-154">C#</span><span class="sxs-lookup"><span data-stu-id="3a267-154">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_invitation_post-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3a267-155">Javascript</span><span class="sxs-lookup"><span data-stu-id="3a267-155">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_invitation_post-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="3a267-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3a267-156">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_invitation_post-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- {
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/v1.0/api/invitation-post.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/invitation-post.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/invitation-post.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: create_user_from_users/invitedUser:
      Property 'invitedUser' is of type Custom but has no custom members."
  ]
}-->
