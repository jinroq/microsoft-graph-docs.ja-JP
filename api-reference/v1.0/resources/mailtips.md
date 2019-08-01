---
title: メールヒントリソースの種類
description: 'メッセージの作成中にユーザーに対して表示される、受信者に関する情報メッセージ。 たとえば、不在時のメッセージ '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 90f6f1a66631223a45a34797b6d18c13259d6241
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36036324"
---
# <a name="mailtips-resource-type"></a><span data-ttu-id="5c230-104">メールヒントリソースの種類</span><span class="sxs-lookup"><span data-stu-id="5c230-104">mailTips resource type</span></span>

<span data-ttu-id="5c230-105">メッセージの作成中にユーザーに対して表示される、受信者に関する情報メッセージ。</span><span class="sxs-lookup"><span data-stu-id="5c230-105">Informative messages about a recipient, that are displayed to users while they are composing a message.</span></span> <span data-ttu-id="5c230-106">たとえば、不在時のメッセージは、メッセージの受信者に対する自動応答として表示されます。</span><span class="sxs-lookup"><span data-stu-id="5c230-106">For example, an out-of-office message as an automatic reply for a message recipient.</span></span>


## <a name="properties"></a><span data-ttu-id="5c230-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5c230-107">Properties</span></span>
| <span data-ttu-id="5c230-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5c230-108">Property</span></span>     | <span data-ttu-id="5c230-109">型</span><span class="sxs-lookup"><span data-stu-id="5c230-109">Type</span></span>   |<span data-ttu-id="5c230-110">説明</span><span class="sxs-lookup"><span data-stu-id="5c230-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="5c230-111">自動応答</span><span class="sxs-lookup"><span data-stu-id="5c230-111">automaticReplies</span></span> | [<span data-ttu-id="5c230-112">automaticRepliesMailTips</span><span class="sxs-lookup"><span data-stu-id="5c230-112">automaticRepliesMailTips</span></span>](../resources/automaticrepliesmailtips.md) | <span data-ttu-id="5c230-113">受信者によって設定されている場合、自動応答のメールヒント。</span><span class="sxs-lookup"><span data-stu-id="5c230-113">Mail tips for automatic reply if it has been set up by the recipient.</span></span> |
| <span data-ttu-id="5c230-114">customMailTip</span><span class="sxs-lookup"><span data-stu-id="5c230-114">customMailTip</span></span> | <span data-ttu-id="5c230-115">String</span><span class="sxs-lookup"><span data-stu-id="5c230-115">String</span></span> | <span data-ttu-id="5c230-116">受信者のメールボックスに設定できるカスタムメールヒント。</span><span class="sxs-lookup"><span data-stu-id="5c230-116">A custom mail tip that can be set on the recipient's mailbox.</span></span> |
| <span data-ttu-id="5c230-117">deliveryRestricted</span><span class="sxs-lookup"><span data-stu-id="5c230-117">deliveryRestricted</span></span>| <span data-ttu-id="5c230-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="5c230-118">Boolean</span></span> | <span data-ttu-id="5c230-119">受信者のメールボックスが制限されているかどうか。たとえば、事前に定義された送信者の一覧からのメッセージの受信、送信者の定義済みリストからのメッセージの拒否、認証済みの送信者からのメッセージの受信のみを行います。</span><span class="sxs-lookup"><span data-stu-id="5c230-119">Whether the recipient's mailbox is restricted, for example, accepting messages from only a predefined list of senders, rejecting messages from a predefined list of senders, or accepting messages from only authenticated senders.</span></span> |
| <span data-ttu-id="5c230-120">emailAddress</span><span class="sxs-lookup"><span data-stu-id="5c230-120">emailAddress</span></span> | [<span data-ttu-id="5c230-121">emailAddress</span><span class="sxs-lookup"><span data-stu-id="5c230-121">emailAddress</span></span>](../resources/emailaddress.md) | <span data-ttu-id="5c230-122">メールヒントを取得する受信者の電子メールアドレス。</span><span class="sxs-lookup"><span data-stu-id="5c230-122">The email address of the recipient to get mailtips for.</span></span> |
| <span data-ttu-id="5c230-123">error</span><span class="sxs-lookup"><span data-stu-id="5c230-123">error</span></span> | [<span data-ttu-id="5c230-124">mailTipsError</span><span class="sxs-lookup"><span data-stu-id="5c230-124">mailTipsError</span></span>](../resources/mailtipserror.md) | <span data-ttu-id="5c230-125">[Getmailtips ヒント](../api/user-getmailtips.md)アクション中に発生するエラー。</span><span class="sxs-lookup"><span data-stu-id="5c230-125">Errors that occur during the [getMailTips](../api/user-getmailtips.md) action.</span></span> |
| <span data-ttu-id="5c230-126">externalMemberCount</span><span class="sxs-lookup"><span data-stu-id="5c230-126">externalMemberCount</span></span> | <span data-ttu-id="5c230-127">Int32</span><span class="sxs-lookup"><span data-stu-id="5c230-127">Int32</span></span> | <span data-ttu-id="5c230-128">受信者が配布リストの場合の外部メンバーの数。</span><span class="sxs-lookup"><span data-stu-id="5c230-128">The number of external members if the recipient is a distribution list.</span></span> |
| <span data-ttu-id="5c230-129">isModerated</span><span class="sxs-lookup"><span data-stu-id="5c230-129">isModerated</span></span> |<span data-ttu-id="5c230-130">Boolean</span><span class="sxs-lookup"><span data-stu-id="5c230-130">Boolean</span></span>  | <span data-ttu-id="5c230-131">受信者にメッセージを送信するには承認が必要であるかどうか。</span><span class="sxs-lookup"><span data-stu-id="5c230-131">Whether sending messages to the recipient requires approval.</span></span> <span data-ttu-id="5c230-132">たとえば、受信者が大きな配布リストであり、その配布リストに送信されたメッセージを承認するようにモデレーターが設定されている場合、または受信者にメッセージを送信する場合は、受信者の上司の承認が必要です。</span><span class="sxs-lookup"><span data-stu-id="5c230-132">For example, if the recipient is a large distribution list and a moderator has been set up to approve messages sent to that distribution list, or if sending messages to a recipient requires approval of the recipient's manager.</span></span> |
| <span data-ttu-id="5c230-133">mailboxFull</span><span class="sxs-lookup"><span data-stu-id="5c230-133">mailboxFull</span></span> | <span data-ttu-id="5c230-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="5c230-134">Boolean</span></span> | <span data-ttu-id="5c230-135">メールボックスのすべての受信者の状態。</span><span class="sxs-lookup"><span data-stu-id="5c230-135">The mailbox full status of the recipient.</span></span> |
| <span data-ttu-id="5c230-136">maxMessageSize</span><span class="sxs-lookup"><span data-stu-id="5c230-136">maxMessageSize</span></span> | <span data-ttu-id="5c230-137">Int32</span><span class="sxs-lookup"><span data-stu-id="5c230-137">Int32</span></span> | <span data-ttu-id="5c230-138">受信者の組織またはメールボックスに対して構成された最大メッセージサイズ。</span><span class="sxs-lookup"><span data-stu-id="5c230-138">The maximum message size that has been configured for the recipient's organization or mailbox.</span></span> |
| <span data-ttu-id="5c230-139">[受信者] スコープ</span><span class="sxs-lookup"><span data-stu-id="5c230-139">recipientScope</span></span> | <span data-ttu-id="5c230-140">recipientScopeType</span><span class="sxs-lookup"><span data-stu-id="5c230-140">recipientScopeType</span></span> | <span data-ttu-id="5c230-141">受信者の範囲。</span><span class="sxs-lookup"><span data-stu-id="5c230-141">The scope of the recipient.</span></span> <span data-ttu-id="5c230-142">可能な値は、`none`、`internal`、`external`、`externalPartner`、`externalNonParther` です。</span><span class="sxs-lookup"><span data-stu-id="5c230-142">Possible values are: `none`, `internal`, `external`, `externalPartner`, `externalNonParther`.</span></span> <span data-ttu-id="5c230-143">たとえば、管理者は別の組織を "パートナー" に設定することができます。</span><span class="sxs-lookup"><span data-stu-id="5c230-143">For example, an administrator can set another organization to be its "partner".</span></span> <span data-ttu-id="5c230-144">特定の範囲で特定のメールヒントにアクセスできるようにするには、スコープを使用すると便利です。</span><span class="sxs-lookup"><span data-stu-id="5c230-144">The scope is useful if an administrator wants certain mailtips to be accessible to certain scopes.</span></span> <span data-ttu-id="5c230-145">また、送信者に対して、メッセージが組織を離れていることを通知し、言葉、語調、およびコンテンツについての正しい判断を支援するためにも役立ちます。</span><span class="sxs-lookup"><span data-stu-id="5c230-145">It's also useful to senders to inform them that their message may leave the organization, helping them make the correct decisions about wording, tone and content.</span></span>|
| <span data-ttu-id="5c230-146">受信者候補</span><span class="sxs-lookup"><span data-stu-id="5c230-146">recipientSuggestions</span></span> | <span data-ttu-id="5c230-147">[recipient](../resources/recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="5c230-147">[recipient](../resources/recipient.md) collection</span></span> | <span data-ttu-id="5c230-148">同じメッセージに表示される以前のコンテキストに基づいて提案される受信者。</span><span class="sxs-lookup"><span data-stu-id="5c230-148">Recipients suggested based on previous contexts where they appear in the same message.</span></span> |
| <span data-ttu-id="5c230-149">totalMemberCount</span><span class="sxs-lookup"><span data-stu-id="5c230-149">totalMemberCount</span></span> | <span data-ttu-id="5c230-150">Int32</span><span class="sxs-lookup"><span data-stu-id="5c230-150">Int32</span></span> | <span data-ttu-id="5c230-151">受信者が配布リストの場合のメンバー数。</span><span class="sxs-lookup"><span data-stu-id="5c230-151">The number of members if the recipient is a distribution list.</span></span> |

### <a name="recipientscopetype-values"></a><span data-ttu-id="5c230-152">recipientScopeType の値</span><span class="sxs-lookup"><span data-stu-id="5c230-152">recipientScopeType values</span></span>

| <span data-ttu-id="5c230-153">値</span><span class="sxs-lookup"><span data-stu-id="5c230-153">Value</span></span>
|:-------------------------
| <span data-ttu-id="5c230-154">none</span><span class="sxs-lookup"><span data-stu-id="5c230-154">none</span></span>
| <span data-ttu-id="5c230-155">社外</span><span class="sxs-lookup"><span data-stu-id="5c230-155">internal</span></span>
| <span data-ttu-id="5c230-156">社外</span><span class="sxs-lookup"><span data-stu-id="5c230-156">external</span></span>
| <span data-ttu-id="5c230-157">externalPartner</span><span class="sxs-lookup"><span data-stu-id="5c230-157">externalPartner</span></span>
| <span data-ttu-id="5c230-158">externalNonPartner</span><span class="sxs-lookup"><span data-stu-id="5c230-158">externalNonPartner</span></span>


## <a name="json-representation"></a><span data-ttu-id="5c230-159">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5c230-159">JSON representation</span></span>

<span data-ttu-id="5c230-160">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="5c230-160">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "automaticReplies",
    "customMailTip",
    "deliveryRestricted",
    "emailAddress",
    "error",
    "externalMemberCount",
    "isModerated",
    "mailboxFull",
    "maxMessageSize",
    "recipientScope",
    "recipientSuggestions",
    "totalMemberCount"
  ],
  "@odata.type": "microsoft.graph.mailTips"
}-->

```json
{
  "automaticReplies": {"@odata.type": "microsoft.graph.automaticRepliesMailTips"},
  "customMailTip": "string",
  "deliveryRestricted": "boolean",
  "emailAddress": {"@odata.type": "microsoft.graph.emailAddress"},
  "error": {"@odata.type": "microsoft.graph.mailTipsError"},
  "externalMemberCount": 1024,
  "isModerated": "boolean",
  "mailboxFull": "boolean",
  "maxMessageSize": 1024,
  "recipientScope": "string",
  "recipientSuggestions": [{"@odata.type": "microsoft.graph.recipient"}],
  "totalMemberCount": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mailtips resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
