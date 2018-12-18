---
title: メッセージを更新する
description: メッセージ オブジェクトのプロパティを更新します。
author: angelgolfer-ms
ms.openlocfilehash: b8f39dc9648203f86749ba06b88bf2f74b79d88a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27337542"
---
# <a name="update-message"></a><span data-ttu-id="28c23-103">メッセージを更新する</span><span class="sxs-lookup"><span data-stu-id="28c23-103">Update message</span></span>

<span data-ttu-id="28c23-104">メッセージ オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="28c23-104">Update the properties of message object.</span></span>
## <a name="permissions"></a><span data-ttu-id="28c23-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="28c23-105">Permissions</span></span>
<span data-ttu-id="28c23-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="28c23-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="28c23-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="28c23-108">Permission type</span></span>      | <span data-ttu-id="28c23-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="28c23-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="28c23-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="28c23-110">Delegated (work or school account)</span></span> | <span data-ttu-id="28c23-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="28c23-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="28c23-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="28c23-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="28c23-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="28c23-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="28c23-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="28c23-114">Application</span></span> | <span data-ttu-id="28c23-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="28c23-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="28c23-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="28c23-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/messages/{id}
PATCH /users/{id | userPrincipalName}/messages/{id}
PATCH /me/mailFolders/{id}/messages/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="28c23-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="28c23-117">Request headers</span></span>
| <span data-ttu-id="28c23-118">名前</span><span class="sxs-lookup"><span data-stu-id="28c23-118">Name</span></span>       | <span data-ttu-id="28c23-119">種類</span><span class="sxs-lookup"><span data-stu-id="28c23-119">Type</span></span> | <span data-ttu-id="28c23-120">説明</span><span class="sxs-lookup"><span data-stu-id="28c23-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="28c23-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="28c23-121">Authorization</span></span>  | <span data-ttu-id="28c23-122">string</span><span class="sxs-lookup"><span data-stu-id="28c23-122">string</span></span>  | <span data-ttu-id="28c23-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="28c23-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="28c23-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="28c23-125">Content-Type</span></span> | <span data-ttu-id="28c23-126">string</span><span class="sxs-lookup"><span data-stu-id="28c23-126">string</span></span>  | <span data-ttu-id="28c23-p103">エンティティ本文内のデータの性質です。必須。</span><span class="sxs-lookup"><span data-stu-id="28c23-p103">Nature of the data in the body of an entity. Required.</span></span> |
## <a name="request-body"></a><span data-ttu-id="28c23-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="28c23-129">Request body</span></span>
<span data-ttu-id="28c23-p104">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。以下のプロパティは書き込み可能または更新可能です。</span><span class="sxs-lookup"><span data-stu-id="28c23-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed. Writable/Updatable properties are</span></span>

