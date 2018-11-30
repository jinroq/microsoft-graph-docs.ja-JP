---
title: 招待状の作成
description: この API を使用して、新しい 招待状 を作成します。招待状によって外部ユーザーが組織に追加されます。
ms.openlocfilehash: 6150acd3340ff198e2cc344dcc2fb360314c0320
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27020640"
---
# <a name="create-invitation"></a><span data-ttu-id="257ac-104">招待状の作成</span><span class="sxs-lookup"><span data-stu-id="257ac-104">Create invitation</span></span>

<span data-ttu-id="257ac-p102">この API を使用して、新しい [招待状](../resources/invitation.md) を作成します。招待状によって外部ユーザーが組織に追加されます。</span><span class="sxs-lookup"><span data-stu-id="257ac-p102">Use this API to create a new [invitation](../resources/invitation.md). Invitation adds an external user to the organization.</span></span>

<span data-ttu-id="257ac-107">新しい招待状を作成するときに、選択可能ないくつかのオプションがあります。</span><span class="sxs-lookup"><span data-stu-id="257ac-107">When creating a new invitation you have several options available:</span></span>

1. <span data-ttu-id="257ac-p103">招待状の作成に際して、Microsoft Graph は自動的に招待メールを招待ユーザーに直接送信できます。作成応答で返された *inviteRedeemUrl* をアプリが使用して、招待ユーザーへの (任意の通信メカニズムによる) 独自の招待状を作成することもできます。Microsoft Graph によって招待メールが自動的に送信されるようにする場合は、[*invitedUserMessageInfo*](../resources/invitedusermessageinfo.md) を使用してメールの内容と言語を制御できます。</span><span class="sxs-lookup"><span data-stu-id="257ac-p103">On invitation creation, Microsoft Graph can automatically send an invitation email directly to the invited user, or your app can use the *inviteRedeemUrl* returned in the creation response to craft your own invitation (through your communication mechanism of choice) to the invited user. If you decide to have Microsoft Graph send an invitation email automatically, you can control the content and language of the email using [*invitedUserMessageInfo*](../resources/invitedusermessageinfo.md).</span></span>
2. <span data-ttu-id="257ac-p104">ユーザーが招待されると、(userType Guest) のユーザー エンティティが作成され、リソースへのアクセスの制御に使用できるようになります。招待ユーザーは、招待されたリソースにアクセスするためには、引き換え処理を行う必要があります。</span><span class="sxs-lookup"><span data-stu-id="257ac-p104">When the user is invited, a user entity (of userType Guest) is created and can now be used to control access to resources. The invited user has to go through the redemption process to access any resources he has been invited to.</span></span>

## <a name="permissions"></a><span data-ttu-id="257ac-112">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="257ac-112">Permissions</span></span>
<span data-ttu-id="257ac-p105">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="257ac-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="257ac-115">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="257ac-115">Permission type</span></span>      | <span data-ttu-id="257ac-116">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="257ac-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="257ac-117">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="257ac-117">Delegated (work or school account)</span></span> | <span data-ttu-id="257ac-118">User.Invite.All、User.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="257ac-118">User.Invite.All, User.ReadWrite.All, Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="257ac-119">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="257ac-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="257ac-120">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="257ac-120">Not supported.</span></span>    |
|<span data-ttu-id="257ac-121">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="257ac-121">Application</span></span> | <span data-ttu-id="257ac-122">User.Invite.All、User.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="257ac-122">User.Invite.All, User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="257ac-123">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="257ac-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /invitations
```
## <a name="request-headers"></a><span data-ttu-id="257ac-124">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="257ac-124">Request headers</span></span>
| <span data-ttu-id="257ac-125">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="257ac-125">Header</span></span>       | <span data-ttu-id="257ac-126">値</span><span class="sxs-lookup"><span data-stu-id="257ac-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="257ac-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="257ac-127">Authorization</span></span>  | <span data-ttu-id="257ac-p106">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="257ac-p106">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="257ac-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="257ac-130">Content-Type</span></span>  | <span data-ttu-id="257ac-131">application/json</span><span class="sxs-lookup"><span data-stu-id="257ac-131">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="257ac-132">要求本文</span><span class="sxs-lookup"><span data-stu-id="257ac-132">Request body</span></span>
<span data-ttu-id="257ac-133">要求本文で、[invitation](../resources/invitation.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="257ac-133">In the request body, supply a JSON representation of an [invitation](../resources/invitation.md) object.</span></span>

<span data-ttu-id="257ac-134">次の表に、招待状の作成時に必要になるプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="257ac-134">The following table shows the properties that are required when you create a invitation.</span></span>

| <span data-ttu-id="257ac-135">パラメーター</span><span class="sxs-lookup"><span data-stu-id="257ac-135">Parameter</span></span> | <span data-ttu-id="257ac-136">型</span><span class="sxs-lookup"><span data-stu-id="257ac-136">Type</span></span> | <span data-ttu-id="257ac-137">説明</span><span class="sxs-lookup"><span data-stu-id="257ac-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="257ac-138">invitedUserEmailAddress</span><span class="sxs-lookup"><span data-stu-id="257ac-138">invitedUserEmailAddress</span></span> |<span data-ttu-id="257ac-139">文字列</span><span class="sxs-lookup"><span data-stu-id="257ac-139">string</span></span> | <span data-ttu-id="257ac-140">招待するユーザーのメール アドレス。</span><span class="sxs-lookup"><span data-stu-id="257ac-140">The email address of the user you are inviting.</span></span>|
|<span data-ttu-id="257ac-141">inviteRedirectUrl</span><span class="sxs-lookup"><span data-stu-id="257ac-141">inviteRedirectUrl</span></span> |<span data-ttu-id="257ac-142">文字列</span><span class="sxs-lookup"><span data-stu-id="257ac-142">string</span></span> |<span data-ttu-id="257ac-143">引き換え後にユーザーがリダイレクトされる URL。</span><span class="sxs-lookup"><span data-stu-id="257ac-143">The URL that the user will be redirected to after redemption.</span></span>|

## <a name="response"></a><span data-ttu-id="257ac-144">応答</span><span class="sxs-lookup"><span data-stu-id="257ac-144">Response</span></span>

<span data-ttu-id="257ac-145">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [invitation](../resources/invitation.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="257ac-145">If successful, this method returns `201 Created` response code and [invitation](../resources/invitation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="257ac-146">例</span><span class="sxs-lookup"><span data-stu-id="257ac-146">Example</span></span>
##### <a name="request"></a><span data-ttu-id="257ac-147">要求</span><span class="sxs-lookup"><span data-stu-id="257ac-147">Request</span></span>
<span data-ttu-id="257ac-148">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="257ac-148">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_user_from_users"
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

##### <a name="response"></a><span data-ttu-id="257ac-149">応答</span><span class="sxs-lookup"><span data-stu-id="257ac-149">Response</span></span>
<span data-ttu-id="257ac-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="257ac-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<!-- {
  "type": "#page.annotation",
  "suppressions": [
    "Error: create_user_from_users/invitedUser:
      Property 'invitedUser' is of type Custom but has no custom members."
  ]
}-->
