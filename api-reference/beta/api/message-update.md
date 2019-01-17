---
title: メッセージを更新する
description: メッセージ オブジェクトのプロパティを更新します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 6553365ffd31c56348c930be5562ebd65abc734d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27977767"
---
# <a name="update-message"></a><span data-ttu-id="bba6a-103">メッセージを更新する</span><span class="sxs-lookup"><span data-stu-id="bba6a-103">Update message</span></span>

> <span data-ttu-id="bba6a-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="bba6a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bba6a-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bba6a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bba6a-106">メッセージ オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="bba6a-106">Update the properties of a message object.</span></span>
## <a name="permissions"></a><span data-ttu-id="bba6a-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="bba6a-107">Permissions</span></span>
<span data-ttu-id="bba6a-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bba6a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bba6a-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="bba6a-110">Permission type</span></span>      | <span data-ttu-id="bba6a-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="bba6a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bba6a-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="bba6a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="bba6a-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bba6a-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="bba6a-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="bba6a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bba6a-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bba6a-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="bba6a-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="bba6a-116">Application</span></span> | <span data-ttu-id="bba6a-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bba6a-117">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="bba6a-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="bba6a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/messages/{id}
PATCH /users/{id | userPrincipalName}/messages/{id}
PATCH /me/mailFolders/{id}/messages/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="bba6a-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bba6a-119">Request headers</span></span>
| <span data-ttu-id="bba6a-120">名前</span><span class="sxs-lookup"><span data-stu-id="bba6a-120">Name</span></span>       | <span data-ttu-id="bba6a-121">型</span><span class="sxs-lookup"><span data-stu-id="bba6a-121">Type</span></span> | <span data-ttu-id="bba6a-122">説明</span><span class="sxs-lookup"><span data-stu-id="bba6a-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="bba6a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bba6a-123">Authorization</span></span>  | <span data-ttu-id="bba6a-124">string</span><span class="sxs-lookup"><span data-stu-id="bba6a-124">string</span></span>  | <span data-ttu-id="bba6a-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="bba6a-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="bba6a-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bba6a-127">Content-Type</span></span> | <span data-ttu-id="bba6a-128">string</span><span class="sxs-lookup"><span data-stu-id="bba6a-128">string</span></span>  | <span data-ttu-id="bba6a-p104">エンティティ本文内のデータの性質です。必須。</span><span class="sxs-lookup"><span data-stu-id="bba6a-p104">Nature of the data in the body of an entity. Required.</span></span> |
## <a name="request-body"></a><span data-ttu-id="bba6a-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="bba6a-131">Request body</span></span>
<span data-ttu-id="bba6a-132">要求本文で、更新する関連フィールドの値を指定します。</span><span class="sxs-lookup"><span data-stu-id="bba6a-132">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="bba6a-133">要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変更に基づいて再計算されます。</span><span class="sxs-lookup"><span data-stu-id="bba6a-133">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="bba6a-134">最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="bba6a-134">For best performance you shouldn't include existing values that haven't changed.</span></span> <span data-ttu-id="bba6a-135">次のプロパティを更新することができます。</span><span class="sxs-lookup"><span data-stu-id="bba6a-135">The following properties can be updated.</span></span>

