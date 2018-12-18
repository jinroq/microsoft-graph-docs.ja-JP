---
title: messageRulePredicates リソースの種類
description: ルールで使用可能な条件および例外のセットを表します。
author: angelgolfer-ms
ms.openlocfilehash: f83eb524605133d069eb5ff1f902067d3611fdbd
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27304712"
---
# <a name="messagerulepredicates-resource-type"></a><span data-ttu-id="1e53b-103">messageRulePredicates リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1e53b-103">messageRulePredicates resource type</span></span>

> <span data-ttu-id="1e53b-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="1e53b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1e53b-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1e53b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1e53b-106">ルールで使用可能な条件および例外のセットを表します。</span><span class="sxs-lookup"><span data-stu-id="1e53b-106">Represents the set of conditions and exceptions that are available for a rule.</span></span>

## <a name="properties"></a><span data-ttu-id="1e53b-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1e53b-107">Properties</span></span>
| <span data-ttu-id="1e53b-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1e53b-108">Property</span></span>     | <span data-ttu-id="1e53b-109">種類</span><span class="sxs-lookup"><span data-stu-id="1e53b-109">Type</span></span>   |<span data-ttu-id="1e53b-110">説明</span><span class="sxs-lookup"><span data-stu-id="1e53b-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1e53b-111">bodyContains</span><span class="sxs-lookup"><span data-stu-id="1e53b-111">bodyContains</span></span> | <span data-ttu-id="1e53b-112">コレクション (String)</span><span class="sxs-lookup"><span data-stu-id="1e53b-112">Collection (String)</span></span> | <span data-ttu-id="1e53b-113">条件または例外を適用するために、受信メッセージの本文に表示される文字列を表します。</span><span class="sxs-lookup"><span data-stu-id="1e53b-113">Represents the strings that should appear in the body of an incoming message in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="1e53b-114">bodyOrSubjectContains</span><span class="sxs-lookup"><span data-stu-id="1e53b-114">bodyOrSubjectContains</span></span> | <span data-ttu-id="1e53b-115">コレクション (String)</span><span class="sxs-lookup"><span data-stu-id="1e53b-115">Collection (String)</span></span> | <span data-ttu-id="1e53b-116">条件または例外を適用するために、受信メッセージの本文または件名に表示される文字列を表します。</span><span class="sxs-lookup"><span data-stu-id="1e53b-116">Represents the strings that should appear in the body or subject of an incoming message in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="1e53b-117">categories</span><span class="sxs-lookup"><span data-stu-id="1e53b-117">categories</span></span> | <span data-ttu-id="1e53b-118">コレクション (String)</span><span class="sxs-lookup"><span data-stu-id="1e53b-118">Collection (String)</span></span> | <span data-ttu-id="1e53b-119">条件または例外を適用するために、受信メッセージにラベルを付けるカテゴリを表します。</span><span class="sxs-lookup"><span data-stu-id="1e53b-119">Represents the categories that an incoming message should be labeled with in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="1e53b-120">fromAddresses</span><span class="sxs-lookup"><span data-stu-id="1e53b-120">fromAddresses</span></span> | <span data-ttu-id="1e53b-121">コレクション ([Recipient](recipient.md))</span><span class="sxs-lookup"><span data-stu-id="1e53b-121">Collection ([recipient](recipient.md))</span></span> | <span data-ttu-id="1e53b-122">条件または例外を適用するために、受信メッセージの特定の送信者のメール アドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="1e53b-122">Represents the specific sender email addresses of an incoming message in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="1e53b-123">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="1e53b-123">hasAttachments</span></span> | <span data-ttu-id="1e53b-124">ブール型</span><span class="sxs-lookup"><span data-stu-id="1e53b-124">Boolean</span></span> | <span data-ttu-id="1e53b-125">条件または例外を適用するために、受信メッセージに添付ファイルがあるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1e53b-125">Indicates whether an incoming message must have attachments in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="1e53b-126">headerContains</span><span class="sxs-lookup"><span data-stu-id="1e53b-126">headerContains</span></span> | <span data-ttu-id="1e53b-127">コレクション (String)</span><span class="sxs-lookup"><span data-stu-id="1e53b-127">Collection (String)</span></span> | <span data-ttu-id="1e53b-128">条件または例外を適用するために、受信メッセージのヘッダーに表示される文字列を表します。</span><span class="sxs-lookup"><span data-stu-id="1e53b-128">Represents the strings that appear in the headers of an incoming message in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="1e53b-129">importance</span><span class="sxs-lookup"><span data-stu-id="1e53b-129">importance</span></span> | <span data-ttu-id="1e53b-130">String</span><span class="sxs-lookup"><span data-stu-id="1e53b-130">String</span></span> | <span data-ttu-id="1e53b-131">条件または例外を適用するために、受信メッセージに記録される重要性: `low`、`normal`、`high`。</span><span class="sxs-lookup"><span data-stu-id="1e53b-131">The importance that is stamped on an incoming message in order for the condition or exception to apply: `low`, `normal`, `high`.</span></span> |
| <span data-ttu-id="1e53b-132">isApprovalRequest</span><span class="sxs-lookup"><span data-stu-id="1e53b-132">isApprovalRequest</span></span> | <span data-ttu-id="1e53b-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e53b-133">Boolean</span></span> | <span data-ttu-id="1e53b-134">条件または例外を適用するために、受信メッセージが承認要求であるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1e53b-134">Indicates whether an incoming message must be an approval request in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="1e53b-135">isAutomaticForward</span><span class="sxs-lookup"><span data-stu-id="1e53b-135">isAutomaticForward</span></span> | <span data-ttu-id="1e53b-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e53b-136">Boolean</span></span> | <span data-ttu-id="1e53b-137">条件または例外を適用するために、受信メッセージが自動的に転送されるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1e53b-137">Indicates whether an incoming message must be automatically forwarded in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="1e53b-138">isAutomaticReply</span><span class="sxs-lookup"><span data-stu-id="1e53b-138">isAutomaticReply</span></span> | <span data-ttu-id="1e53b-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e53b-139">Boolean</span></span> | <span data-ttu-id="1e53b-140">条件または例外を適用するために、受信メッセージが自動返信であるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1e53b-140">Indicates whether an incoming message must be an auto reply in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="1e53b-141">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="1e53b-141">isEncrypted</span></span> | <span data-ttu-id="1e53b-142">ブール型</span><span class="sxs-lookup"><span data-stu-id="1e53b-142">Boolean</span></span> | <span data-ttu-id="1e53b-143">条件または例外を適用するために、受信メッセージが暗号化されるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1e53b-143">Indicates whether an incoming message must be encrypted in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="1e53b-144">isMeetingRequest</span><span class="sxs-lookup"><span data-stu-id="1e53b-144">isMeetingRequest</span></span> | <span data-ttu-id="1e53b-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e53b-145">Boolean</span></span> | <span data-ttu-id="1e53b-146">条件または例外を適用するために、受信メッセージが会議出席依頼であるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1e53b-146">Indicates whether an incoming message must be a meeting request in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="1e53b-147">isMeetingResponse</span><span class="sxs-lookup"><span data-stu-id="1e53b-147">isMeetingResponse</span></span> | <span data-ttu-id="1e53b-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e53b-148">Boolean</span></span> | <span data-ttu-id="1e53b-149">条件または例外を適用するために、受信メッセージが会議出席依頼の返信であるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1e53b-149">Indicates whether an incoming message must be a meeting response in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="1e53b-150">isNonDeliveryReport</span><span class="sxs-lookup"><span data-stu-id="1e53b-150">isNonDeliveryReport</span></span> | <span data-ttu-id="1e53b-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e53b-151">Boolean</span></span> | <span data-ttu-id="1e53b-152">条件または例外を適用するために、受信メッセージが配信不能レポートであるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1e53b-152">Indicates whether an incoming message must be a non-delivery report in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="1e53b-153">IsPermissionControlled</span><span class="sxs-lookup"><span data-stu-id="1e53b-153">isPermissionControlled</span></span> | <span data-ttu-id="1e53b-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e53b-154">Boolean</span></span> | <span data-ttu-id="1e53b-155">条件または例外を適用するために、受信メッセージがアクセス許可制御 (RMS 保護) されるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1e53b-155">Indicates whether an incoming message must be permission controlled (RMS-protected) in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="1e53b-156">isReadReceipt</span><span class="sxs-lookup"><span data-stu-id="1e53b-156">isReadReceipt</span></span> | <span data-ttu-id="1e53b-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e53b-157">Boolean</span></span> | <span data-ttu-id="1e53b-158">条件または例外を適用するために、受信メッセージが開封確認メッセージであるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1e53b-158">Indicates whether an incoming message must be a read receipt in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="1e53b-159">isSigned</span><span class="sxs-lookup"><span data-stu-id="1e53b-159">isSigned</span></span> | <span data-ttu-id="1e53b-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e53b-160">Boolean</span></span> | <span data-ttu-id="1e53b-161">条件または例外を適用するために、受信メッセージが S/MIME 署名されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1e53b-161">Indicates whether an incoming message must be S/MIME-signed in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="1e53b-162">isVoicemail</span><span class="sxs-lookup"><span data-stu-id="1e53b-162">isVoicemail</span></span> | <span data-ttu-id="1e53b-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e53b-163">Boolean</span></span> | <span data-ttu-id="1e53b-164">条件または例外を適用するために、受信メッセージがボイス メールかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1e53b-164">Indicates whether an incoming message must be a voice mail in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="1e53b-165">messageActionFlag</span><span class="sxs-lookup"><span data-stu-id="1e53b-165">messageActionFlag</span></span> | <span data-ttu-id="1e53b-166">String</span><span class="sxs-lookup"><span data-stu-id="1e53b-166">String</span></span>  | <span data-ttu-id="1e53b-167">条件または例外を適用するために、受信メッセージに表示されるアクション フラグの値を表します。</span><span class="sxs-lookup"><span data-stu-id="1e53b-167">Represents the flag-for-action value that appears on an incoming message in order for the condition or exception to apply.</span></span> <span data-ttu-id="1e53b-168">使用可能な値は、`any`、`call`、`doNotForward`、`followUp`、`fyi`、`forward`、`noResponseNecessary`、`read`、`reply`、`replyToAll`、`review` です。</span><span class="sxs-lookup"><span data-stu-id="1e53b-168">Possible values are: `any`, `call`, `doNotForward`, `followUp`, `fyi`, `forward`, `noResponseNecessary`, `read`, `reply`, `replyToAll`, `review`.</span></span> |
| <span data-ttu-id="1e53b-169">notSentToMe</span><span class="sxs-lookup"><span data-stu-id="1e53b-169">notSentToMe</span></span> | <span data-ttu-id="1e53b-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e53b-170">Boolean</span></span> | <span data-ttu-id="1e53b-171">条件または例外を適用するために、メールボックスの所有者が受信メッセージの受信者でないことを示します。</span><span class="sxs-lookup"><span data-stu-id="1e53b-171">Indicates whether the owner of the mailbox must not be a recipient of an incoming message in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="1e53b-172">recipientContains</span><span class="sxs-lookup"><span data-stu-id="1e53b-172">recipientContains</span></span> | <span data-ttu-id="1e53b-173">コレクション (String)</span><span class="sxs-lookup"><span data-stu-id="1e53b-173">Collection (String)</span></span> | <span data-ttu-id="1e53b-174">条件または例外を適用するために、受信メッセージの **ToRecipients** または **CcRecipients** プロパティに表示される文字列を表します。</span><span class="sxs-lookup"><span data-stu-id="1e53b-174">Represents the strings that appear in either the **toRecipients** or **ccRecipients** properties of an incoming message in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="1e53b-175">senderContains</span><span class="sxs-lookup"><span data-stu-id="1e53b-175">senderContains</span></span> | <span data-ttu-id="1e53b-176">コレクション (String)</span><span class="sxs-lookup"><span data-stu-id="1e53b-176">Collection (String)</span></span> | <span data-ttu-id="1e53b-177">条件または例外を適用するために、受信メッセージの **From** プロパティに表示される文字列を表します。</span><span class="sxs-lookup"><span data-stu-id="1e53b-177">Represents the strings that appear in the **from** property of an incoming message in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="1e53b-178">sensitivity</span><span class="sxs-lookup"><span data-stu-id="1e53b-178">sensitivity</span></span> | <span data-ttu-id="1e53b-179">String</span><span class="sxs-lookup"><span data-stu-id="1e53b-179">String</span></span> | <span data-ttu-id="1e53b-p103">条件または例外を適用するために、受信メッセージに記録される秘密度レベルを表します。使用可能な値: `normal`、`personal`、`private`、`confidential`。</span><span class="sxs-lookup"><span data-stu-id="1e53b-p103">Represents the sensitivity level that must be stamped on an incoming message in order for the condition or exception to apply. Possible values are: `normal`, `personal`, `private`, `confidential`.</span></span> |
| <span data-ttu-id="1e53b-182">sentCcMe</span><span class="sxs-lookup"><span data-stu-id="1e53b-182">sentCcMe</span></span> | <span data-ttu-id="1e53b-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e53b-183">Boolean</span></span> | <span data-ttu-id="1e53b-184">条件または例外を適用するために、メールボックスの所有者が受信メッセージの **ccRecipients** プロパティにあるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1e53b-184">Indicates whether the owner of the mailbox must be in the **ccRecipients** property of an incoming message in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="1e53b-185">sentOnlyToMe</span><span class="sxs-lookup"><span data-stu-id="1e53b-185">sentOnlyToMe</span></span> | <span data-ttu-id="1e53b-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e53b-186">Boolean</span></span> | <span data-ttu-id="1e53b-187">条件または例外を適用するために、メールボックスの所有者が受信メッセージの唯一の受信者かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1e53b-187">Indicates whether the owner of the mailbox must be the only recipient in an incoming message in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="1e53b-188">sentToAddresses</span><span class="sxs-lookup"><span data-stu-id="1e53b-188">sentToAddresses</span></span> | <span data-ttu-id="1e53b-189">コレクション ([Recipient](recipient.md))</span><span class="sxs-lookup"><span data-stu-id="1e53b-189">Collection ([recipient](recipient.md))</span></span> | <span data-ttu-id="1e53b-190">条件または例外を適用するために、受信メッセージが送信されたメール アドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="1e53b-190">Represents the email addresses that an incoming message must have been sent to in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="1e53b-191">sentToMe</span><span class="sxs-lookup"><span data-stu-id="1e53b-191">sentToMe</span></span> | <span data-ttu-id="1e53b-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e53b-192">Boolean</span></span> | <span data-ttu-id="1e53b-193">条件または例外を適用するために、メールボックスの所有者が受信メッセージの **ToRecipients** プロパティにあるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1e53b-193">Indicates whether the owner of the mailbox must be in the **toRecipients** property of an incoming message in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="1e53b-194">sentToOrCcMe</span><span class="sxs-lookup"><span data-stu-id="1e53b-194">sentToOrCcMe</span></span> | <span data-ttu-id="1e53b-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e53b-195">Boolean</span></span> | <span data-ttu-id="1e53b-196">条件または例外を適用するために、メールボックスの所有者が受信メッセージの **toRecipients** または **ccRecipients** プロパティにあるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1e53b-196">Indicates whether the owner of the mailbox must be in either a **toRecipients** or **ccRecipients** property of an incoming message in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="1e53b-197">subjectContains</span><span class="sxs-lookup"><span data-stu-id="1e53b-197">subjectContains</span></span> | <span data-ttu-id="1e53b-198">コレクション (String)</span><span class="sxs-lookup"><span data-stu-id="1e53b-198">Collection (String)</span></span> | <span data-ttu-id="1e53b-199">条件または例外を適用するために、受信メッセージの件名に表示される文字列を表します。</span><span class="sxs-lookup"><span data-stu-id="1e53b-199">Represents the strings that appear in the subject of an incoming message in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="1e53b-200">withinSizeRange</span><span class="sxs-lookup"><span data-stu-id="1e53b-200">withinSizeRange</span></span> | [<span data-ttu-id="1e53b-201">sizeRange</span><span class="sxs-lookup"><span data-stu-id="1e53b-201">sizeRange</span></span>](sizerange.md) | <span data-ttu-id="1e53b-202">条件または例外を適用するために、受信メッセージに想定される最小サイズと最大サイズ (単位: キロバイト) を表します。</span><span class="sxs-lookup"><span data-stu-id="1e53b-202">Represents the minimum and maximum sizes (in kilobytes) that an incoming message must fall in between in order for the condition or exception to apply.</span></span> |



## <a name="json-representation"></a><span data-ttu-id="1e53b-203">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1e53b-203">JSON representation</span></span>
<span data-ttu-id="1e53b-204">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="1e53b-204">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "messageRulePredicates resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->