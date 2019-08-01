---
title: 招待リソースの種類
description: 組織に外部ユーザーを追加するために使用される招待を表します。
localization_priority: Priority
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 4b6ea88a0e07fb74f2ec3834902f175e78906f68
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36036737"
---
# <a name="invitation-resource-type"></a><span data-ttu-id="4416d-103">招待リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4416d-103">invitation resource type</span></span>

<span data-ttu-id="4416d-104">組織に外部ユーザーを追加するために使用される招待を表します。</span><span class="sxs-lookup"><span data-stu-id="4416d-104">Represents an invitation that is used to add external users to an organization.</span></span> 

<span data-ttu-id="4416d-105">招待処理では、次のフローが使用されます。</span><span class="sxs-lookup"><span data-stu-id="4416d-105">The invitation process uses the following flow:</span></span>

* <span data-ttu-id="4416d-106">招待状が作成されます。</span><span class="sxs-lookup"><span data-stu-id="4416d-106">An invitation is created</span></span>
* <span data-ttu-id="4416d-107">招待状が招待ユーザーに送信されます (招待状リンクを含む)。</span><span class="sxs-lookup"><span data-stu-id="4416d-107">An invitation is sent to the invited user (containing an invitation link)</span></span>
* <span data-ttu-id="4416d-108">招待ユーザーが招待状リンクをクリックしてサインインし、招待状を引き換え、招待ユーザーを表すユーザー エンティティの作成が完了します。</span><span class="sxs-lookup"><span data-stu-id="4416d-108">The invited user clicks on the invitation link, signs in and redeems the invitation and creation of the user entity representing the invited user completes</span></span>
* <span data-ttu-id="4416d-109">引き換えが完了した後、特定のページにユーザーがリダイレクトされます。</span><span class="sxs-lookup"><span data-stu-id="4416d-109">The user is redirected to a specific page after redemption completes</span></span>

<span data-ttu-id="4416d-p101">招待状を作成すると、応答で引き換え URL が返されます (*inviteRedeemUrl*)。招待状作成 API では、*sendInvitationMessage* を true に設定することにより、引き換え URL を含むメールが自動的に招待ユーザーに送信されます。招待ユーザーに送信されるメッセージをカスタマイズすることもできます。代わりに、他の手段で引き換え URL を送信したい場合は、*sendInvitationMessage* を false に設定し、応答からの引き換え URL を使用して、独自の通信を作成することもできます。現在、引き換え処理を実行するための API はありません。招待ユーザーは、上記手順の通信で送信された *inviteRedeemUrl* リンクをクリックして、対話型引き換え処理をブラウザーで行う必要があります。完了すると、招待ユーザーは、組織における外部ユーザーになります。</span><span class="sxs-lookup"><span data-stu-id="4416d-p101">Creating an invitation will return a redemption URL in the response (*inviteRedeemUrl*). The create invitation API can automatically send an email containing the redemption URL to the invited user, by setting the *sendInvitationMessage* to true. You can also customize the message that will be sent to the invited user. Instead, if you wish to send the redemption URL through some other means, you can set the *sendInvitationMessage* to false and use the redeem URL from the response to craft your own communication. Currently, there is no API to perform the redemption process. The invited user has to click on the *inviteRedeemUrl* link sent in the communication in the step above, and go through the interactive redemption process in a browser. Once completed, the invited user becomes an external user in the organization.</span></span>


## <a name="methods"></a><span data-ttu-id="4416d-117">メソッド</span><span class="sxs-lookup"><span data-stu-id="4416d-117">Methods</span></span>
| <span data-ttu-id="4416d-118">メソッド</span><span class="sxs-lookup"><span data-stu-id="4416d-118">Method</span></span>       | <span data-ttu-id="4416d-119">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="4416d-119">Return Type</span></span>  |<span data-ttu-id="4416d-120">説明</span><span class="sxs-lookup"><span data-stu-id="4416d-120">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4416d-121">招待状の作成</span><span class="sxs-lookup"><span data-stu-id="4416d-121">Create invitation</span></span>](../api/invitation-post.md) | <span data-ttu-id="4416d-122">invitation</span><span class="sxs-lookup"><span data-stu-id="4416d-122">invitation</span></span> | <span data-ttu-id="4416d-123">招待状オブジェクトのプロパティと関係を書き込みます。</span><span class="sxs-lookup"><span data-stu-id="4416d-123">Write properties and relationships of invitation object.</span></span>|

