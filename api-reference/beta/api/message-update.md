---
title: メッセージを更新する
description: メッセージ オブジェクトのプロパティを更新します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 78f030e49f5e9caad5cf505be0118eee5b732752
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573670"
---
# <a name="update-message"></a><span data-ttu-id="2bca1-103">メッセージを更新する</span><span class="sxs-lookup"><span data-stu-id="2bca1-103">Update message</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2bca1-104">メッセージ オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="2bca1-104">Update the properties of a message object.</span></span>
## <a name="permissions"></a><span data-ttu-id="2bca1-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="2bca1-105">Permissions</span></span>
<span data-ttu-id="2bca1-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2bca1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2bca1-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2bca1-108">Permission type</span></span>      | <span data-ttu-id="2bca1-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="2bca1-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2bca1-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2bca1-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2bca1-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2bca1-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="2bca1-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2bca1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2bca1-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2bca1-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="2bca1-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2bca1-114">Application</span></span> | <span data-ttu-id="2bca1-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2bca1-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="2bca1-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2bca1-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/messages/{id}
PATCH /users/{id | userPrincipalName}/messages/{id}
PATCH /me/mailFolders/{id}/messages/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="2bca1-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2bca1-117">Request headers</span></span>
| <span data-ttu-id="2bca1-118">名前</span><span class="sxs-lookup"><span data-stu-id="2bca1-118">Name</span></span>       | <span data-ttu-id="2bca1-119">型</span><span class="sxs-lookup"><span data-stu-id="2bca1-119">Type</span></span> | <span data-ttu-id="2bca1-120">説明</span><span class="sxs-lookup"><span data-stu-id="2bca1-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="2bca1-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="2bca1-121">Authorization</span></span>  | <span data-ttu-id="2bca1-122">string</span><span class="sxs-lookup"><span data-stu-id="2bca1-122">string</span></span>  | <span data-ttu-id="2bca1-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="2bca1-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2bca1-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2bca1-125">Content-Type</span></span> | <span data-ttu-id="2bca1-126">string</span><span class="sxs-lookup"><span data-stu-id="2bca1-126">string</span></span>  | <span data-ttu-id="2bca1-p103">エンティティ本文内のデータの性質です。必須。</span><span class="sxs-lookup"><span data-stu-id="2bca1-p103">Nature of the data in the body of an entity. Required.</span></span> |
## <a name="request-body"></a><span data-ttu-id="2bca1-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="2bca1-129">Request body</span></span>
<span data-ttu-id="2bca1-130">要求本文で、更新する関連フィールドの値を指定します。</span><span class="sxs-lookup"><span data-stu-id="2bca1-130">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="2bca1-131">要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変更に基づいて再計算されます。</span><span class="sxs-lookup"><span data-stu-id="2bca1-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="2bca1-132">最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="2bca1-132">For best performance you shouldn't include existing values that haven't changed.</span></span> <span data-ttu-id="2bca1-133">次のプロパティを更新することができます。</span><span class="sxs-lookup"><span data-stu-id="2bca1-133">The following properties can be updated.</span></span>

