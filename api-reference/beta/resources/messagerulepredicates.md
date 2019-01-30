---
title: messageRulePredicates リソースの種類
description: ルールで使用可能な条件および例外のセットを表します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: fda6a160d30dc0d822f2e0aeb5642250d6b69658
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2019
ms.locfileid: "29644036"
---
# <a name="messagerulepredicates-resource-type"></a><span data-ttu-id="5f3ba-103">messageRulePredicates リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5f3ba-103">messageRulePredicates resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5f3ba-104">ルールで使用可能な条件および例外のセットを表します。</span><span class="sxs-lookup"><span data-stu-id="5f3ba-104">Represents the set of conditions and exceptions that are available for a rule.</span></span>

## <a name="properties"></a><span data-ttu-id="5f3ba-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5f3ba-105">Properties</span></span>
| <span data-ttu-id="5f3ba-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5f3ba-106">Property</span></span>     | <span data-ttu-id="5f3ba-107">型</span><span class="sxs-lookup"><span data-stu-id="5f3ba-107">Type</span></span>   |<span data-ttu-id="5f3ba-108">説明</span><span class="sxs-lookup"><span data-stu-id="5f3ba-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="5f3ba-109">bodyContains</span><span class="sxs-lookup"><span data-stu-id="5f3ba-109">bodyContains</span></span> | <span data-ttu-id="5f3ba-110">コレクション (String)</span><span class="sxs-lookup"><span data-stu-id="5f3ba-110">Collection (String)</span></span> | <span data-ttu-id="5f3ba-111">条件または例外を適用するために、受信メッセージの本文に表示される文字列を表します。</span><span class="sxs-lookup"><span data-stu-id="5f3ba-111">Represents the strings that should appear in the body of an incoming message in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="5f3ba-112">bodyOrSubjectContains</span><span class="sxs-lookup"><span data-stu-id="5f3ba-112">bodyOrSubjectContains</span></span> | <span data-ttu-id="5f3ba-113">コレクション (String)</span><span class="sxs-lookup"><span data-stu-id="5f3ba-113">Collection (String)</span></span> | <span data-ttu-id="5f3ba-114">条件または例外を適用するために、受信メッセージの本文または件名に表示される文字列を表します。</span><span class="sxs-lookup"><span data-stu-id="5f3ba-114">Represents the strings that should appear in the body or subject of an incoming message in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="5f3ba-115">categories</span><span class="sxs-lookup"><span data-stu-id="5f3ba-115">categories</span></span> | <span data-ttu-id="5f3ba-116">コレクション (String)</span><span class="sxs-lookup"><span data-stu-id="5f3ba-116">Collection (String)</span></span> | <span data-ttu-id="5f3ba-117">条件または例外を適用するために、受信メッセージにラベルを付けるカテゴリを表します。</span><span class="sxs-lookup"><span data-stu-id="5f3ba-117">Represents the categories that an incoming message should be labeled with in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="5f3ba-118">fromAddresses</span><span class="sxs-lookup"><span data-stu-id="5f3ba-118">fromAddresses</span></span> | <span data-ttu-id="5f3ba-119">コレクション ([Recipient](recipient.md))</span><span class="sxs-lookup"><span data-stu-id="5f3ba-119">Collection ([recipient](recipient.md))</span></span> | <span data-ttu-id="5f3ba-120">条件または例外を適用するために、受信メッセージの特定の送信者のメール アドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="5f3ba-120">Represents the specific sender email addresses of an incoming message in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="5f3ba-121">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="5f3ba-121">hasAttachments</span></span> | <span data-ttu-id="5f3ba-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f3ba-122">Boolean</span></span> | <span data-ttu-id="5f3ba-123">条件または例外を適用するために、受信メッセージに添付ファイルがあるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="5f3ba-123">Indicates whether an incoming message must have attachments in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="5f3ba-124">headerContains</span><span class="sxs-lookup"><span data-stu-id="5f3ba-124">headerContains</span></span> | <span data-ttu-id="5f3ba-125">コレクション (String)</span><span class="sxs-lookup"><span data-stu-id="5f3ba-125">Collection (String)</span></span> | <span data-ttu-id="5f3ba-126">条件または例外を適用するために、受信メッセージのヘッダーに表示される文字列を表します。</span><span class="sxs-lookup"><span data-stu-id="5f3ba-126">Represents the strings that appear in the headers of an incoming message in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="5f3ba-127">importance</span><span class="sxs-lookup"><span data-stu-id="5f3ba-127">importance</span></span> | <span data-ttu-id="5f3ba-128">String</span><span class="sxs-lookup"><span data-stu-id="5f3ba-128">String</span></span> | <span data-ttu-id="5f3ba-129">条件または例外を適用するために、受信メッセージに記録される重要性: `low`、`normal`、`high`。</span><span class="sxs-lookup"><span data-stu-id="5f3ba-129">The importance that is stamped on an incoming message in order for the condition or exception to apply: `low`, `normal`, `high`.</span></span> |
| <span data-ttu-id="5f3ba-130">isApprovalRequest</span><span class="sxs-lookup"><span data-stu-id="5f3ba-130">isApprovalRequest</span></span> | <span data-ttu-id="5f3ba-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f3ba-131">Boolean</span></span> | <span data-ttu-id="5f3ba-132">条件または例外を適用するために、受信メッセージが承認要求であるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="5f3ba-132">Indicates whether an incoming message must be an approval request in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="5f3ba-133">isAutomaticForward</span><span class="sxs-lookup"><span data-stu-id="5f3ba-133">isAutomaticForward</span></span> | <span data-ttu-id="5f3ba-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f3ba-134">Boolean</span></span> | <span data-ttu-id="5f3ba-135">条件または例外を適用するために、受信メッセージが自動的に転送されるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="5f3ba-135">Indicates whether an incoming message must be automatically forwarded in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="5f3ba-136">isAutomaticReply</span><span class="sxs-lookup"><span data-stu-id="5f3ba-136">isAutomaticReply</span></span> | <span data-ttu-id="5f3ba-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f3ba-137">Boolean</span></span> | <span data-ttu-id="5f3ba-138">条件または例外を適用するために、受信メッセージが自動返信であるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="5f3ba-138">Indicates whether an incoming message must be an auto reply in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="5f3ba-139">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="5f3ba-139">isEncrypted</span></span> | <span data-ttu-id="5f3ba-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f3ba-140">Boolean</span></span> | <span data-ttu-id="5f3ba-141">条件または例外を適用するために、受信メッセージが暗号化されるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="5f3ba-141">Indicates whether an incoming message must be encrypted in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="5f3ba-142">isMeetingRequest</span><span class="sxs-lookup"><span data-stu-id="5f3ba-142">isMeetingRequest</span></span> | <span data-ttu-id="5f3ba-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f3ba-143">Boolean</span></span> | <span data-ttu-id="5f3ba-144">条件または例外を適用するために、受信メッセージが会議出席依頼であるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="5f3ba-144">Indicates whether an incoming message must be a meeting request in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="5f3ba-145">isMeetingResponse</span><span class="sxs-lookup"><span data-stu-id="5f3ba-145">isMeetingResponse</span></span> | <span data-ttu-id="5f3ba-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f3ba-146">Boolean</span></span> | <span data-ttu-id="5f3ba-147">条件または例外を適用するために、受信メッセージが会議出席依頼の返信であるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="5f3ba-147">Indicates whether an incoming message must be a meeting response in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="5f3ba-148">isNonDeliveryReport</span><span class="sxs-lookup"><span data-stu-id="5f3ba-148">isNonDeliveryReport</span></span> | <span data-ttu-id="5f3ba-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f3ba-149">Boolean</span></span> | <span data-ttu-id="5f3ba-150">条件または例外を適用するために、受信メッセージが配信不能レポートであるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="5f3ba-150">Indicates whether an incoming message must be a non-delivery report in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="5f3ba-151">IsPermissionControlled</span><span class="sxs-lookup"><span data-stu-id="5f3ba-151">isPermissionControlled</span></span> | <span data-ttu-id="5f3ba-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f3ba-152">Boolean</span></span> | <span data-ttu-id="5f3ba-153">条件または例外を適用するために、受信メッセージがアクセス許可制御 (RMS 保護) されるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="5f3ba-153">Indicates whether an incoming message must be permission controlled (RMS-protected) in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="5f3ba-154">isReadReceipt</span><span class="sxs-lookup"><span data-stu-id="5f3ba-154">isReadReceipt</span></span> | <span data-ttu-id="5f3ba-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f3ba-155">Boolean</span></span> | <span data-ttu-id="5f3ba-156">条件または例外を適用するために、受信メッセージが開封確認メッセージであるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="5f3ba-156">Indicates whether an incoming message must be a read receipt in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="5f3ba-157">isSigned</span><span class="sxs-lookup"><span data-stu-id="5f3ba-157">isSigned</span></span> | <span data-ttu-id="5f3ba-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f3ba-158">Boolean</span></span> | <span data-ttu-id="5f3ba-159">条件または例外を適用するために、受信メッセージが S/MIME 署名されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="5f3ba-159">Indicates whether an incoming message must be S/MIME-signed in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="5f3ba-160">isVoicemail</span><span class="sxs-lookup"><span data-stu-id="5f3ba-160">isVoicemail</span></span> | <span data-ttu-id="5f3ba-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f3ba-161">Boolean</span></span> | <span data-ttu-id="5f3ba-162">条件または例外を適用するために、受信メッセージがボイス メールかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="5f3ba-162">Indicates whether an incoming message must be a voice mail in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="5f3ba-163">messageActionFlag</span><span class="sxs-lookup"><span data-stu-id="5f3ba-163">messageActionFlag</span></span> | <span data-ttu-id="5f3ba-164">String</span><span class="sxs-lookup"><span data-stu-id="5f3ba-164">String</span></span>  | <span data-ttu-id="5f3ba-165">条件または例外を適用するために、受信メッセージに表示されるアクション フラグの値を表します。</span><span class="sxs-lookup"><span data-stu-id="5f3ba-165">Represents the flag-for-action value that appears on an incoming message in order for the condition or exception to apply.</span></span> <span data-ttu-id="5f3ba-166">使用可能な値は、`any`、`call`、`doNotForward`、`followUp`、`fyi`、`forward`、`noResponseNecessary`、`read`、`reply`、`replyToAll`、`review` です。</span><span class="sxs-lookup"><span data-stu-id="5f3ba-166">Possible values are: `any`, `call`, `doNotForward`, `followUp`, `fyi`, `forward`, `noResponseNecessary`, `read`, `reply`, `replyToAll`, `review`.</span></span> |
| <span data-ttu-id="5f3ba-167">notSentToMe</span><span class="sxs-lookup"><span data-stu-id="5f3ba-167">notSentToMe</span></span> | <span data-ttu-id="5f3ba-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f3ba-168">Boolean</span></span> | <span data-ttu-id="5f3ba-169">条件または例外を適用するために、メールボックスの所有者が受信メッセージの受信者でないことを示します。</span><span class="sxs-lookup"><span data-stu-id="5f3ba-169">Indicates whether the owner of the mailbox must not be a recipient of an incoming message in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="5f3ba-170">recipientContains</span><span class="sxs-lookup"><span data-stu-id="5f3ba-170">recipientContains</span></span> | <span data-ttu-id="5f3ba-171">コレクション (String)</span><span class="sxs-lookup"><span data-stu-id="5f3ba-171">Collection (String)</span></span> | <span data-ttu-id="5f3ba-172">条件または例外を適用するために、受信メッセージの **ToRecipients** または **CcRecipients** プロパティに表示される文字列を表します。</span><span class="sxs-lookup"><span data-stu-id="5f3ba-172">Represents the strings that appear in either the **toRecipients** or **ccRecipients** properties of an incoming message in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="5f3ba-173">senderContains</span><span class="sxs-lookup"><span data-stu-id="5f3ba-173">senderContains</span></span> | <span data-ttu-id="5f3ba-174">コレクション (String)</span><span class="sxs-lookup"><span data-stu-id="5f3ba-174">Collection (String)</span></span> | <span data-ttu-id="5f3ba-175">条件または例外を適用するために、受信メッセージの **From** プロパティに表示される文字列を表します。</span><span class="sxs-lookup"><span data-stu-id="5f3ba-175">Represents the strings that appear in the **from** property of an incoming message in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="5f3ba-176">sensitivity</span><span class="sxs-lookup"><span data-stu-id="5f3ba-176">sensitivity</span></span> | <span data-ttu-id="5f3ba-177">String</span><span class="sxs-lookup"><span data-stu-id="5f3ba-177">String</span></span> | <span data-ttu-id="5f3ba-p102">条件または例外を適用するために、受信メッセージに記録される秘密度レベルを表します。使用可能な値: `normal`、`personal`、`private`、`confidential`。</span><span class="sxs-lookup"><span data-stu-id="5f3ba-p102">Represents the sensitivity level that must be stamped on an incoming message in order for the condition or exception to apply. Possible values are: `normal`, `personal`, `private`, `confidential`.</span></span> |
| <span data-ttu-id="5f3ba-180">sentCcMe</span><span class="sxs-lookup"><span data-stu-id="5f3ba-180">sentCcMe</span></span> | <span data-ttu-id="5f3ba-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f3ba-181">Boolean</span></span> | <span data-ttu-id="5f3ba-182">条件または例外を適用するために、メールボックスの所有者が受信メッセージの **ccRecipients** プロパティにあるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="5f3ba-182">Indicates whether the owner of the mailbox must be in the **ccRecipients** property of an incoming message in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="5f3ba-183">sentOnlyToMe</span><span class="sxs-lookup"><span data-stu-id="5f3ba-183">sentOnlyToMe</span></span> | <span data-ttu-id="5f3ba-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f3ba-184">Boolean</span></span> | <span data-ttu-id="5f3ba-185">条件または例外を適用するために、メールボックスの所有者が受信メッセージの唯一の受信者かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="5f3ba-185">Indicates whether the owner of the mailbox must be the only recipient in an incoming message in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="5f3ba-186">sentToAddresses</span><span class="sxs-lookup"><span data-stu-id="5f3ba-186">sentToAddresses</span></span> | <span data-ttu-id="5f3ba-187">コレクション ([Recipient](recipient.md))</span><span class="sxs-lookup"><span data-stu-id="5f3ba-187">Collection ([recipient](recipient.md))</span></span> | <span data-ttu-id="5f3ba-188">条件または例外を適用するために、受信メッセージが送信されたメール アドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="5f3ba-188">Represents the email addresses that an incoming message must have been sent to in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="5f3ba-189">sentToMe</span><span class="sxs-lookup"><span data-stu-id="5f3ba-189">sentToMe</span></span> | <span data-ttu-id="5f3ba-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f3ba-190">Boolean</span></span> | <span data-ttu-id="5f3ba-191">条件または例外を適用するために、メールボックスの所有者が受信メッセージの **ToRecipients** プロパティにあるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="5f3ba-191">Indicates whether the owner of the mailbox must be in the **toRecipients** property of an incoming message in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="5f3ba-192">sentToOrCcMe</span><span class="sxs-lookup"><span data-stu-id="5f3ba-192">sentToOrCcMe</span></span> | <span data-ttu-id="5f3ba-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f3ba-193">Boolean</span></span> | <span data-ttu-id="5f3ba-194">条件または例外を適用するために、メールボックスの所有者が受信メッセージの **toRecipients** または **ccRecipients** プロパティにあるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="5f3ba-194">Indicates whether the owner of the mailbox must be in either a **toRecipients** or **ccRecipients** property of an incoming message in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="5f3ba-195">subjectContains</span><span class="sxs-lookup"><span data-stu-id="5f3ba-195">subjectContains</span></span> | <span data-ttu-id="5f3ba-196">コレクション (String)</span><span class="sxs-lookup"><span data-stu-id="5f3ba-196">Collection (String)</span></span> | <span data-ttu-id="5f3ba-197">条件または例外を適用するために、受信メッセージの件名に表示される文字列を表します。</span><span class="sxs-lookup"><span data-stu-id="5f3ba-197">Represents the strings that appear in the subject of an incoming message in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="5f3ba-198">withinSizeRange</span><span class="sxs-lookup"><span data-stu-id="5f3ba-198">withinSizeRange</span></span> | [<span data-ttu-id="5f3ba-199">sizeRange</span><span class="sxs-lookup"><span data-stu-id="5f3ba-199">sizeRange</span></span>](sizerange.md) | <span data-ttu-id="5f3ba-200">条件または例外を適用するために、受信メッセージに想定される最小サイズと最大サイズ (単位: キロバイト) を表します。</span><span class="sxs-lookup"><span data-stu-id="5f3ba-200">Represents the minimum and maximum sizes (in kilobytes) that an incoming message must fall in between in order for the condition or exception to apply.</span></span> |



