---
title: リソースの種類のメール ヒント
description: 'メッセージの作成中にユーザーに表示される、受信者に関する情報メッセージです。 たとえば、不在時のメッセージ '
localization_priority: Normal
ms.openlocfilehash: 0506d10ad4b1c5eb473b04a30eb8d48334685574
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27891694"
---
# <a name="mailtips-resource-type"></a><span data-ttu-id="8e28d-104">リソースの種類のメール ヒント</span><span class="sxs-lookup"><span data-stu-id="8e28d-104">mailTips resource type</span></span>

<span data-ttu-id="8e28d-105">メッセージの作成中にユーザーに表示される、受信者に関する情報メッセージです。</span><span class="sxs-lookup"><span data-stu-id="8e28d-105">Informative messages about a recipient, that are displayed to users while they are composing a message.</span></span> <span data-ttu-id="8e28d-106">など、不在時のメッセージ、自動返信メッセージの受信者として。</span><span class="sxs-lookup"><span data-stu-id="8e28d-106">For example, an out-of-office message as an automatic reply for a message recipient.</span></span>


## <a name="properties"></a><span data-ttu-id="8e28d-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8e28d-107">Properties</span></span>
| <span data-ttu-id="8e28d-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8e28d-108">Property</span></span>     | <span data-ttu-id="8e28d-109">種類</span><span class="sxs-lookup"><span data-stu-id="8e28d-109">Type</span></span>   |<span data-ttu-id="8e28d-110">説明</span><span class="sxs-lookup"><span data-stu-id="8e28d-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="8e28d-111">automaticReplies</span><span class="sxs-lookup"><span data-stu-id="8e28d-111">automaticReplies</span></span> | [<span data-ttu-id="8e28d-112">automaticRepliesMailTips</span><span class="sxs-lookup"><span data-stu-id="8e28d-112">automaticRepliesMailTips</span></span>](../resources/automaticrepliesmailtips.md) | <span data-ttu-id="8e28d-113">受信者によって設定されている場合の自動応答に関するメールのヒント。</span><span class="sxs-lookup"><span data-stu-id="8e28d-113">Mail tips for automatic reply if it has been set up by the recipient.</span></span> |
| <span data-ttu-id="8e28d-114">customMailTip</span><span class="sxs-lookup"><span data-stu-id="8e28d-114">customMailTip</span></span> | <span data-ttu-id="8e28d-115">String</span><span class="sxs-lookup"><span data-stu-id="8e28d-115">String</span></span> | <span data-ttu-id="8e28d-116">受信者のメールボックスに設定可能なカスタム メールのヒント。</span><span class="sxs-lookup"><span data-stu-id="8e28d-116">A custom mail tip that can be set on the recipient's mailbox.</span></span> |
| <span data-ttu-id="8e28d-117">deliveryRestricted</span><span class="sxs-lookup"><span data-stu-id="8e28d-117">deliveryRestricted</span></span>| <span data-ttu-id="8e28d-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="8e28d-118">Boolean</span></span> | <span data-ttu-id="8e28d-119">受信者のメールボックスが制限されているかどうか。たとえば、送信者の定義済みリストからのメッセージのみを受け付ける、送信者の定義済みリストからのメッセージを拒否する、または認証された送信者からのメッセージのみを受信するなどです。</span><span class="sxs-lookup"><span data-stu-id="8e28d-119">Whether the recipient's mailbox is restricted, for example, accepting messages from only a predefined list of senders, rejecting messages from a predefined list of senders, or accepting messages from only authenticated senders.</span></span> |
| <span data-ttu-id="8e28d-120">emailAddress</span><span class="sxs-lookup"><span data-stu-id="8e28d-120">emailAddress</span></span> | [<span data-ttu-id="8e28d-121">emailAddress</span><span class="sxs-lookup"><span data-stu-id="8e28d-121">emailAddress</span></span>](../resources/emailaddress.md) | <span data-ttu-id="8e28d-122">メールヒントを取得する受信者の電子メール アドレス。</span><span class="sxs-lookup"><span data-stu-id="8e28d-122">The email address of the recipient to get mailtips for.</span></span> |
| <span data-ttu-id="8e28d-123">エラー</span><span class="sxs-lookup"><span data-stu-id="8e28d-123">error</span></span> | [<span data-ttu-id="8e28d-124">mailTipsError</span><span class="sxs-lookup"><span data-stu-id="8e28d-124">mailTipsError</span></span>](../resources/mailtipserror.md) | <span data-ttu-id="8e28d-125">[GetMailTips](../api/user-getmailtips.md)操作中に発生するエラーです。</span><span class="sxs-lookup"><span data-stu-id="8e28d-125">Errors that occur during the [getMailTips](../api/user-getmailtips.md) action.</span></span> |
| <span data-ttu-id="8e28d-126">externalMemberCount</span><span class="sxs-lookup"><span data-stu-id="8e28d-126">externalMemberCount</span></span> | <span data-ttu-id="8e28d-127">Int32</span><span class="sxs-lookup"><span data-stu-id="8e28d-127">Int32</span></span> | <span data-ttu-id="8e28d-128">受信者が配布リストの場合は外部メンバーの数です。</span><span class="sxs-lookup"><span data-stu-id="8e28d-128">The number of external members if the recipient is a distribution list.</span></span> |
| <span data-ttu-id="8e28d-129">isModerated</span><span class="sxs-lookup"><span data-stu-id="8e28d-129">isModerated</span></span> |<span data-ttu-id="8e28d-130">Boolean</span><span class="sxs-lookup"><span data-stu-id="8e28d-130">Boolean</span></span>  | <span data-ttu-id="8e28d-p103">受信者へのメッセージ送信に承認が必要かどうか。たとえば、受信者が大規模な配布リストであり、モデレーターが配布リストに送信されたメッセージを承認するようにセットアップされている場合、または受信者へのメッセージの送信に受信者の上司の承認を必要とする場合などです。</span><span class="sxs-lookup"><span data-stu-id="8e28d-p103">Whether sending messages to the recipient requires approval. For example, if the recipient is a large distribution list and a moderator has been set up to approve messages sent to that distribution list, or if sending messages to a recipient requires approval of the recipient's manager.</span></span> |
| <span data-ttu-id="8e28d-133">mailboxFull</span><span class="sxs-lookup"><span data-stu-id="8e28d-133">mailboxFull</span></span> | <span data-ttu-id="8e28d-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="8e28d-134">Boolean</span></span> | <span data-ttu-id="8e28d-135">受信者のメールボックスのフル状態。</span><span class="sxs-lookup"><span data-stu-id="8e28d-135">The mailbox full status of the recipient.</span></span> |
| <span data-ttu-id="8e28d-136">maxMessageSize</span><span class="sxs-lookup"><span data-stu-id="8e28d-136">maxMessageSize</span></span> | <span data-ttu-id="8e28d-137">Int32</span><span class="sxs-lookup"><span data-stu-id="8e28d-137">Int32</span></span> | <span data-ttu-id="8e28d-138">受信者の組織またはメールボックスに対して構成されているメッセージの最大サイズ。</span><span class="sxs-lookup"><span data-stu-id="8e28d-138">The maximum message size that has been configured for the recipient's organization or mailbox.</span></span> |
| <span data-ttu-id="8e28d-139">recipientScope</span><span class="sxs-lookup"><span data-stu-id="8e28d-139">recipientScope</span></span> | <span data-ttu-id="8e28d-140">recipientScopeType</span><span class="sxs-lookup"><span data-stu-id="8e28d-140">recipientScopeType</span></span> | <span data-ttu-id="8e28d-141">受信者のスコープ。</span><span class="sxs-lookup"><span data-stu-id="8e28d-141">The scope of the recipient.</span></span> <span data-ttu-id="8e28d-142">可能な値は、`none`、`internal`、`external`、`externalPartner`、`externalNonParther` です。</span><span class="sxs-lookup"><span data-stu-id="8e28d-142">Possible values are: `none`, `internal`, `external`, `externalPartner`, `externalNonParther`.</span></span> <span data-ttu-id="8e28d-143">たとえば、管理者は、その「パートナー」になるように別の組織を設定できます。</span><span class="sxs-lookup"><span data-stu-id="8e28d-143">For example, an administrator can set another organization to be its "partner".</span></span> <span data-ttu-id="8e28d-144">スコープは、管理者が特定のスコープにアクセスできるようにする特定のメール ヒントを希望する場合に便利です。</span><span class="sxs-lookup"><span data-stu-id="8e28d-144">The scope is useful if an administrator wants certain mailtips to be accessible to certain scopes.</span></span> <span data-ttu-id="8e28d-145">送信者のメッセージが言葉使い、トーン、およびコンテンツに関する正しい判断を下すことを支援、組織になることを通知するに有用なもあります。</span><span class="sxs-lookup"><span data-stu-id="8e28d-145">It's also useful to senders to inform them that their message may leave the organization, helping them make the correct decisions about wording, tone and content.</span></span>|
| <span data-ttu-id="8e28d-146">recipientSuggestions</span><span class="sxs-lookup"><span data-stu-id="8e28d-146">recipientSuggestions</span></span> | <span data-ttu-id="8e28d-147">[recipient](../resources/recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="8e28d-147">[recipient](../resources/recipient.md) collection</span></span> | <span data-ttu-id="8e28d-148">同じメッセージに表示される前のコンテキストに基づいて提案される受信者。</span><span class="sxs-lookup"><span data-stu-id="8e28d-148">Recipients suggested based on previous contexts where they appear in the same message.</span></span> |
| <span data-ttu-id="8e28d-149">totalMemberCount</span><span class="sxs-lookup"><span data-stu-id="8e28d-149">totalMemberCount</span></span> | <span data-ttu-id="8e28d-150">Int32</span><span class="sxs-lookup"><span data-stu-id="8e28d-150">Int32</span></span> | <span data-ttu-id="8e28d-151">受信者が配布リストの場合はメンバー数です。</span><span class="sxs-lookup"><span data-stu-id="8e28d-151">The number of members if the recipient is a distribution list.</span></span> |

### <a name="recipientscopetype-values"></a><span data-ttu-id="8e28d-152">recipientScopeType 値</span><span class="sxs-lookup"><span data-stu-id="8e28d-152">recipientScopeType values</span></span>

| <span data-ttu-id="8e28d-153">値</span><span class="sxs-lookup"><span data-stu-id="8e28d-153">Value</span></span>
|:-------------------------
| <span data-ttu-id="8e28d-154">none</span><span class="sxs-lookup"><span data-stu-id="8e28d-154">none</span></span>
| <span data-ttu-id="8e28d-155">内部</span><span class="sxs-lookup"><span data-stu-id="8e28d-155">internal</span></span>
| <span data-ttu-id="8e28d-156">外部</span><span class="sxs-lookup"><span data-stu-id="8e28d-156">external</span></span>
| <span data-ttu-id="8e28d-157">externalPartner</span><span class="sxs-lookup"><span data-stu-id="8e28d-157">externalPartner</span></span>
| <span data-ttu-id="8e28d-158">externalNonPartner</span><span class="sxs-lookup"><span data-stu-id="8e28d-158">externalNonPartner</span></span>


## <a name="json-representation"></a><span data-ttu-id="8e28d-159">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8e28d-159">JSON representation</span></span>

<span data-ttu-id="8e28d-160">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="8e28d-160">Here is a JSON representation of the resource.</span></span>

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