| <span data-ttu-id="2bca1-134">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2bca1-134">Property</span></span>     | <span data-ttu-id="2bca1-135">型</span><span class="sxs-lookup"><span data-stu-id="2bca1-135">Type</span></span>   |<span data-ttu-id="2bca1-136">説明</span><span class="sxs-lookup"><span data-stu-id="2bca1-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2bca1-137">bccRecipients</span><span class="sxs-lookup"><span data-stu-id="2bca1-137">bccRecipients</span></span>|<span data-ttu-id="2bca1-138">Recipient</span><span class="sxs-lookup"><span data-stu-id="2bca1-138">Recipient</span></span>|<span data-ttu-id="2bca1-139">メッセージの BCC 受信者。</span><span class="sxs-lookup"><span data-stu-id="2bca1-139">The Bcc recipients for the message.</span></span> |
|<span data-ttu-id="2bca1-140">body</span><span class="sxs-lookup"><span data-stu-id="2bca1-140">body</span></span>|<span data-ttu-id="2bca1-141">ItemBody</span><span class="sxs-lookup"><span data-stu-id="2bca1-141">ItemBody</span></span>|<span data-ttu-id="2bca1-142">メッセージの本文。</span><span class="sxs-lookup"><span data-stu-id="2bca1-142">The body of the message.</span></span> <span data-ttu-id="2bca1-143">更新可能な場合にのみ isDraft = true です。</span><span class="sxs-lookup"><span data-stu-id="2bca1-143">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="2bca1-144">categories</span><span class="sxs-lookup"><span data-stu-id="2bca1-144">categories</span></span>|<span data-ttu-id="2bca1-145">String コレクション</span><span class="sxs-lookup"><span data-stu-id="2bca1-145">String collection</span></span>|<span data-ttu-id="2bca1-146">メッセージに関連付けられたカテゴリ。</span><span class="sxs-lookup"><span data-stu-id="2bca1-146">The categories associated with the message.</span></span>|
|<span data-ttu-id="2bca1-147">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="2bca1-147">ccRecipients</span></span>|<span data-ttu-id="2bca1-148">Recipient collection</span><span class="sxs-lookup"><span data-stu-id="2bca1-148">Recipient collection</span></span>|<span data-ttu-id="2bca1-149">メッセージの CC 受信者。</span><span class="sxs-lookup"><span data-stu-id="2bca1-149">The Cc recipients for the message.</span></span> |
|<span data-ttu-id="2bca1-150">from</span><span class="sxs-lookup"><span data-stu-id="2bca1-150">from</span></span>|<span data-ttu-id="2bca1-151">Recipient</span><span class="sxs-lookup"><span data-stu-id="2bca1-151">Recipient</span></span>|<span data-ttu-id="2bca1-152">メッセージのメールボックス所有者と送信者。</span><span class="sxs-lookup"><span data-stu-id="2bca1-152">The mailbox owner and sender of the message.</span></span> <span data-ttu-id="2bca1-153">使用される実際のメールボックスに対応する必要があります。</span><span class="sxs-lookup"><span data-stu-id="2bca1-153">Must correspond to the actual mailbox used.</span></span> |
|<span data-ttu-id="2bca1-154">importance</span><span class="sxs-lookup"><span data-stu-id="2bca1-154">importance</span></span>|<span data-ttu-id="2bca1-155">String</span><span class="sxs-lookup"><span data-stu-id="2bca1-155">String</span></span>|<span data-ttu-id="2bca1-p107">メッセージの重要度です。可能な値は、`Low`、`Normal`、`High` です。</span><span class="sxs-lookup"><span data-stu-id="2bca1-p107">The importance of the message. Possible values are: `Low`, `Normal`, `High`.</span></span>|
|<span data-ttu-id="2bca1-158">inferenceClassification</span><span class="sxs-lookup"><span data-stu-id="2bca1-158">inferenceClassification</span></span> | <span data-ttu-id="2bca1-159">String</span><span class="sxs-lookup"><span data-stu-id="2bca1-159">String</span></span> | <span data-ttu-id="2bca1-p108">推定される関連性や重要性、または明示的なオーバーライドに基づく、ユーザーのメッセージの分類です。使用可能な値: `focused` または `other`。</span><span class="sxs-lookup"><span data-stu-id="2bca1-p108">The classification of the message for the user, based on inferred relevance or importance, or on an explicit override. Possible values are: `focused` or `other`.</span></span> |
|<span data-ttu-id="2bca1-162">internetMessageId</span><span class="sxs-lookup"><span data-stu-id="2bca1-162">internetMessageId</span></span> |<span data-ttu-id="2bca1-163">String</span><span class="sxs-lookup"><span data-stu-id="2bca1-163">String</span></span> |<span data-ttu-id="2bca1-164">[RFC2822](https://www.ietf.org/rfc/rfc2822.txt) によって指定された形式のメッセージ ID。</span><span class="sxs-lookup"><span data-stu-id="2bca1-164">The message ID in the format specified by [RFC2822](https://www.ietf.org/rfc/rfc2822.txt).</span></span> <span data-ttu-id="2bca1-165">更新可能な場合にのみ isDraft = true です。</span><span class="sxs-lookup"><span data-stu-id="2bca1-165">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="2bca1-166">isDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="2bca1-166">isDeliveryReceiptRequested</span></span>|<span data-ttu-id="2bca1-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="2bca1-167">Boolean</span></span>|<span data-ttu-id="2bca1-168">メッセージの開封応答が要求されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="2bca1-168">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="2bca1-169">isRead</span><span class="sxs-lookup"><span data-stu-id="2bca1-169">isRead</span></span>|<span data-ttu-id="2bca1-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="2bca1-170">Boolean</span></span>|<span data-ttu-id="2bca1-171">メッセージが開封されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="2bca1-171">Indicates whether the message has been read.</span></span>|
|<span data-ttu-id="2bca1-172">isReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="2bca1-172">isReadReceiptRequested</span></span>|<span data-ttu-id="2bca1-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="2bca1-173">Boolean</span></span>|<span data-ttu-id="2bca1-174">メッセージの開封確認メッセージが要求されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="2bca1-174">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="2bca1-175">multiValueLegacyExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="2bca1-175">multiValueLegacyExtendedProperty</span></span>| <span data-ttu-id="2bca1-176">[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) collection</span><span class="sxs-lookup"><span data-stu-id="2bca1-176">[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="2bca1-177">複数値のコレクションでは、メッセージに対して定義されたプロパティを拡張します。</span><span class="sxs-lookup"><span data-stu-id="2bca1-177">The collection of multi-value extended properties defined for the message.</span></span> <span data-ttu-id="2bca1-178">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="2bca1-178">Nullable.</span></span>|
|<span data-ttu-id="2bca1-179">replyTo</span><span class="sxs-lookup"><span data-stu-id="2bca1-179">replyTo</span></span>|<span data-ttu-id="2bca1-180">Recipient collection</span><span class="sxs-lookup"><span data-stu-id="2bca1-180">Recipient collection</span></span>|<span data-ttu-id="2bca1-181">返信時に使用される電子メール アドレス。</span><span class="sxs-lookup"><span data-stu-id="2bca1-181">The email addresses to use when replying.</span></span> <span data-ttu-id="2bca1-182">更新可能な場合にのみ isDraft = true です。</span><span class="sxs-lookup"><span data-stu-id="2bca1-182">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="2bca1-183">sender</span><span class="sxs-lookup"><span data-stu-id="2bca1-183">sender</span></span>|<span data-ttu-id="2bca1-184">Recipient</span><span class="sxs-lookup"><span data-stu-id="2bca1-184">Recipient</span></span>|<span data-ttu-id="2bca1-185">メッセージを生成するために実際に使用されるアカウント。</span><span class="sxs-lookup"><span data-stu-id="2bca1-185">The account that is actually used to generate the message.</span></span> <span data-ttu-id="2bca1-186">[共有されているメールボックス](https://docs.microsoft.com/en-us/exchange/collaboration/shared-mailboxes/shared-mailboxes)、または[委任](https://support.office.com/en-us/article/allow-someone-else-to-manage-your-mail-and-calendar-41c40c04-3bd1-4d22-963a-28eafec25926)としてメッセージを送信するメッセージを送信するときに更新します。</span><span class="sxs-lookup"><span data-stu-id="2bca1-186">Updatable when sending a message from a [shared mailbox](https://docs.microsoft.com/en-us/exchange/collaboration/shared-mailboxes/shared-mailboxes), or sending a message as a [delegate](https://support.office.com/en-us/article/allow-someone-else-to-manage-your-mail-and-calendar-41c40c04-3bd1-4d22-963a-28eafec25926).</span></span> <span data-ttu-id="2bca1-187">いずれの場合も、値は、使用される実際のメールボックスに対応する必要があります。</span><span class="sxs-lookup"><span data-stu-id="2bca1-187">In any case, the value must correspond to the actual mailbox used.</span></span>|
|<span data-ttu-id="2bca1-188">singleValueLegacyExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="2bca1-188">singleValueLegacyExtendedProperty</span></span>| <span data-ttu-id="2bca1-189">[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) collection</span><span class="sxs-lookup"><span data-stu-id="2bca1-189">[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="2bca1-190">単一値のコレクションでは、メッセージに対して定義されたプロパティを拡張します。</span><span class="sxs-lookup"><span data-stu-id="2bca1-190">The collection of single-value extended properties defined for the message.</span></span> <span data-ttu-id="2bca1-191">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="2bca1-191">Nullable.</span></span>|
|<span data-ttu-id="2bca1-192">subject</span><span class="sxs-lookup"><span data-stu-id="2bca1-192">subject</span></span>|<span data-ttu-id="2bca1-193">String</span><span class="sxs-lookup"><span data-stu-id="2bca1-193">String</span></span>|<span data-ttu-id="2bca1-194">メッセージの件名。</span><span class="sxs-lookup"><span data-stu-id="2bca1-194">The subject of the message.</span></span> <span data-ttu-id="2bca1-195">更新可能な場合にのみ isDraft = true です。</span><span class="sxs-lookup"><span data-stu-id="2bca1-195">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="2bca1-196">toRecipients</span><span class="sxs-lookup"><span data-stu-id="2bca1-196">toRecipients</span></span>|<span data-ttu-id="2bca1-197">Recipient collection</span><span class="sxs-lookup"><span data-stu-id="2bca1-197">Recipient collection</span></span>|<span data-ttu-id="2bca1-198">宛先] の受信者のメッセージです。</span><span class="sxs-lookup"><span data-stu-id="2bca1-198">The To recipients for the message.</span></span> |

<span data-ttu-id="2bca1-199">**メッセージ** リソースは[拡張機能](/graph/extensibility-overview)をサポートしているため、`PATCH` 操作を使用して、既存の**メッセージ** インスタンスで拡張機能のカスタム プロパティにあるアプリ固有のデータを追加、更新、または削除することができます。</span><span class="sxs-lookup"><span data-stu-id="2bca1-199">Since the **message** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **message** instance.</span></span>

## <a name="response"></a><span data-ttu-id="2bca1-200">応答</span><span class="sxs-lookup"><span data-stu-id="2bca1-200">Response</span></span>

<span data-ttu-id="2bca1-201">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [message](../resources/message.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="2bca1-201">If successful, this method returns a `200 OK` response code and updated [message](../resources/message.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2bca1-202">例</span><span class="sxs-lookup"><span data-stu-id="2bca1-202">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2bca1-203">要求</span><span class="sxs-lookup"><span data-stu-id="2bca1-203">Request</span></span>
<span data-ttu-id="2bca1-204">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2bca1-204">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_message"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/messages/{id}
Content-type: application/json
Content-length: 248

{
  "subject": "subject-value",
  "body": {
    "contentType": "",
    "content": "content-value"
  },
  "inferenceClassification": "other"
}
```
##### <a name="response"></a><span data-ttu-id="2bca1-205">応答</span><span class="sxs-lookup"><span data-stu-id="2bca1-205">Response</span></span>
<span data-ttu-id="2bca1-p115">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="2bca1-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 248

{
  "receivedDateTime": "2016-10-19T10:37:00Z",
  "sentDateTime": "2016-10-19T10:37:00Z",
  "hasAttachments": true,
  "subject": "subject-value",
  "body": {
    "contentType": "",
    "content": "content-value"
  },
  "bodyPreview": "bodyPreview-value",
  "inferenceClassification": "other"
}
```

## <a name="see-also"></a><span data-ttu-id="2bca1-209">関連項目</span><span class="sxs-lookup"><span data-stu-id="2bca1-209">See also</span></span>

- [<span data-ttu-id="2bca1-210">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="2bca1-210">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="2bca1-211">オープン拡張機能を使用したユーザーへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="2bca1-211">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="2bca1-212">スキーマ拡張機能を使用したグループへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="2bca1-212">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update message",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/message-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