## <a name="json-representation"></a><span data-ttu-id="5f3ba-201">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5f3ba-201">JSON representation</span></span>
<span data-ttu-id="5f3ba-202">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="5f3ba-202">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
   ],
  "@odata.type": "microsoft.graph.messageRulePredicates"
}-->

```json
{
  "bodyContains": ["String"],
  "bodyOrSubjectContains": ["String"],
  "categories": ["String"],
  "fromAddresses": [{"@odata.type": "microsoft.graph.recipient"}],
  "hasAttachments": "Boolean",
  "headerContains": ["String"],
  "importance": "String",
  "isApprovalRequest": "Boolean",
  "isAutomaticForward": "Boolean",
  "isAutomaticReply": "Boolean",
  "isEncrypted": "Boolean",
  "isMeetingRequest": "Boolean",
  "isMeetingResponse": "Boolean",
  "isNonDeliveryReport": "Boolean",
  "isPermissionControlled": "Boolean",
  "isReadReceipt": "Boolean",
  "isSigned": "Boolean",
  "isVoicemail": "Boolean",
  "messageActionFlag": "String",
  "notSentToMe": "Boolean",
  "recipientContains": ["String"],
  "senderContains": ["String"],
  "sensitivity": "String",
  "sentCcMe": "Boolean",
  "sentOnlyToMe": "Boolean",
  "sentToAddresses": [{"@odata.type": "microsoft.graph.recipient"}],
  "sentToMe": "Boolean",
  "sentToOrCcMe": "Boolean",
  "subjectContains": ["String"],
  "withinSizeRange": {"@odata.type": "microsoft.graph.sizeRange"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "messageRulePredicates resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/messagerulepredicates.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
