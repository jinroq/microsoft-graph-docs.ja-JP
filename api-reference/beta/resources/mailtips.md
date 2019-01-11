---
title: リソースの種類のメール ヒント
description: 'メッセージの作成中にユーザーに表示される、受信者に関する情報メッセージです。 たとえば、不在時のメッセージ '
localization_priority: Normal
ms.openlocfilehash: 62955594412b2d42a4d05b4b13858c4e511605df
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860642"
---
# <a name="mailtips-resource-type"></a><span data-ttu-id="ccbc6-104">リソースの種類のメール ヒント</span><span class="sxs-lookup"><span data-stu-id="ccbc6-104">mailTips resource type</span></span>

> <span data-ttu-id="ccbc6-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ccbc6-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ccbc6-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ccbc6-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ccbc6-107">メッセージの作成中にユーザーに表示される、受信者に関する情報メッセージです。</span><span class="sxs-lookup"><span data-stu-id="ccbc6-107">Informative messages about a recipient, that are displayed to users while they are composing a message.</span></span> <span data-ttu-id="ccbc6-108">など、不在時のメッセージ、自動返信メッセージの受信者として。</span><span class="sxs-lookup"><span data-stu-id="ccbc6-108">For example, an out-of-office message as an automatic reply for a message recipient.</span></span>