| <span data-ttu-id="bba6a-136">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bba6a-136">Property</span></span>     | <span data-ttu-id="bba6a-137">型</span><span class="sxs-lookup"><span data-stu-id="bba6a-137">Type</span></span>   |<span data-ttu-id="bba6a-138">説明</span><span class="sxs-lookup"><span data-stu-id="bba6a-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bba6a-139">bccRecipients</span><span class="sxs-lookup"><span data-stu-id="bba6a-139">bccRecipients</span></span>|<span data-ttu-id="bba6a-140">Recipient</span><span class="sxs-lookup"><span data-stu-id="bba6a-140">Recipient</span></span>|<span data-ttu-id="bba6a-141">メッセージの BCC 受信者。</span><span class="sxs-lookup"><span data-stu-id="bba6a-141">The Bcc recipients for the message.</span></span> |
|<span data-ttu-id="bba6a-142">body</span><span class="sxs-lookup"><span data-stu-id="bba6a-142">body</span></span>|<span data-ttu-id="bba6a-143">ItemBody</span><span class="sxs-lookup"><span data-stu-id="bba6a-143">ItemBody</span></span>|<span data-ttu-id="bba6a-144">メッセージの本文。</span><span class="sxs-lookup"><span data-stu-id="bba6a-144">The body of the message.</span></span> <span data-ttu-id="bba6a-145">更新可能な場合にのみ isDraft = true です。</span><span class="sxs-lookup"><span data-stu-id="bba6a-145">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="bba6a-146">categories</span><span class="sxs-lookup"><span data-stu-id="bba6a-146">categories</span></span>|<span data-ttu-id="bba6a-147">String コレクション</span><span class="sxs-lookup"><span data-stu-id="bba6a-147">String collection</span></span>|<span data-ttu-id="bba6a-148">メッセージに関連付けられたカテゴリ。</span><span class="sxs-lookup"><span data-stu-id="bba6a-148">The categories associated with the message.</span></span>|
|<span data-ttu-id="bba6a-149">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="bba6a-149">ccRecipients</span></span>|<span data-ttu-id="bba6a-150">Recipient collection</span><span class="sxs-lookup"><span data-stu-id="bba6a-150">Recipient collection</span></span>|<span data-ttu-id="bba6a-151">メッセージの CC 受信者。</span><span class="sxs-lookup"><span data-stu-id="bba6a-151">The Cc recipients for the message.</span></span> |
|<span data-ttu-id="bba6a-152">from</span><span class="sxs-lookup"><span data-stu-id="bba6a-152">from</span></span>|<span data-ttu-id="bba6a-153">Recipient</span><span class="sxs-lookup"><span data-stu-id="bba6a-153">Recipient</span></span>|<span data-ttu-id="bba6a-154">メッセージのメールボックス所有者と送信者。</span><span class="sxs-lookup"><span data-stu-id="bba6a-154">The mailbox owner and sender of the message.</span></span> <span data-ttu-id="bba6a-155">使用される実際のメールボックスに対応する必要があります。</span><span class="sxs-lookup"><span data-stu-id="bba6a-155">Must correspond to the actual mailbox used.</span></span> |
|<span data-ttu-id="bba6a-156">importance</span><span class="sxs-lookup"><span data-stu-id="bba6a-156">importance</span></span>|<span data-ttu-id="bba6a-157">String</span><span class="sxs-lookup"><span data-stu-id="bba6a-157">String</span></span>|<span data-ttu-id="bba6a-p108">メッセージの重要度です。可能な値は、`Low`、`Normal`、`High` です。</span><span class="sxs-lookup"><span data-stu-id="bba6a-p108">The importance of the message. Possible values are: `Low`, `Normal`, `High`.</span></span>|
|<span data-ttu-id="bba6a-160">inferenceClassification</span><span class="sxs-lookup"><span data-stu-id="bba6a-160">inferenceClassification</span></span> | <span data-ttu-id="bba6a-161">String</span><span class="sxs-lookup"><span data-stu-id="bba6a-161">String</span></span> | <span data-ttu-id="bba6a-p109">推定される関連性や重要性、または明示的なオーバーライドに基づく、ユーザーのメッセージの分類です。使用可能な値: `focused` または `other`。</span><span class="sxs-lookup"><span data-stu-id="bba6a-p109">The classification of the message for the user, based on inferred relevance or importance, or on an explicit override. Possible values are: `focused` or `other`.</span></span> |
|<span data-ttu-id="bba6a-164">internetMessageId</span><span class="sxs-lookup"><span data-stu-id="bba6a-164">internetMessageId</span></span> |<span data-ttu-id="bba6a-165">String</span><span class="sxs-lookup"><span data-stu-id="bba6a-165">String</span></span> |<span data-ttu-id="bba6a-166">[RFC2822](https://www.ietf.org/rfc/rfc2822.txt) によって指定された形式のメッセージ ID。</span><span class="sxs-lookup"><span data-stu-id="bba6a-166">The message ID in the format specified by [RFC2822](https://www.ietf.org/rfc/rfc2822.txt).</span></span> <span data-ttu-id="bba6a-167">更新可能な場合にのみ isDraft = true です。</span><span class="sxs-lookup"><span data-stu-id="bba6a-167">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="bba6a-168">isDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="bba6a-168">isDeliveryReceiptRequested</span></span>|<span data-ttu-id="bba6a-169">ブール値</span><span class="sxs-lookup"><span data-stu-id="bba6a-169">Boolean</span></span>|<span data-ttu-id="bba6a-170">メッセージの開封応答が要求されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="bba6a-170">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="bba6a-171">isRead</span><span class="sxs-lookup"><span data-stu-id="bba6a-171">isRead</span></span>|<span data-ttu-id="bba6a-172">ブール値</span><span class="sxs-lookup"><span data-stu-id="bba6a-172">Boolean</span></span>|<span data-ttu-id="bba6a-173">メッセージが開封されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="bba6a-173">Indicates whether the message has been read.</span></span>|
|<span data-ttu-id="bba6a-174">isReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="bba6a-174">isReadReceiptRequested</span></span>|<span data-ttu-id="bba6a-175">ブール値</span><span class="sxs-lookup"><span data-stu-id="bba6a-175">Boolean</span></span>|<span data-ttu-id="bba6a-176">メッセージの開封確認メッセージが要求されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="bba6a-176">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="bba6a-177">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="bba6a-177">multiValueExtendedProperties</span></span>|<span data-ttu-id="bba6a-178">[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) collection</span><span class="sxs-lookup"><span data-stu-id="bba6a-178">[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="bba6a-179">複数値のコレクションでは、メッセージに対して定義されたプロパティを拡張します。</span><span class="sxs-lookup"><span data-stu-id="bba6a-179">The collection of multi-value extended properties defined for the message.</span></span> <span data-ttu-id="bba6a-180">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="bba6a-180">Nullable.</span></span>|
|<span data-ttu-id="bba6a-181">replyTo</span><span class="sxs-lookup"><span data-stu-id="bba6a-181">replyTo</span></span>|<span data-ttu-id="bba6a-182">Recipient collection</span><span class="sxs-lookup"><span data-stu-id="bba6a-182">Recipient collection</span></span>|<span data-ttu-id="bba6a-183">返信時に使用される電子メール アドレス。</span><span class="sxs-lookup"><span data-stu-id="bba6a-183">The email addresses to use when replying.</span></span> <span data-ttu-id="bba6a-184">更新可能な場合にのみ isDraft = true です。</span><span class="sxs-lookup"><span data-stu-id="bba6a-184">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="bba6a-185">sender</span><span class="sxs-lookup"><span data-stu-id="bba6a-185">sender</span></span>|<span data-ttu-id="bba6a-186">Recipient</span><span class="sxs-lookup"><span data-stu-id="bba6a-186">Recipient</span></span>|<span data-ttu-id="bba6a-187">メッセージを生成するために実際に使用されるアカウント。</span><span class="sxs-lookup"><span data-stu-id="bba6a-187">The account that is actually used to generate the message.</span></span> <span data-ttu-id="bba6a-188">[共有されているメールボックス](https://docs.microsoft.com/en-us/exchange/collaboration/shared-mailboxes/shared-mailboxes)、または[委任](https://support.office.com/en-us/article/allow-someone-else-to-manage-your-mail-and-calendar-41c40c04-3bd1-4d22-963a-28eafec25926)としてメッセージを送信するメッセージを送信するときに更新します。</span><span class="sxs-lookup"><span data-stu-id="bba6a-188">Updatable when sending a message from a [shared mailbox](https://docs.microsoft.com/en-us/exchange/collaboration/shared-mailboxes/shared-mailboxes), or sending a message as a [delegate](https://support.office.com/en-us/article/allow-someone-else-to-manage-your-mail-and-calendar-41c40c04-3bd1-4d22-963a-28eafec25926).</span></span> <span data-ttu-id="bba6a-189">いずれの場合も、値は、使用される実際のメールボックスに対応する必要があります。</span><span class="sxs-lookup"><span data-stu-id="bba6a-189">In any case, the value must correspond to the actual mailbox used.</span></span>|
|<span data-ttu-id="bba6a-190">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="bba6a-190">singleValueExtendedProperties</span></span>|<span data-ttu-id="bba6a-191">[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) collection</span><span class="sxs-lookup"><span data-stu-id="bba6a-191">[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="bba6a-192">単一値のコレクションでは、メッセージに対して定義されたプロパティを拡張します。</span><span class="sxs-lookup"><span data-stu-id="bba6a-192">The collection of single-value extended properties defined for the message.</span></span> <span data-ttu-id="bba6a-193">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="bba6a-193">Nullable.</span></span>|
|<span data-ttu-id="bba6a-194">subject</span><span class="sxs-lookup"><span data-stu-id="bba6a-194">subject</span></span>|<span data-ttu-id="bba6a-195">String</span><span class="sxs-lookup"><span data-stu-id="bba6a-195">String</span></span>|<span data-ttu-id="bba6a-196">メッセージの件名。</span><span class="sxs-lookup"><span data-stu-id="bba6a-196">The subject of the message.</span></span> <span data-ttu-id="bba6a-197">更新可能な場合にのみ isDraft = true です。</span><span class="sxs-lookup"><span data-stu-id="bba6a-197">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="bba6a-198">toRecipients</span><span class="sxs-lookup"><span data-stu-id="bba6a-198">toRecipients</span></span>|<span data-ttu-id="bba6a-199">Recipient collection</span><span class="sxs-lookup"><span data-stu-id="bba6a-199">Recipient collection</span></span>|<span data-ttu-id="bba6a-200">宛先] の受信者のメッセージです。</span><span class="sxs-lookup"><span data-stu-id="bba6a-200">The To recipients for the message.</span></span> |

<span data-ttu-id="bba6a-201">**メッセージ** リソースは[拡張機能](/graph/extensibility-overview)をサポートしているため、`PATCH` 操作を使用して、既存の**メッセージ** インスタンスで拡張機能のカスタム プロパティにあるアプリ固有のデータを追加、更新、または削除することができます。</span><span class="sxs-lookup"><span data-stu-id="bba6a-201">Since the **message** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **message** instance.</span></span>

## <a name="response"></a><span data-ttu-id="bba6a-202">応答</span><span class="sxs-lookup"><span data-stu-id="bba6a-202">Response</span></span>

<span data-ttu-id="bba6a-203">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [message](../resources/message.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="bba6a-203">If successful, this method returns a `200 OK` response code and updated [message](../resources/message.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="bba6a-204">例</span><span class="sxs-lookup"><span data-stu-id="bba6a-204">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bba6a-205">要求</span><span class="sxs-lookup"><span data-stu-id="bba6a-205">Request</span></span>
<span data-ttu-id="bba6a-206">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="bba6a-206">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="bba6a-207">応答</span><span class="sxs-lookup"><span data-stu-id="bba6a-207">Response</span></span>
<span data-ttu-id="bba6a-p116">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="bba6a-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="bba6a-211">関連項目</span><span class="sxs-lookup"><span data-stu-id="bba6a-211">See also</span></span>

- [<span data-ttu-id="bba6a-212">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="bba6a-212">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="bba6a-213">オープン拡張機能を使用したユーザーへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="bba6a-213">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="bba6a-214">スキーマ拡張機能を使用したグループへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="bba6a-214">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update message",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