| <span data-ttu-id="28c23-134">プロパティ</span><span class="sxs-lookup"><span data-stu-id="28c23-134">Property</span></span>     | <span data-ttu-id="28c23-135">種類</span><span class="sxs-lookup"><span data-stu-id="28c23-135">Type</span></span>   |<span data-ttu-id="28c23-136">説明</span><span class="sxs-lookup"><span data-stu-id="28c23-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="28c23-137">bccRecipients</span><span class="sxs-lookup"><span data-stu-id="28c23-137">bccRecipients</span></span>|<span data-ttu-id="28c23-138">Recipient</span><span class="sxs-lookup"><span data-stu-id="28c23-138">Recipient</span></span>|<span data-ttu-id="28c23-139">メッセージの BCC 受信者。</span><span class="sxs-lookup"><span data-stu-id="28c23-139">The Bcc recipients for the message.</span></span> <span data-ttu-id="28c23-140">更新可能な場合にのみ isDraft = true です。</span><span class="sxs-lookup"><span data-stu-id="28c23-140">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="28c23-141">categories</span><span class="sxs-lookup"><span data-stu-id="28c23-141">categories</span></span>|<span data-ttu-id="28c23-142">String コレクション</span><span class="sxs-lookup"><span data-stu-id="28c23-142">String collection</span></span>|<span data-ttu-id="28c23-143">メッセージに関連付けられたカテゴリ。</span><span class="sxs-lookup"><span data-stu-id="28c23-143">The categories associated with the message.</span></span>|
|<span data-ttu-id="28c23-144">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="28c23-144">ccRecipients</span></span>|<span data-ttu-id="28c23-145">Recipient collection</span><span class="sxs-lookup"><span data-stu-id="28c23-145">Recipient collection</span></span>|<span data-ttu-id="28c23-146">メッセージの CC 受信者。</span><span class="sxs-lookup"><span data-stu-id="28c23-146">The Cc recipients for the message.</span></span> <span data-ttu-id="28c23-147">更新可能な場合にのみ isDraft = true です。</span><span class="sxs-lookup"><span data-stu-id="28c23-147">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="28c23-148">from</span><span class="sxs-lookup"><span data-stu-id="28c23-148">from</span></span>|<span data-ttu-id="28c23-149">Recipient</span><span class="sxs-lookup"><span data-stu-id="28c23-149">Recipient</span></span>|<span data-ttu-id="28c23-150">メッセージのメールボックス所有者と送信者。</span><span class="sxs-lookup"><span data-stu-id="28c23-150">The mailbox owner and sender of the message.</span></span> <span data-ttu-id="28c23-151">更新可能な場合にのみ isDraft = true です。</span><span class="sxs-lookup"><span data-stu-id="28c23-151">Updatable only if isDraft = true.</span></span> <span data-ttu-id="28c23-152">使用される実際のメールボックスに対応する必要があります。</span><span class="sxs-lookup"><span data-stu-id="28c23-152">Must correspond to the actual mailbox used.</span></span>|
|<span data-ttu-id="28c23-153">importance</span><span class="sxs-lookup"><span data-stu-id="28c23-153">importance</span></span>|<span data-ttu-id="28c23-154">String</span><span class="sxs-lookup"><span data-stu-id="28c23-154">String</span></span>|<span data-ttu-id="28c23-155">メッセージの重要性。</span><span class="sxs-lookup"><span data-stu-id="28c23-155">The importance of the message.</span></span> <span data-ttu-id="28c23-156">可能な値: `Low`、 `Normal`、 `High`。</span><span class="sxs-lookup"><span data-stu-id="28c23-156">The possible values are: `Low`, `Normal`, `High`.</span></span>|
|<span data-ttu-id="28c23-157">inferenceClassification</span><span class="sxs-lookup"><span data-stu-id="28c23-157">inferenceClassification</span></span> | <span data-ttu-id="28c23-158">String</span><span class="sxs-lookup"><span data-stu-id="28c23-158">String</span></span> | <span data-ttu-id="28c23-159">推論の妥当性や重要度、または明示的なオーバーライドに基づいて、ユーザーに対するメッセージの分類です。</span><span class="sxs-lookup"><span data-stu-id="28c23-159">The classification of the message for the user, based on inferred relevance or importance, or on an explicit override.</span></span> <span data-ttu-id="28c23-160">可能な値:`focused`または`other`。</span><span class="sxs-lookup"><span data-stu-id="28c23-160">The possible values are: `focused` or `other`.</span></span> |
|<span data-ttu-id="28c23-161">internetMessageId</span><span class="sxs-lookup"><span data-stu-id="28c23-161">internetMessageId</span></span> |<span data-ttu-id="28c23-162">String</span><span class="sxs-lookup"><span data-stu-id="28c23-162">String</span></span> |<span data-ttu-id="28c23-163">[RFC2822](https://www.ietf.org/rfc/rfc2822.txt) によって指定された形式のメッセージ ID。</span><span class="sxs-lookup"><span data-stu-id="28c23-163">The message ID in the format specified by [RFC2822](https://www.ietf.org/rfc/rfc2822.txt).</span></span> <span data-ttu-id="28c23-164">更新可能な場合にのみ isDraft = true です。</span><span class="sxs-lookup"><span data-stu-id="28c23-164">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="28c23-165">isRead</span><span class="sxs-lookup"><span data-stu-id="28c23-165">isRead</span></span>|<span data-ttu-id="28c23-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="28c23-166">Boolean</span></span>|<span data-ttu-id="28c23-167">メッセージが読み取られたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="28c23-167">Indicates whether the message has been read.</span></span>|
|<span data-ttu-id="28c23-168">replyTo</span><span class="sxs-lookup"><span data-stu-id="28c23-168">replyTo</span></span>|<span data-ttu-id="28c23-169">Recipient collection</span><span class="sxs-lookup"><span data-stu-id="28c23-169">Recipient collection</span></span>|<span data-ttu-id="28c23-170">返信時に使用される電子メール アドレス。</span><span class="sxs-lookup"><span data-stu-id="28c23-170">The email addresses to use when replying.</span></span> <span data-ttu-id="28c23-171">更新可能な場合にのみ isDraft = true です。</span><span class="sxs-lookup"><span data-stu-id="28c23-171">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="28c23-172">sender</span><span class="sxs-lookup"><span data-stu-id="28c23-172">sender</span></span>|<span data-ttu-id="28c23-173">Recipient</span><span class="sxs-lookup"><span data-stu-id="28c23-173">Recipient</span></span>|<span data-ttu-id="28c23-174">メッセージを生成するために実際に使用されるアカウント。</span><span class="sxs-lookup"><span data-stu-id="28c23-174">The account that is actually used to generate the message.</span></span> <span data-ttu-id="28c23-175">更新可能な場合にのみ isDraft = true の場合と[共有されているメールボックス](https://docs.microsoft.com/en-us/exchange/collaboration/shared-mailboxes/shared-mailboxes)からメッセージを送信すると[デリゲート](https://support.office.com/en-us/article/allow-someone-else-to-manage-your-mail-and-calendar-41c40c04-3bd1-4d22-963a-28eafec25926)としてメッセージを送信します。</span><span class="sxs-lookup"><span data-stu-id="28c23-175">Updatable only if isDraft = true, and when sending a message from a [shared mailbox](https://docs.microsoft.com/en-us/exchange/collaboration/shared-mailboxes/shared-mailboxes), or sending a message as a [delegate](https://support.office.com/en-us/article/allow-someone-else-to-manage-your-mail-and-calendar-41c40c04-3bd1-4d22-963a-28eafec25926).</span></span> <span data-ttu-id="28c23-176">いずれの場合も、値は、使用される実際のメールボックスに対応する必要があります。</span><span class="sxs-lookup"><span data-stu-id="28c23-176">In any case, the value must correspond to the actual mailbox used.</span></span>|
|<span data-ttu-id="28c23-177">toRecipients</span><span class="sxs-lookup"><span data-stu-id="28c23-177">toRecipients</span></span>|<span data-ttu-id="28c23-178">Recipient collection</span><span class="sxs-lookup"><span data-stu-id="28c23-178">Recipient collection</span></span>|<span data-ttu-id="28c23-179">宛先] の受信者のメッセージです。</span><span class="sxs-lookup"><span data-stu-id="28c23-179">The To recipients for the message.</span></span> <span data-ttu-id="28c23-180">更新可能な場合にのみ isDraft = true です。</span><span class="sxs-lookup"><span data-stu-id="28c23-180">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="28c23-181">body</span><span class="sxs-lookup"><span data-stu-id="28c23-181">body</span></span>|<span data-ttu-id="28c23-182">ItemBody</span><span class="sxs-lookup"><span data-stu-id="28c23-182">ItemBody</span></span>|<span data-ttu-id="28c23-183">メッセージの本文。</span><span class="sxs-lookup"><span data-stu-id="28c23-183">The body of the message.</span></span> <span data-ttu-id="28c23-184">更新可能な場合にのみ isDraft = true です。</span><span class="sxs-lookup"><span data-stu-id="28c23-184">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="28c23-185">isDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="28c23-185">isDeliveryReceiptRequested</span></span>|<span data-ttu-id="28c23-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="28c23-186">Boolean</span></span>|<span data-ttu-id="28c23-187">メッセージの開封応答が要求されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="28c23-187">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="28c23-188">isReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="28c23-188">isReadReceiptRequested</span></span>|<span data-ttu-id="28c23-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="28c23-189">Boolean</span></span>|<span data-ttu-id="28c23-190">メッセージの開封応答が要求されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="28c23-190">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="28c23-191">subject</span><span class="sxs-lookup"><span data-stu-id="28c23-191">subject</span></span>|<span data-ttu-id="28c23-192">String</span><span class="sxs-lookup"><span data-stu-id="28c23-192">String</span></span>|<span data-ttu-id="28c23-193">メッセージの件名。</span><span class="sxs-lookup"><span data-stu-id="28c23-193">The subject of the message.</span></span> <span data-ttu-id="28c23-194">更新可能な場合にのみ isDraft = true です。</span><span class="sxs-lookup"><span data-stu-id="28c23-194">Updatable only if isDraft = true.</span></span>|

<span data-ttu-id="28c23-195">**メッセージ** リソースは[拡張機能](/graph/extensibility-overview)をサポートしているため、`PATCH` 操作を使用して、既存の**メッセージ** インスタンスで拡張機能のカスタム プロパティにあるアプリ固有のデータを追加、更新、または削除することができます。</span><span class="sxs-lookup"><span data-stu-id="28c23-195">Since the **message** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **message** instance.</span></span>

## <a name="response"></a><span data-ttu-id="28c23-196">応答</span><span class="sxs-lookup"><span data-stu-id="28c23-196">Response</span></span>

<span data-ttu-id="28c23-197">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [message](../resources/message.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="28c23-197">If successful, this method returns a `200 OK` response code and updated [message](../resources/message.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="28c23-198">例</span><span class="sxs-lookup"><span data-stu-id="28c23-198">Example</span></span>
##### <a name="request"></a><span data-ttu-id="28c23-199">要求</span><span class="sxs-lookup"><span data-stu-id="28c23-199">Request</span></span>
<span data-ttu-id="28c23-200">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="28c23-200">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_message"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/messages/{id}
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
##### <a name="response"></a><span data-ttu-id="28c23-201">応答</span><span class="sxs-lookup"><span data-stu-id="28c23-201">Response</span></span>
<span data-ttu-id="28c23-p116">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="28c23-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "receivedDateTime": "datetime-value",
  "sentDateTime": "datetime-value",
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

## <a name="see-also"></a><span data-ttu-id="28c23-205">関連項目</span><span class="sxs-lookup"><span data-stu-id="28c23-205">See also</span></span>

- [<span data-ttu-id="28c23-206">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="28c23-206">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="28c23-207">オープン拡張機能を使用したユーザーへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="28c23-207">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update message",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