## <a name="properties"></a><span data-ttu-id="ccbc6-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ccbc6-109">Properties</span></span>
| <span data-ttu-id="ccbc6-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ccbc6-110">Property</span></span>     | <span data-ttu-id="ccbc6-111">種類</span><span class="sxs-lookup"><span data-stu-id="ccbc6-111">Type</span></span>   |<span data-ttu-id="ccbc6-112">説明</span><span class="sxs-lookup"><span data-stu-id="ccbc6-112">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ccbc6-113">automaticReplies</span><span class="sxs-lookup"><span data-stu-id="ccbc6-113">automaticReplies</span></span> | [<span data-ttu-id="ccbc6-114">automaticRepliesMailTips</span><span class="sxs-lookup"><span data-stu-id="ccbc6-114">automaticRepliesMailTips</span></span>](../resources/automaticrepliesmailtips.md) | <span data-ttu-id="ccbc6-115">受信者によって設定されている場合の自動応答に関するメールのヒント。</span><span class="sxs-lookup"><span data-stu-id="ccbc6-115">Mail tips for automatic reply if it has been set up by the recipient.</span></span> |
| <span data-ttu-id="ccbc6-116">customMailTip</span><span class="sxs-lookup"><span data-stu-id="ccbc6-116">customMailTip</span></span> | <span data-ttu-id="ccbc6-117">String</span><span class="sxs-lookup"><span data-stu-id="ccbc6-117">String</span></span> | <span data-ttu-id="ccbc6-118">受信者のメールボックスに設定可能なカスタム メールのヒント。</span><span class="sxs-lookup"><span data-stu-id="ccbc6-118">A custom mail tip that can be set on the recipient's mailbox.</span></span> |
| <span data-ttu-id="ccbc6-119">deliveryRestricted</span><span class="sxs-lookup"><span data-stu-id="ccbc6-119">deliveryRestricted</span></span>| <span data-ttu-id="ccbc6-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="ccbc6-120">Boolean</span></span> | <span data-ttu-id="ccbc6-121">受信者のメールボックスが制限されているかどうか。たとえば、送信者の定義済みリストからのメッセージのみを受け付ける、送信者の定義済みリストからのメッセージを拒否する、または認証された送信者からのメッセージのみを受信するなどです。</span><span class="sxs-lookup"><span data-stu-id="ccbc6-121">Whether the recipient's mailbox is restricted, for example, accepting messages from only a predefined list of senders, rejecting messages from a predefined list of senders, or accepting messages from only authenticated senders.</span></span> |
| <span data-ttu-id="ccbc6-122">emailAddress</span><span class="sxs-lookup"><span data-stu-id="ccbc6-122">emailAddress</span></span> | [<span data-ttu-id="ccbc6-123">emailAddress</span><span class="sxs-lookup"><span data-stu-id="ccbc6-123">emailAddress</span></span>](../resources/emailaddress.md) | <span data-ttu-id="ccbc6-124">メールヒントを取得する受信者の電子メール アドレス。</span><span class="sxs-lookup"><span data-stu-id="ccbc6-124">The email address of the recipient to get mailtips for.</span></span> |
| <span data-ttu-id="ccbc6-125">エラー</span><span class="sxs-lookup"><span data-stu-id="ccbc6-125">error</span></span> | [<span data-ttu-id="ccbc6-126">mailTipsError</span><span class="sxs-lookup"><span data-stu-id="ccbc6-126">mailTipsError</span></span>](../resources/mailtipserror.md) | <span data-ttu-id="ccbc6-127">[GetMailTips](../api/user-getmailtips.md)操作中に発生するエラーです。</span><span class="sxs-lookup"><span data-stu-id="ccbc6-127">Errors that occur during the [getMailTips](../api/user-getmailtips.md) action.</span></span> |
| <span data-ttu-id="ccbc6-128">externalMemberCount</span><span class="sxs-lookup"><span data-stu-id="ccbc6-128">externalMemberCount</span></span> | <span data-ttu-id="ccbc6-129">Int32</span><span class="sxs-lookup"><span data-stu-id="ccbc6-129">Int32</span></span> | <span data-ttu-id="ccbc6-130">受信者が配布リストの場合は外部メンバーの数です。</span><span class="sxs-lookup"><span data-stu-id="ccbc6-130">The number of external members if the recipient is a distribution list.</span></span> |
| <span data-ttu-id="ccbc6-131">isModerated</span><span class="sxs-lookup"><span data-stu-id="ccbc6-131">isModerated</span></span> |<span data-ttu-id="ccbc6-132">Boolean</span><span class="sxs-lookup"><span data-stu-id="ccbc6-132">Boolean</span></span>  | <span data-ttu-id="ccbc6-p104">受信者へのメッセージ送信に承認が必要かどうか。たとえば、受信者が大規模な配布リストであり、モデレーターが配布リストに送信されたメッセージを承認するようにセットアップされている場合、または受信者へのメッセージの送信に受信者の上司の承認を必要とする場合などです。</span><span class="sxs-lookup"><span data-stu-id="ccbc6-p104">Whether sending messages to the recipient requires approval. For example, if the recipient is a large distribution list and a moderator has been set up to approve messages sent to that distribution list, or if sending messages to a recipient requires approval of the recipient's manager.</span></span> |
| <span data-ttu-id="ccbc6-135">mailboxFull</span><span class="sxs-lookup"><span data-stu-id="ccbc6-135">mailboxFull</span></span> | <span data-ttu-id="ccbc6-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="ccbc6-136">Boolean</span></span> | <span data-ttu-id="ccbc6-137">受信者のメールボックスのフル状態。</span><span class="sxs-lookup"><span data-stu-id="ccbc6-137">The mailbox full status of the recipient.</span></span> |
| <span data-ttu-id="ccbc6-138">maxMessageSize</span><span class="sxs-lookup"><span data-stu-id="ccbc6-138">maxMessageSize</span></span> | <span data-ttu-id="ccbc6-139">Int32</span><span class="sxs-lookup"><span data-stu-id="ccbc6-139">Int32</span></span> | <span data-ttu-id="ccbc6-140">受信者の組織またはメールボックスに対して構成されているメッセージの最大サイズ。</span><span class="sxs-lookup"><span data-stu-id="ccbc6-140">The maximum message size that has been configured for the recipient's organization or mailbox.</span></span> |
| <span data-ttu-id="ccbc6-141">recipientScope</span><span class="sxs-lookup"><span data-stu-id="ccbc6-141">recipientScope</span></span> | <span data-ttu-id="ccbc6-142">String</span><span class="sxs-lookup"><span data-stu-id="ccbc6-142">String</span></span> | <span data-ttu-id="ccbc6-143">受信者のスコープ。</span><span class="sxs-lookup"><span data-stu-id="ccbc6-143">The scope of the recipient.</span></span> <span data-ttu-id="ccbc6-144">可能な値は、`none`、`internal`、`external`、`externalPartner`、`externalNonParther` です。</span><span class="sxs-lookup"><span data-stu-id="ccbc6-144">Possible values are: `none`, `internal`, `external`, `externalPartner`, `externalNonParther`.</span></span> <span data-ttu-id="ccbc6-145">たとえば、管理者は、その「パートナー」になるように別の組織を設定できます。</span><span class="sxs-lookup"><span data-stu-id="ccbc6-145">For example, an administrator can set another organization to be its "partner".</span></span> <span data-ttu-id="ccbc6-146">スコープは、管理者が特定のスコープにアクセスできるようにする特定のメール ヒントを希望する場合に便利です。</span><span class="sxs-lookup"><span data-stu-id="ccbc6-146">The scope is useful if an administrator wants certain mailtips to be accessible to certain scopes.</span></span> <span data-ttu-id="ccbc6-147">送信者のメッセージが言葉使い、トーン、およびコンテンツに関する正しい判断を下すことを支援、組織になることを通知するに有用なもあります。</span><span class="sxs-lookup"><span data-stu-id="ccbc6-147">It's also useful to senders to inform them that their message may leave the organization, helping them make the correct decisions about wording, tone and content.</span></span>|
| <span data-ttu-id="ccbc6-148">recipientSuggestions</span><span class="sxs-lookup"><span data-stu-id="ccbc6-148">recipientSuggestions</span></span> | <span data-ttu-id="ccbc6-149">[recipient](../resources/recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="ccbc6-149">[recipient](../resources/recipient.md) collection</span></span> | <span data-ttu-id="ccbc6-150">同じメッセージに表示される前のコンテキストに基づいて提案される受信者。</span><span class="sxs-lookup"><span data-stu-id="ccbc6-150">Recipients suggested based on previous contexts where they appear in the same message.</span></span> |
| <span data-ttu-id="ccbc6-151">totalMemberCount</span><span class="sxs-lookup"><span data-stu-id="ccbc6-151">totalMemberCount</span></span> | <span data-ttu-id="ccbc6-152">Int32</span><span class="sxs-lookup"><span data-stu-id="ccbc6-152">Int32</span></span> | <span data-ttu-id="ccbc6-153">受信者が配布リストの場合はメンバー数です。</span><span class="sxs-lookup"><span data-stu-id="ccbc6-153">The number of members if the recipient is a distribution list.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ccbc6-154">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ccbc6-154">JSON representation</span></span>

<span data-ttu-id="ccbc6-155">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ccbc6-155">Here is a JSON representation of the resource.</span></span>

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
