---
title: 招待マネージャー
description: '招待マネージャーを使用して、組織に外部ユーザーを追加するための招待状を作成します。 '
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 72ff2ca13a0de314697961504da9a4203afdb2b1
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27981050"
---
# <a name="invitation-manager"></a><span data-ttu-id="0816f-103">招待マネージャー</span><span class="sxs-lookup"><span data-stu-id="0816f-103">invitation manager</span></span>

> <span data-ttu-id="0816f-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="0816f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0816f-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0816f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0816f-106">招待マネージャーを使用して、組織に外部ユーザーを追加するための招待状を作成します。</span><span class="sxs-lookup"><span data-stu-id="0816f-106">Use the invitation manager to create an invite, in order to add an external user to the organization.</span></span> 

<span data-ttu-id="0816f-107">招待処理では、次のフローが使用されます。</span><span class="sxs-lookup"><span data-stu-id="0816f-107">The invitation process uses the following flow:</span></span>

* <span data-ttu-id="0816f-108">招待状が作成されます。</span><span class="sxs-lookup"><span data-stu-id="0816f-108">An invitation is created</span></span>
* <span data-ttu-id="0816f-109">招待状が招待ユーザーに送信されます (招待状リンクを含む)。</span><span class="sxs-lookup"><span data-stu-id="0816f-109">An invitation is sent to the invited user (containing an invitation link)</span></span>
* <span data-ttu-id="0816f-110">招待ユーザーが招待状リンクをクリックしてサインインし、招待状を引き換え、招待ユーザーを表すユーザー エンティティの作成が完了します。</span><span class="sxs-lookup"><span data-stu-id="0816f-110">The invited user clicks on the invitation link, signs in and redeems the invitation and creation of the user entity representing the invited user completes</span></span>
* <span data-ttu-id="0816f-111">引き換えが完了した後、特定のページにユーザーがリダイレクトされます。</span><span class="sxs-lookup"><span data-stu-id="0816f-111">The user is redirected to a specific page after redemption completes</span></span>

<span data-ttu-id="0816f-p102">招待状を作成すると、応答で引き換え URL が返されます (*inviteRedeemUrl*)。招待状作成 API では、*sendInvitationMessage* を true に設定することにより、引き換え URL を含むメールが自動的に招待ユーザーに送信されます。招待ユーザーに送信されるメッセージをカスタマイズすることもできます。代わりに、他の手段で引き換え URL を送信したい場合は、*sendInvitationMessage* を false に設定し、応答からの引き換え URL を使用して、独自の通信を作成することもできます。現在、引き換え処理を実行するための API はありません。招待ユーザーは、上記手順の通信で送信された *inviteRedeemUrl* リンクをクリックして、対話型引き換え処理をブラウザーで行う必要があります。完了すると、招待ユーザーは、組織における外部ユーザーになります。</span><span class="sxs-lookup"><span data-stu-id="0816f-p102">Creating an invitation will return a redemption URL in the response (*inviteRedeemUrl*). The create invitation API can automatically send an email containing the redemption URL to the invited user, by setting the *sendInvitationMessage* to true. You can also customize the message that will be sent to the invited user. Instead, if you wish to send the redemption URL through some other means, you can set the *sendInvitationMessage* to false and use the redeem URL from the response to craft your own communication. Currently, there is no API to perform the redemption process. The invited user has to click on the *inviteRedeemUrl* link sent in the communication in the step above, and go through the interactive redemption process in a browser. Once completed, the invited user becomes an external user in the organization.</span></span>


## <a name="methods"></a><span data-ttu-id="0816f-119">メソッド</span><span class="sxs-lookup"><span data-stu-id="0816f-119">Methods</span></span>
| <span data-ttu-id="0816f-120">メソッド</span><span class="sxs-lookup"><span data-stu-id="0816f-120">Method</span></span>       | <span data-ttu-id="0816f-121">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="0816f-121">Return Type</span></span>  |<span data-ttu-id="0816f-122">説明</span><span class="sxs-lookup"><span data-stu-id="0816f-122">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0816f-123">招待状の作成</span><span class="sxs-lookup"><span data-stu-id="0816f-123">Create invitation</span></span>](../api/invitation-post.md) | <span data-ttu-id="0816f-124">invitation</span><span class="sxs-lookup"><span data-stu-id="0816f-124">invitation</span></span> | <span data-ttu-id="0816f-125">招待状オブジェクトのプロパティと関係を書き込みます。</span><span class="sxs-lookup"><span data-stu-id="0816f-125">Write properties and relationships of invitation object.</span></span>|