## <a name="properties"></a><span data-ttu-id="4416d-124">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4416d-124">Properties</span></span>
| <span data-ttu-id="4416d-125">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4416d-125">Property</span></span>     | <span data-ttu-id="4416d-126">型</span><span class="sxs-lookup"><span data-stu-id="4416d-126">Type</span></span>   |<span data-ttu-id="4416d-127">説明</span><span class="sxs-lookup"><span data-stu-id="4416d-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4416d-128">invitedUserDisplayName</span><span class="sxs-lookup"><span data-stu-id="4416d-128">invitedUserDisplayName</span></span>|<span data-ttu-id="4416d-129">String</span><span class="sxs-lookup"><span data-stu-id="4416d-129">String</span></span>|<span data-ttu-id="4416d-130">招待されるユーザーの表示名。</span><span class="sxs-lookup"><span data-stu-id="4416d-130">The display name of the user being invited.</span></span>|
|<span data-ttu-id="4416d-131">invitedUserEmailAddress</span><span class="sxs-lookup"><span data-stu-id="4416d-131">invitedUserEmailAddress</span></span>|<span data-ttu-id="4416d-132">String</span><span class="sxs-lookup"><span data-stu-id="4416d-132">String</span></span>|<span data-ttu-id="4416d-p102">招待されるユーザーのメール アドレス。必須。</span><span class="sxs-lookup"><span data-stu-id="4416d-p102">The email address of the user being invited. Required.</span></span>|
|<span data-ttu-id="4416d-135">invitedUserMessageInfo</span><span class="sxs-lookup"><span data-stu-id="4416d-135">invitedUserMessageInfo</span></span>|[<span data-ttu-id="4416d-136">invitedUserMessageInfo</span><span class="sxs-lookup"><span data-stu-id="4416d-136">invitedUserMessageInfo</span></span>](invitedusermessageinfo.md)|<span data-ttu-id="4416d-137">メッセージ テキスト、言語、および cc 受信者リストのカスタマイズなど、招待ユーザーに送信されるメッセージの追加構成。</span><span class="sxs-lookup"><span data-stu-id="4416d-137">Additional configuration for the message being sent to the invited user, including customizing message text, language and cc recipient list.</span></span>|
|<span data-ttu-id="4416d-138">sendInvitationMessage</span><span class="sxs-lookup"><span data-stu-id="4416d-138">sendInvitationMessage</span></span>|<span data-ttu-id="4416d-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="4416d-139">Boolean</span></span>|<span data-ttu-id="4416d-p103">招待されるユーザーにメールを送信するかどうかを示します。既定値は false です。</span><span class="sxs-lookup"><span data-stu-id="4416d-p103">Indicates whether an email should be sent to the user being invited or not. The default is false.</span></span>|
|<span data-ttu-id="4416d-142">inviteRedirectUrl</span><span class="sxs-lookup"><span data-stu-id="4416d-142">inviteRedirectUrl</span></span>|<span data-ttu-id="4416d-143">String</span><span class="sxs-lookup"><span data-stu-id="4416d-143">String</span></span>|<span data-ttu-id="4416d-p104">招待状が引き換えられるとにユーザーがリダイレクトされる URL。必須。</span><span class="sxs-lookup"><span data-stu-id="4416d-p104">The URL user should be redirected to once the invitation is redeemed. Required.</span></span>|
|<span data-ttu-id="4416d-146">inviteRedeemUrl</span><span class="sxs-lookup"><span data-stu-id="4416d-146">inviteRedeemUrl</span></span>|<span data-ttu-id="4416d-147">String</span><span class="sxs-lookup"><span data-stu-id="4416d-147">String</span></span>|<span data-ttu-id="4416d-p105">ユーザーが招待状の引き換えに使用できる URL。読み取り専用</span><span class="sxs-lookup"><span data-stu-id="4416d-p105">The URL user can use to redeem his invitation. Read-Only</span></span>|
|<span data-ttu-id="4416d-150">invitedUserType</span><span class="sxs-lookup"><span data-stu-id="4416d-150">invitedUserType</span></span>|<span data-ttu-id="4416d-151">String</span><span class="sxs-lookup"><span data-stu-id="4416d-151">String</span></span>|<span data-ttu-id="4416d-152">招待されるユーザーの userType。</span><span class="sxs-lookup"><span data-stu-id="4416d-152">The userType of the user being invited.</span></span> <span data-ttu-id="4416d-153">既定では Guest です。</span><span class="sxs-lookup"><span data-stu-id="4416d-153">By default, this is Guest.</span></span> <span data-ttu-id="4416d-154">会社の管理者の場合は、Member として招待できます。</span><span class="sxs-lookup"><span data-stu-id="4416d-154">You can invite as Member if you are a company administrator.</span></span> |
|<span data-ttu-id="4416d-155">status</span><span class="sxs-lookup"><span data-stu-id="4416d-155">status</span></span>|<span data-ttu-id="4416d-156">String</span><span class="sxs-lookup"><span data-stu-id="4416d-156">String</span></span>|<span data-ttu-id="4416d-p107">招待の状態。可能な値:PendingAcceptance、Completed、InProgress、および Error</span><span class="sxs-lookup"><span data-stu-id="4416d-p107">The status of the invitation. Possible values: PendingAcceptance, Completed, InProgress, and Error</span></span>|

## <a name="relationships"></a><span data-ttu-id="4416d-159">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="4416d-159">Relationships</span></span>
| <span data-ttu-id="4416d-160">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="4416d-160">Relationship</span></span> | <span data-ttu-id="4416d-161">型</span><span class="sxs-lookup"><span data-stu-id="4416d-161">Type</span></span>   |<span data-ttu-id="4416d-162">説明</span><span class="sxs-lookup"><span data-stu-id="4416d-162">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4416d-163">invitedUser</span><span class="sxs-lookup"><span data-stu-id="4416d-163">invitedUser</span></span>|[<span data-ttu-id="4416d-164">User</span><span class="sxs-lookup"><span data-stu-id="4416d-164">User</span></span>](user.md)|<span data-ttu-id="4416d-p108">招待状作成の一環として作成されたユーザー。読み取り専用</span><span class="sxs-lookup"><span data-stu-id="4416d-p108">The user created as part of the invitation creation. Read-Only</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4416d-167">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4416d-167">JSON representation</span></span>
<span data-ttu-id="4416d-168">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="4416d-168">Here is a JSON representation of the resource</span></span>

<!-- { "blockType": "resource", "baseType": "microsoft.graph.entity", "@odata.type": "microsoft.graph.invitation" } -->
```json
{
  "invitedUserDisplayName": "string",
  "invitedUserEmailAddress": "string",
  "invitedUserMessageInfo": {"@odata.type": "microsoft.graph.invitedUserMessageInfo"},
  "sendInvitationMessage": false,
  "inviteRedirectUrl": "string",
  "inviteRedeemUrl": "string",
  "status": "string",
  "invitedUser": {"@odata.type": "microsoft.graph.user"},
  "invitedUserType": "string"
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
