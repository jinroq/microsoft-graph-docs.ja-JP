---
title: messageRulePredicates リソースの種類
description: ルールで使用可能な条件および例外のセットを表します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: e36cabc34e1374d666e8a9c34d72dd570a0eb2f9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966728"
---
# <a name="messagerulepredicates-resource-type"></a><span data-ttu-id="1c39d-103">messageRulePredicates リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1c39d-103">messageRulePredicates resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1c39d-104">ルールで使用可能な条件および例外のセットを表します。</span><span class="sxs-lookup"><span data-stu-id="1c39d-104">Represents the set of conditions and exceptions that are available for a rule.</span></span>

## <a name="properties"></a><span data-ttu-id="1c39d-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1c39d-105">Properties</span></span>
| <span data-ttu-id="1c39d-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1c39d-106">Property</span></span>     | <span data-ttu-id="1c39d-107">型</span><span class="sxs-lookup"><span data-stu-id="1c39d-107">Type</span></span>   |<span data-ttu-id="1c39d-108">説明</span><span class="sxs-lookup"><span data-stu-id="1c39d-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1c39d-109">bodyContains</span><span class="sxs-lookup"><span data-stu-id="1c39d-109">bodyContains</span></span> | <span data-ttu-id="1c39d-110">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="1c39d-110">String collection</span></span> | <span data-ttu-id="1c39d-111">条件または例外を適用するために、受信メッセージの本文に表示される文字列を表します。</span><span class="sxs-lookup"><span data-stu-id="1c39d-111">Represents the strings that should appear in the body of an incoming message in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="1c39d-112">bodyOrSubjectContains</span><span class="sxs-lookup"><span data-stu-id="1c39d-112">bodyOrSubjectContains</span></span> | <span data-ttu-id="1c39d-113">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="1c39d-113">String collection</span></span> | <span data-ttu-id="1c39d-114">条件または例外を適用するために、受信メッセージの本文または件名に表示される文字列を表します。</span><span class="sxs-lookup"><span data-stu-id="1c39d-114">Represents the strings that should appear in the body or subject of an incoming message in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="1c39d-115">categories</span><span class="sxs-lookup"><span data-stu-id="1c39d-115">categories</span></span> | <span data-ttu-id="1c39d-116">String collection</span><span class="sxs-lookup"><span data-stu-id="1c39d-116">String collection</span></span> | <span data-ttu-id="1c39d-117">条件または例外を適用するために、受信メッセージにラベルを付けるカテゴリを表します。</span><span class="sxs-lookup"><span data-stu-id="1c39d-117">Represents the categories that an incoming message should be labeled with in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="1c39d-118">fromAddresses</span><span class="sxs-lookup"><span data-stu-id="1c39d-118">fromAddresses</span></span> | <span data-ttu-id="1c39d-119">[recipient](recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="1c39d-119">[recipient](recipient.md) collection</span></span> | <span data-ttu-id="1c39d-120">条件または例外を適用するために、受信メッセージの特定の送信者のメール アドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="1c39d-120">Represents the specific sender email addresses of an incoming message in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="1c39d-121">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="1c39d-121">hasAttachments</span></span> | <span data-ttu-id="1c39d-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="1c39d-122">Boolean</span></span> | <span data-ttu-id="1c39d-123">条件または例外を適用するために、受信メッセージに添付ファイルがあるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1c39d-123">Indicates whether an incoming message must have attachments in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="1c39d-124">headerContains</span><span class="sxs-lookup"><span data-stu-id="1c39d-124">headerContains</span></span> | <span data-ttu-id="1c39d-125">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="1c39d-125">String collection</span></span> | <span data-ttu-id="1c39d-126">条件または例外を適用するために、受信メッセージのヘッダーに表示される文字列を表します。</span><span class="sxs-lookup"><span data-stu-id="1c39d-126">Represents the strings that appear in the headers of an incoming message in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="1c39d-127">importance</span><span class="sxs-lookup"><span data-stu-id="1c39d-127">importance</span></span> | <span data-ttu-id="1c39d-128">importance</span><span class="sxs-lookup"><span data-stu-id="1c39d-128">importance</span></span> | <span data-ttu-id="1c39d-129">条件または例外を適用するために、受信メッセージに記録される重要性: `low`、`normal`、`high`。</span><span class="sxs-lookup"><span data-stu-id="1c39d-129">The importance that is stamped on an incoming message in order for the condition or exception to apply: `low`, `normal`, `high`.</span></span> |
| <span data-ttu-id="1c39d-130">isApprovalRequest</span><span class="sxs-lookup"><span data-stu-id="1c39d-130">isApprovalRequest</span></span> | <span data-ttu-id="1c39d-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="1c39d-131">Boolean</span></span> | <span data-ttu-id="1c39d-132">条件または例外を適用するために、受信メッセージが承認要求であるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1c39d-132">Indicates whether an incoming message must be an approval request in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="1c39d-133">isAutomaticForward</span><span class="sxs-lookup"><span data-stu-id="1c39d-133">isAutomaticForward</span></span> | <span data-ttu-id="1c39d-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="1c39d-134">Boolean</span></span> | <span data-ttu-id="1c39d-135">条件または例外を適用するために、受信メッセージが自動的に転送されるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1c39d-135">Indicates whether an incoming message must be automatically forwarded in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="1c39d-136">isAutomaticReply</span><span class="sxs-lookup"><span data-stu-id="1c39d-136">isAutomaticReply</span></span> | <span data-ttu-id="1c39d-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="1c39d-137">Boolean</span></span> | <span data-ttu-id="1c39d-138">条件または例外を適用するために、受信メッセージが自動返信であるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1c39d-138">Indicates whether an incoming message must be an auto reply in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="1c39d-139">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="1c39d-139">isEncrypted</span></span> | <span data-ttu-id="1c39d-140">ブール型</span><span class="sxs-lookup"><span data-stu-id="1c39d-140">Boolean</span></span> | <span data-ttu-id="1c39d-141">条件または例外を適用するために、受信メッセージが暗号化されるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1c39d-141">Indicates whether an incoming message must be encrypted in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="1c39d-142">isMeetingRequest</span><span class="sxs-lookup"><span data-stu-id="1c39d-142">isMeetingRequest</span></span> | <span data-ttu-id="1c39d-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="1c39d-143">Boolean</span></span> | <span data-ttu-id="1c39d-144">条件または例外を適用するために、受信メッセージが会議出席依頼であるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1c39d-144">Indicates whether an incoming message must be a meeting request in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="1c39d-145">isMeetingResponse</span><span class="sxs-lookup"><span data-stu-id="1c39d-145">isMeetingResponse</span></span> | <span data-ttu-id="1c39d-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="1c39d-146">Boolean</span></span> | <span data-ttu-id="1c39d-147">条件または例外を適用するために、受信メッセージが会議出席依頼の返信であるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1c39d-147">Indicates whether an incoming message must be a meeting response in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="1c39d-148">isNonDeliveryReport</span><span class="sxs-lookup"><span data-stu-id="1c39d-148">isNonDeliveryReport</span></span> | <span data-ttu-id="1c39d-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="1c39d-149">Boolean</span></span> | <span data-ttu-id="1c39d-150">条件または例外を適用するために、受信メッセージが配信不能レポートであるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1c39d-150">Indicates whether an incoming message must be a non-delivery report in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="1c39d-151">IsPermissionControlled</span><span class="sxs-lookup"><span data-stu-id="1c39d-151">isPermissionControlled</span></span> | <span data-ttu-id="1c39d-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="1c39d-152">Boolean</span></span> | <span data-ttu-id="1c39d-153">条件または例外を適用するために、受信メッセージがアクセス許可制御 (RMS 保護) されるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1c39d-153">Indicates whether an incoming message must be permission controlled (RMS-protected) in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="1c39d-154">isReadReceipt</span><span class="sxs-lookup"><span data-stu-id="1c39d-154">isReadReceipt</span></span> | <span data-ttu-id="1c39d-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="1c39d-155">Boolean</span></span> | <span data-ttu-id="1c39d-156">条件または例外を適用するために、受信メッセージが開封確認メッセージであるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1c39d-156">Indicates whether an incoming message must be a read receipt in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="1c39d-157">isSigned</span><span class="sxs-lookup"><span data-stu-id="1c39d-157">isSigned</span></span> | <span data-ttu-id="1c39d-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="1c39d-158">Boolean</span></span> | <span data-ttu-id="1c39d-159">条件または例外を適用するために、受信メッセージが S/MIME 署名されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1c39d-159">Indicates whether an incoming message must be S/MIME-signed in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="1c39d-160">isVoicemail</span><span class="sxs-lookup"><span data-stu-id="1c39d-160">isVoicemail</span></span> | <span data-ttu-id="1c39d-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="1c39d-161">Boolean</span></span> | <span data-ttu-id="1c39d-162">条件または例外を適用するために、受信メッセージがボイス メールかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1c39d-162">Indicates whether an incoming message must be a voice mail in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="1c39d-163">messageActionFlag</span><span class="sxs-lookup"><span data-stu-id="1c39d-163">messageActionFlag</span></span> | <span data-ttu-id="1c39d-164">messageActionFlag</span><span class="sxs-lookup"><span data-stu-id="1c39d-164">messageActionFlag</span></span>  | <span data-ttu-id="1c39d-165">条件または例外を適用するために、受信メッセージに表示されるアクション フラグの値を表します。</span><span class="sxs-lookup"><span data-stu-id="1c39d-165">Represents the flag-for-action value that appears on an incoming message in order for the condition or exception to apply.</span></span> <span data-ttu-id="1c39d-166">使用可能な値は`any`、 `call`、 `doNotForward` `followUp` `fyi` `forward` `noResponseNecessary` `read` `reply`、、、、、、、、、 `review` `replyToAll`です。</span><span class="sxs-lookup"><span data-stu-id="1c39d-166">The possible values are: `any`, `call`, `doNotForward`, `followUp`, `fyi`, `forward`, `noResponseNecessary`, `read`, `reply`, `replyToAll`, `review`.</span></span> |
| <span data-ttu-id="1c39d-167">notSentToMe</span><span class="sxs-lookup"><span data-stu-id="1c39d-167">notSentToMe</span></span> | <span data-ttu-id="1c39d-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="1c39d-168">Boolean</span></span> | <span data-ttu-id="1c39d-169">条件または例外を適用するために、メールボックスの所有者が受信メッセージの受信者でないことを示します。</span><span class="sxs-lookup"><span data-stu-id="1c39d-169">Indicates whether the owner of the mailbox must not be a recipient of an incoming message in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="1c39d-170">recipientContains</span><span class="sxs-lookup"><span data-stu-id="1c39d-170">recipientContains</span></span> | <span data-ttu-id="1c39d-171">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="1c39d-171">String collection</span></span> | <span data-ttu-id="1c39d-172">条件または例外を適用するために、受信メッセージの **ToRecipients** または **CcRecipients** プロパティに表示される文字列を表します。</span><span class="sxs-lookup"><span data-stu-id="1c39d-172">Represents the strings that appear in either the **toRecipients** or **ccRecipients** properties of an incoming message in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="1c39d-173">senderContains</span><span class="sxs-lookup"><span data-stu-id="1c39d-173">senderContains</span></span> | <span data-ttu-id="1c39d-174">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="1c39d-174">String collection</span></span> | <span data-ttu-id="1c39d-175">条件または例外を適用するために、受信メッセージの **From** プロパティに表示される文字列を表します。</span><span class="sxs-lookup"><span data-stu-id="1c39d-175">Represents the strings that appear in the **from** property of an incoming message in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="1c39d-176">sensitivity</span><span class="sxs-lookup"><span data-stu-id="1c39d-176">sensitivity</span></span> | <span data-ttu-id="1c39d-177">sensitivity</span><span class="sxs-lookup"><span data-stu-id="1c39d-177">sensitivity</span></span> | <span data-ttu-id="1c39d-178">条件または例外を適用するために、受信メッセージにスタンプする必要がある秘密度レベルを表します。</span><span class="sxs-lookup"><span data-stu-id="1c39d-178">Represents the sensitivity level that must be stamped on an incoming message in order for the condition or exception to apply.</span></span> <span data-ttu-id="1c39d-179">使用可能な値: `normal`、`personal`、`private`、`confidential`。</span><span class="sxs-lookup"><span data-stu-id="1c39d-179">The possible values are: `normal`, `personal`, `private`, `confidential`.</span></span> |
| <span data-ttu-id="1c39d-180">sentCcMe</span><span class="sxs-lookup"><span data-stu-id="1c39d-180">sentCcMe</span></span> | <span data-ttu-id="1c39d-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="1c39d-181">Boolean</span></span> | <span data-ttu-id="1c39d-182">条件または例外を適用するために、メールボックスの所有者が受信メッセージの **ccRecipients** プロパティにあるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1c39d-182">Indicates whether the owner of the mailbox must be in the **ccRecipients** property of an incoming message in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="1c39d-183">sentOnlyToMe</span><span class="sxs-lookup"><span data-stu-id="1c39d-183">sentOnlyToMe</span></span> | <span data-ttu-id="1c39d-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="1c39d-184">Boolean</span></span> | <span data-ttu-id="1c39d-185">条件または例外を適用するために、メールボックスの所有者が受信メッセージの唯一の受信者かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1c39d-185">Indicates whether the owner of the mailbox must be the only recipient in an incoming message in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="1c39d-186">sentToAddresses</span><span class="sxs-lookup"><span data-stu-id="1c39d-186">sentToAddresses</span></span> | <span data-ttu-id="1c39d-187">[recipient](recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="1c39d-187">[recipient](recipient.md) collection</span></span> | <span data-ttu-id="1c39d-188">条件または例外を適用するために、受信メッセージが送信されたメール アドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="1c39d-188">Represents the email addresses that an incoming message must have been sent to in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="1c39d-189">sentToMe</span><span class="sxs-lookup"><span data-stu-id="1c39d-189">sentToMe</span></span> | <span data-ttu-id="1c39d-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="1c39d-190">Boolean</span></span> | <span data-ttu-id="1c39d-191">条件または例外を適用するために、メールボックスの所有者が受信メッセージの **ToRecipients** プロパティにあるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1c39d-191">Indicates whether the owner of the mailbox must be in the **toRecipients** property of an incoming message in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="1c39d-192">sentToOrCcMe</span><span class="sxs-lookup"><span data-stu-id="1c39d-192">sentToOrCcMe</span></span> | <span data-ttu-id="1c39d-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="1c39d-193">Boolean</span></span> | <span data-ttu-id="1c39d-194">条件または例外を適用するために、メールボックスの所有者が受信メッセージの **toRecipients** または **ccRecipients** プロパティにあるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1c39d-194">Indicates whether the owner of the mailbox must be in either a **toRecipients** or **ccRecipients** property of an incoming message in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="1c39d-195">subjectContains</span><span class="sxs-lookup"><span data-stu-id="1c39d-195">subjectContains</span></span> | <span data-ttu-id="1c39d-196">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="1c39d-196">String collection</span></span> | <span data-ttu-id="1c39d-197">条件または例外を適用するために、受信メッセージの件名に表示される文字列を表します。</span><span class="sxs-lookup"><span data-stu-id="1c39d-197">Represents the strings that appear in the subject of an incoming message in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="1c39d-198">withinSizeRange</span><span class="sxs-lookup"><span data-stu-id="1c39d-198">withinSizeRange</span></span> | [<span data-ttu-id="1c39d-199">sizeRange</span><span class="sxs-lookup"><span data-stu-id="1c39d-199">sizeRange</span></span>](sizerange.md) | <span data-ttu-id="1c39d-200">条件または例外を適用するために、受信メッセージに想定される最小サイズと最大サイズ (単位: キロバイト) を表します。</span><span class="sxs-lookup"><span data-stu-id="1c39d-200">Represents the minimum and maximum sizes (in kilobytes) that an incoming message must fall in between in order for the condition or exception to apply.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="1c39d-201">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1c39d-201">JSON representation</span></span>
<span data-ttu-id="1c39d-202">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="1c39d-202">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