## <a name="properties"></a><span data-ttu-id="0816f-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0816f-126">Properties</span></span>
| <span data-ttu-id="0816f-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0816f-127">Property</span></span>     | <span data-ttu-id="0816f-128">種類</span><span class="sxs-lookup"><span data-stu-id="0816f-128">Type</span></span>   |<span data-ttu-id="0816f-129">説明</span><span class="sxs-lookup"><span data-stu-id="0816f-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0816f-130">invitedUserDisplayName</span><span class="sxs-lookup"><span data-stu-id="0816f-130">invitedUserDisplayName</span></span>|<span data-ttu-id="0816f-131">String</span><span class="sxs-lookup"><span data-stu-id="0816f-131">String</span></span>|<span data-ttu-id="0816f-132">招待されるユーザーの表示名。</span><span class="sxs-lookup"><span data-stu-id="0816f-132">The display name of the user being invited.</span></span>|
|<span data-ttu-id="0816f-133">invitedUserEmailAddress</span><span class="sxs-lookup"><span data-stu-id="0816f-133">invitedUserEmailAddress</span></span>|<span data-ttu-id="0816f-134">String</span><span class="sxs-lookup"><span data-stu-id="0816f-134">String</span></span>|<span data-ttu-id="0816f-p103">招待されるユーザーのメール アドレス。必須。</span><span class="sxs-lookup"><span data-stu-id="0816f-p103">The email address of the user being invited. Required.</span></span>|
|<span data-ttu-id="0816f-137">invitedUserMessageInfo</span><span class="sxs-lookup"><span data-stu-id="0816f-137">invitedUserMessageInfo</span></span>|[<span data-ttu-id="0816f-138">invitedUserMessageInfo</span><span class="sxs-lookup"><span data-stu-id="0816f-138">invitedUserMessageInfo</span></span>](invitedusermessageinfo.md)|<span data-ttu-id="0816f-139">メッセージ テキスト、言語、および cc 受信者リストのカスタマイズなど、招待ユーザーに送信されるメッセージの追加構成。</span><span class="sxs-lookup"><span data-stu-id="0816f-139">Additional configuration for the message being sent to the invited user, including customizing message text, language and cc recipient list.</span></span>|
|<span data-ttu-id="0816f-140">sendInvitationMessage</span><span class="sxs-lookup"><span data-stu-id="0816f-140">sendInvitationMessage</span></span>|<span data-ttu-id="0816f-141">ブール値</span><span class="sxs-lookup"><span data-stu-id="0816f-141">Boolean</span></span>|<span data-ttu-id="0816f-p104">招待されるユーザーにメールを送信するかどうかを示します。既定値は false です。</span><span class="sxs-lookup"><span data-stu-id="0816f-p104">Indicates whether an email should be sent to the user being invited or not. The default is false.</span></span>|
|<span data-ttu-id="0816f-144">inviteRedirectUrl</span><span class="sxs-lookup"><span data-stu-id="0816f-144">inviteRedirectUrl</span></span>|<span data-ttu-id="0816f-145">String</span><span class="sxs-lookup"><span data-stu-id="0816f-145">String</span></span>|<span data-ttu-id="0816f-p105">招待状が引き換えられるとにユーザーがリダイレクトされる URL。必須。</span><span class="sxs-lookup"><span data-stu-id="0816f-p105">The URL user should be redirected to once the invitation is redeemed. Required.</span></span>|
|<span data-ttu-id="0816f-148">inviteRedeemUrl</span><span class="sxs-lookup"><span data-stu-id="0816f-148">inviteRedeemUrl</span></span>|<span data-ttu-id="0816f-149">String</span><span class="sxs-lookup"><span data-stu-id="0816f-149">String</span></span>|<span data-ttu-id="0816f-p106">ユーザーが招待状の引き換えに使用できる URL。読み取り専用</span><span class="sxs-lookup"><span data-stu-id="0816f-p106">The URL user can use to redeem his invitation. Read-Only</span></span>|
|<span data-ttu-id="0816f-152">invitedUserType</span><span class="sxs-lookup"><span data-stu-id="0816f-152">invitedUserType</span></span>|<span data-ttu-id="0816f-153">String</span><span class="sxs-lookup"><span data-stu-id="0816f-153">String</span></span>|<span data-ttu-id="0816f-p107">招待されるユーザーの userType。既定では Guest です。会社の管理者は、Member として招待できます。</span><span class="sxs-lookup"><span data-stu-id="0816f-p107">The userType of the user being invited. By default, this is Guest. You can invite as Member if you're are company administrator.</span></span> |
|<span data-ttu-id="0816f-157">status</span><span class="sxs-lookup"><span data-stu-id="0816f-157">status</span></span>|<span data-ttu-id="0816f-158">String</span><span class="sxs-lookup"><span data-stu-id="0816f-158">String</span></span>|<span data-ttu-id="0816f-p108">招待の状態。可能な値:PendingAcceptance、Completed、InProgress、および Error</span><span class="sxs-lookup"><span data-stu-id="0816f-p108">The status of the invitation. Possible values: PendingAcceptance, Completed, InProgress, and Error</span></span>|

## <a name="relationships"></a><span data-ttu-id="0816f-161">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0816f-161">Relationships</span></span>
| <span data-ttu-id="0816f-162">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0816f-162">Relationship</span></span> | <span data-ttu-id="0816f-163">型</span><span class="sxs-lookup"><span data-stu-id="0816f-163">Type</span></span>   |<span data-ttu-id="0816f-164">説明</span><span class="sxs-lookup"><span data-stu-id="0816f-164">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0816f-165">invitedUser</span><span class="sxs-lookup"><span data-stu-id="0816f-165">invitedUser</span></span>|[<span data-ttu-id="0816f-166">User</span><span class="sxs-lookup"><span data-stu-id="0816f-166">User</span></span>](user.md)|<span data-ttu-id="0816f-p109">招待状作成の一環として作成されたユーザー。読み取り専用</span><span class="sxs-lookup"><span data-stu-id="0816f-p109">The user created as part of the invitation creation. Read-Only</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0816f-169">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0816f-169">JSON representation</span></span>
<span data-ttu-id="0816f-170">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="0816f-170">Here is a JSON representation of the resource</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.invitations" } -->
```json
{
  "invitedUserDisplayName": "string",
  "invitedUserEmailAddress": "string",
  "invitedUserMessageInfo": {"@odata.type": "microsoft.graph.invitedUserMessageInfo"},
  "sendInvitationMessage": false,
  "inviteRedirectUrl": "string",
  "inviteRedeemUrl": "string",
  "status": "string",

  "invitedUser": [{"@odata.type": "microsoft.graph.user"}]
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2016-22-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "invitation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
