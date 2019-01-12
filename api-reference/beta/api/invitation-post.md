---
title: 招待状の作成
description: この API を使用して、新しい 招待状 を作成します。招待状によって外部ユーザーが組織に追加されます。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 4ec0fce295046182c93ccb36ecab3706ad787f80
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27983668"
---
# <a name="create-invitation"></a><span data-ttu-id="8a5a1-104">招待状の作成</span><span class="sxs-lookup"><span data-stu-id="8a5a1-104">Create invitation</span></span>

> <span data-ttu-id="8a5a1-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="8a5a1-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8a5a1-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8a5a1-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8a5a1-p103">この API を使用して、新しい [招待状](../resources/invitation.md) を作成します。招待状によって外部ユーザーが組織に追加されます。</span><span class="sxs-lookup"><span data-stu-id="8a5a1-p103">Use this API to create a new [invitation](../resources/invitation.md). Invitation adds an external user to the organization.</span></span>

<span data-ttu-id="8a5a1-109">新しい招待状を作成するときに、選択可能ないくつかのオプションがあります。</span><span class="sxs-lookup"><span data-stu-id="8a5a1-109">When creating a new invitation you have several options available:</span></span>

1. <span data-ttu-id="8a5a1-p104">招待状の作成に際して、Microsoft Graph は自動的に招待メールを招待ユーザーに直接送信できます。作成応答で返された *inviteRedeemUrl* をアプリが使用して、招待ユーザーへの (任意の通信メカニズムによる) 独自の招待状を作成することもできます。Microsoft Graph によって招待メールが自動的に送信されるようにする場合は、[*invitedUserMessageInfo*](../resources/invitedusermessageinfo.md) を使用してメールの内容と言語を制御できます。</span><span class="sxs-lookup"><span data-stu-id="8a5a1-p104">On invitation creation, Microsoft Graph can automatically send an invitation email directly to the invited user, or your app can use the *inviteRedeemUrl* returned in the creation response to craft your own invitation (through your communication mechanism of choice) to the invited user. If you decide to have Microsoft Graph send an invitation email automatically, you can control the content and language of the email using [*invitedUserMessageInfo*](../resources/invitedusermessageinfo.md).</span></span>
2. <span data-ttu-id="8a5a1-p105">ユーザーが招待されると、(userType Guest) のユーザー エンティティが作成され、リソースへのアクセスの制御に使用できるようになります。招待ユーザーは、招待されたリソースにアクセスするためには、引き換え処理を行う必要があります。</span><span class="sxs-lookup"><span data-stu-id="8a5a1-p105">When the user is invited, a user entity (of userType Guest) is created and can now be used to control access to resources. The invited user has to go through the redemption process to access any resources he has been invited to.</span></span>

## <a name="permissions"></a><span data-ttu-id="8a5a1-114">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8a5a1-114">Permissions</span></span>
<span data-ttu-id="8a5a1-p106">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8a5a1-p106">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="8a5a1-117">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8a5a1-117">Permission type</span></span>      | <span data-ttu-id="8a5a1-118">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="8a5a1-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8a5a1-119">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8a5a1-119">Delegated (work or school account)</span></span> | <span data-ttu-id="8a5a1-120">User.Invite.All、User.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a5a1-120">User.Invite.All, User.ReadWrite.All, Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="8a5a1-121">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8a5a1-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8a5a1-122">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8a5a1-122">Not supported.</span></span>    |
|<span data-ttu-id="8a5a1-123">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8a5a1-123">Application</span></span> | <span data-ttu-id="8a5a1-124">User.Invite.All、User.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a5a1-124">User.Invite.All, User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8a5a1-125">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8a5a1-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /invitations
```
## <a name="request-headers"></a><span data-ttu-id="8a5a1-126">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8a5a1-126">Request headers</span></span>
| <span data-ttu-id="8a5a1-127">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8a5a1-127">Header</span></span>       | <span data-ttu-id="8a5a1-128">値</span><span class="sxs-lookup"><span data-stu-id="8a5a1-128">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8a5a1-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="8a5a1-129">Authorization</span></span>  | <span data-ttu-id="8a5a1-p107">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="8a5a1-p107">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="8a5a1-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8a5a1-132">Content-Type</span></span>  | <span data-ttu-id="8a5a1-133">application/json</span><span class="sxs-lookup"><span data-stu-id="8a5a1-133">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8a5a1-134">要求本文</span><span class="sxs-lookup"><span data-stu-id="8a5a1-134">Request body</span></span>
<span data-ttu-id="8a5a1-135">要求本文で、[invitation](../resources/invitation.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="8a5a1-135">In the request body, supply a JSON representation of an [invitation](../resources/invitation.md) object.</span></span>

<span data-ttu-id="8a5a1-136">次の表に、招待状の作成時に必要になるプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="8a5a1-136">The following table shows the properties that are required when you create a invitation.</span></span>

| <span data-ttu-id="8a5a1-137">パラメーター</span><span class="sxs-lookup"><span data-stu-id="8a5a1-137">Parameter</span></span> | <span data-ttu-id="8a5a1-138">型</span><span class="sxs-lookup"><span data-stu-id="8a5a1-138">Type</span></span> | <span data-ttu-id="8a5a1-139">説明</span><span class="sxs-lookup"><span data-stu-id="8a5a1-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8a5a1-140">invitedUserEmailAddress</span><span class="sxs-lookup"><span data-stu-id="8a5a1-140">invitedUserEmailAddress</span></span> |<span data-ttu-id="8a5a1-141">文字列</span><span class="sxs-lookup"><span data-stu-id="8a5a1-141">string</span></span> | <span data-ttu-id="8a5a1-142">招待するユーザーのメール アドレス。</span><span class="sxs-lookup"><span data-stu-id="8a5a1-142">The email address of the user you are inviting.</span></span>|
|<span data-ttu-id="8a5a1-143">inviteRedirectUrl</span><span class="sxs-lookup"><span data-stu-id="8a5a1-143">inviteRedirectUrl</span></span> |<span data-ttu-id="8a5a1-144">文字列</span><span class="sxs-lookup"><span data-stu-id="8a5a1-144">string</span></span> |<span data-ttu-id="8a5a1-145">引き換え後にユーザーがリダイレクトされる URL。</span><span class="sxs-lookup"><span data-stu-id="8a5a1-145">The URL that the user will be redirected to after redemption.</span></span>|

## <a name="response"></a><span data-ttu-id="8a5a1-146">応答</span><span class="sxs-lookup"><span data-stu-id="8a5a1-146">Response</span></span>

<span data-ttu-id="8a5a1-147">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [invitation](../resources/invitation.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="8a5a1-147">If successful, this method returns `201 Created` response code and [invitation](../resources/invitation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8a5a1-148">例</span><span class="sxs-lookup"><span data-stu-id="8a5a1-148">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8a5a1-149">要求</span><span class="sxs-lookup"><span data-stu-id="8a5a1-149">Request</span></span>
<span data-ttu-id="8a5a1-150">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8a5a1-150">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_user_from_users"
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

##### <a name="response"></a><span data-ttu-id="8a5a1-151">応答</span><span class="sxs-lookup"><span data-stu-id="8a5a1-151">Response</span></span>
<span data-ttu-id="8a5a1-p108">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8a5a1-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.invitations"
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
