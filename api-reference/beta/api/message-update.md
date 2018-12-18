---
title: メッセージを更新する
description: メッセージ オブジェクトのプロパティを更新します。
author: angelgolfer-ms
ms.openlocfilehash: 9c717e913c641b6dffd582252538965961369a7f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27321477"
---
# <a name="update-message"></a><span data-ttu-id="de24f-103">メッセージを更新する</span><span class="sxs-lookup"><span data-stu-id="de24f-103">Update message</span></span>

> <span data-ttu-id="de24f-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="de24f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="de24f-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="de24f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="de24f-106">メッセージ オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="de24f-106">Update the properties of message object.</span></span>
## <a name="permissions"></a><span data-ttu-id="de24f-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="de24f-107">Permissions</span></span>
<span data-ttu-id="de24f-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="de24f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="de24f-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="de24f-110">Permission type</span></span>      | <span data-ttu-id="de24f-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="de24f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="de24f-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="de24f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="de24f-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="de24f-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="de24f-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="de24f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="de24f-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="de24f-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="de24f-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="de24f-116">Application</span></span> | <span data-ttu-id="de24f-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="de24f-117">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="de24f-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="de24f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/messages/{id}
PATCH /users/{id | userPrincipalName}/messages/{id}
PATCH /me/mailFolders/{id}/messages/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="de24f-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="de24f-119">Request headers</span></span>
| <span data-ttu-id="de24f-120">名前</span><span class="sxs-lookup"><span data-stu-id="de24f-120">Name</span></span>       | <span data-ttu-id="de24f-121">種類</span><span class="sxs-lookup"><span data-stu-id="de24f-121">Type</span></span> | <span data-ttu-id="de24f-122">説明</span><span class="sxs-lookup"><span data-stu-id="de24f-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="de24f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="de24f-123">Authorization</span></span>  | <span data-ttu-id="de24f-124">string</span><span class="sxs-lookup"><span data-stu-id="de24f-124">string</span></span>  | <span data-ttu-id="de24f-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="de24f-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="de24f-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="de24f-127">Content-Type</span></span> | <span data-ttu-id="de24f-128">string</span><span class="sxs-lookup"><span data-stu-id="de24f-128">string</span></span>  | <span data-ttu-id="de24f-p104">エンティティ本文内のデータの性質です。必須。</span><span class="sxs-lookup"><span data-stu-id="de24f-p104">Nature of the data in the body of an entity. Required.</span></span> |
## <a name="request-body"></a><span data-ttu-id="de24f-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="de24f-131">Request body</span></span>
<span data-ttu-id="de24f-p105">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。以下のプロパティは書き込み可能または更新可能です。</span><span class="sxs-lookup"><span data-stu-id="de24f-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed. Writable/Updatable properties are</span></span>

| <span data-ttu-id="de24f-136">プロパティ</span><span class="sxs-lookup"><span data-stu-id="de24f-136">Property</span></span>     | <span data-ttu-id="de24f-137">種類</span><span class="sxs-lookup"><span data-stu-id="de24f-137">Type</span></span>   |<span data-ttu-id="de24f-138">説明</span><span class="sxs-lookup"><span data-stu-id="de24f-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="de24f-139">bccRecipients</span><span class="sxs-lookup"><span data-stu-id="de24f-139">bccRecipients</span></span>|<span data-ttu-id="de24f-140">Recipient</span><span class="sxs-lookup"><span data-stu-id="de24f-140">Recipient</span></span>|<span data-ttu-id="de24f-141">メッセージの BCC 受信者。</span><span class="sxs-lookup"><span data-stu-id="de24f-141">The Bcc recipients for the message.</span></span> <span data-ttu-id="de24f-142">更新可能な場合にのみ isDraft = true です。</span><span class="sxs-lookup"><span data-stu-id="de24f-142">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="de24f-143">categories</span><span class="sxs-lookup"><span data-stu-id="de24f-143">categories</span></span>|<span data-ttu-id="de24f-144">String コレクション</span><span class="sxs-lookup"><span data-stu-id="de24f-144">String collection</span></span>|<span data-ttu-id="de24f-145">メッセージに関連付けられたカテゴリ。</span><span class="sxs-lookup"><span data-stu-id="de24f-145">The categories associated with the message.</span></span>|
|<span data-ttu-id="de24f-146">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="de24f-146">ccRecipients</span></span>|<span data-ttu-id="de24f-147">Recipient collection</span><span class="sxs-lookup"><span data-stu-id="de24f-147">Recipient collection</span></span>|<span data-ttu-id="de24f-148">メッセージの CC 受信者。</span><span class="sxs-lookup"><span data-stu-id="de24f-148">The Cc recipients for the message.</span></span> <span data-ttu-id="de24f-149">更新可能な場合にのみ isDraft = true です。</span><span class="sxs-lookup"><span data-stu-id="de24f-149">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="de24f-150">from</span><span class="sxs-lookup"><span data-stu-id="de24f-150">from</span></span>|<span data-ttu-id="de24f-151">Recipient</span><span class="sxs-lookup"><span data-stu-id="de24f-151">Recipient</span></span>|<span data-ttu-id="de24f-152">メッセージのメールボックス所有者と送信者。</span><span class="sxs-lookup"><span data-stu-id="de24f-152">The mailbox owner and sender of the message.</span></span> <span data-ttu-id="de24f-153">更新可能な場合にのみ isDraft = true です。</span><span class="sxs-lookup"><span data-stu-id="de24f-153">Updatable only if isDraft = true.</span></span> <span data-ttu-id="de24f-154">使用される実際のメールボックスに対応する必要があります。</span><span class="sxs-lookup"><span data-stu-id="de24f-154">Must correspond to the actual mailbox used.</span></span> |
|<span data-ttu-id="de24f-155">importance</span><span class="sxs-lookup"><span data-stu-id="de24f-155">importance</span></span>|<span data-ttu-id="de24f-156">String</span><span class="sxs-lookup"><span data-stu-id="de24f-156">String</span></span>|<span data-ttu-id="de24f-p109">メッセージの重要度です。可能な値は、`Low`、`Normal`、`High` です。</span><span class="sxs-lookup"><span data-stu-id="de24f-p109">The importance of the message. Possible values are: `Low`, `Normal`, `High`.</span></span>|
|<span data-ttu-id="de24f-159">inferenceClassification</span><span class="sxs-lookup"><span data-stu-id="de24f-159">inferenceClassification</span></span> | <span data-ttu-id="de24f-160">String</span><span class="sxs-lookup"><span data-stu-id="de24f-160">String</span></span> | <span data-ttu-id="de24f-p110">推定される関連性や重要性、または明示的なオーバーライドに基づく、ユーザーのメッセージの分類です。使用可能な値: `focused` または `other`。</span><span class="sxs-lookup"><span data-stu-id="de24f-p110">The classification of the message for the user, based on inferred relevance or importance, or on an explicit override. Possible values are: `focused` or `other`.</span></span> |
|<span data-ttu-id="de24f-163">internetMessageId</span><span class="sxs-lookup"><span data-stu-id="de24f-163">internetMessageId</span></span> |<span data-ttu-id="de24f-164">String</span><span class="sxs-lookup"><span data-stu-id="de24f-164">String</span></span> |<span data-ttu-id="de24f-165">[RFC2822](https://www.ietf.org/rfc/rfc2822.txt) によって指定された形式のメッセージ ID。</span><span class="sxs-lookup"><span data-stu-id="de24f-165">The message ID in the format specified by [RFC2822](https://www.ietf.org/rfc/rfc2822.txt).</span></span> <span data-ttu-id="de24f-166">更新可能な場合にのみ isDraft = true です。</span><span class="sxs-lookup"><span data-stu-id="de24f-166">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="de24f-167">isRead</span><span class="sxs-lookup"><span data-stu-id="de24f-167">isRead</span></span>|<span data-ttu-id="de24f-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="de24f-168">Boolean</span></span>|<span data-ttu-id="de24f-169">メッセージが読み取られたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="de24f-169">Indicates whether the message has been read.</span></span>|
|<span data-ttu-id="de24f-170">replyTo</span><span class="sxs-lookup"><span data-stu-id="de24f-170">replyTo</span></span>|<span data-ttu-id="de24f-171">Recipient collection</span><span class="sxs-lookup"><span data-stu-id="de24f-171">Recipient collection</span></span>|<span data-ttu-id="de24f-172">返信時に使用される電子メール アドレス。</span><span class="sxs-lookup"><span data-stu-id="de24f-172">The email addresses to use when replying.</span></span> <span data-ttu-id="de24f-173">更新可能な場合にのみ isDraft = true です。</span><span class="sxs-lookup"><span data-stu-id="de24f-173">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="de24f-174">sender</span><span class="sxs-lookup"><span data-stu-id="de24f-174">sender</span></span>|<span data-ttu-id="de24f-175">Recipient</span><span class="sxs-lookup"><span data-stu-id="de24f-175">Recipient</span></span>|<span data-ttu-id="de24f-176">メッセージを生成するために実際に使用されるアカウント。</span><span class="sxs-lookup"><span data-stu-id="de24f-176">The account that is actually used to generate the message.</span></span> <span data-ttu-id="de24f-177">更新可能な場合にのみ isDraft = true の場合と[共有されているメールボックス](https://docs.microsoft.com/en-us/exchange/collaboration/shared-mailboxes/shared-mailboxes)からメッセージを送信すると[デリゲート](https://support.office.com/en-us/article/allow-someone-else-to-manage-your-mail-and-calendar-41c40c04-3bd1-4d22-963a-28eafec25926)としてメッセージを送信します。</span><span class="sxs-lookup"><span data-stu-id="de24f-177">Updatable only if isDraft = true, and when sending a message from a [shared mailbox](https://docs.microsoft.com/en-us/exchange/collaboration/shared-mailboxes/shared-mailboxes), or sending a message as a [delegate](https://support.office.com/en-us/article/allow-someone-else-to-manage-your-mail-and-calendar-41c40c04-3bd1-4d22-963a-28eafec25926).</span></span> <span data-ttu-id="de24f-178">いずれの場合も、値は、使用される実際のメールボックスに対応する必要があります。</span><span class="sxs-lookup"><span data-stu-id="de24f-178">In any case, the value must correspond to the actual mailbox used.</span></span>|
|<span data-ttu-id="de24f-179">toRecipients</span><span class="sxs-lookup"><span data-stu-id="de24f-179">toRecipients</span></span>|<span data-ttu-id="de24f-180">Recipient collection</span><span class="sxs-lookup"><span data-stu-id="de24f-180">Recipient collection</span></span>|<span data-ttu-id="de24f-181">宛先] の受信者のメッセージです。</span><span class="sxs-lookup"><span data-stu-id="de24f-181">The To recipients for the message.</span></span> <span data-ttu-id="de24f-182">更新可能な場合にのみ isDraft = true です。</span><span class="sxs-lookup"><span data-stu-id="de24f-182">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="de24f-183">body</span><span class="sxs-lookup"><span data-stu-id="de24f-183">body</span></span>|<span data-ttu-id="de24f-184">ItemBody</span><span class="sxs-lookup"><span data-stu-id="de24f-184">ItemBody</span></span>|<span data-ttu-id="de24f-185">メッセージの本文。</span><span class="sxs-lookup"><span data-stu-id="de24f-185">The body of the message.</span></span> <span data-ttu-id="de24f-186">更新可能な場合にのみ isDraft = true です。</span><span class="sxs-lookup"><span data-stu-id="de24f-186">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="de24f-187">isDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="de24f-187">isDeliveryReceiptRequested</span></span>|<span data-ttu-id="de24f-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="de24f-188">Boolean</span></span>|<span data-ttu-id="de24f-189">メッセージの開封応答が要求されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="de24f-189">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="de24f-190">isReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="de24f-190">isReadReceiptRequested</span></span>|<span data-ttu-id="de24f-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="de24f-191">Boolean</span></span>|<span data-ttu-id="de24f-192">メッセージの開封応答が要求されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="de24f-192">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="de24f-193">subject</span><span class="sxs-lookup"><span data-stu-id="de24f-193">subject</span></span>|<span data-ttu-id="de24f-194">String</span><span class="sxs-lookup"><span data-stu-id="de24f-194">String</span></span>|<span data-ttu-id="de24f-195">メッセージの件名。</span><span class="sxs-lookup"><span data-stu-id="de24f-195">The subject of the message.</span></span> <span data-ttu-id="de24f-196">更新可能な場合にのみ isDraft = true です。</span><span class="sxs-lookup"><span data-stu-id="de24f-196">Updatable only if isDraft = true.</span></span>|

<span data-ttu-id="de24f-197">**メッセージ** リソースは[拡張機能](/graph/extensibility-overview)をサポートしているため、`PATCH` 操作を使用して、既存の**メッセージ** インスタンスで拡張機能のカスタム プロパティにあるアプリ固有のデータを追加、更新、または削除することができます。</span><span class="sxs-lookup"><span data-stu-id="de24f-197">Since the **message** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **message** instance.</span></span>

## <a name="response"></a><span data-ttu-id="de24f-198">応答</span><span class="sxs-lookup"><span data-stu-id="de24f-198">Response</span></span>

<span data-ttu-id="de24f-199">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [message](../resources/message.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="de24f-199">If successful, this method returns a `200 OK` response code and updated [message](../resources/message.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="de24f-200">例</span><span class="sxs-lookup"><span data-stu-id="de24f-200">Example</span></span>
##### <a name="request"></a><span data-ttu-id="de24f-201">要求</span><span class="sxs-lookup"><span data-stu-id="de24f-201">Request</span></span>
<span data-ttu-id="de24f-202">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="de24f-202">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="de24f-203">応答</span><span class="sxs-lookup"><span data-stu-id="de24f-203">Response</span></span>
<span data-ttu-id="de24f-p117">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="de24f-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="de24f-207">関連項目</span><span class="sxs-lookup"><span data-stu-id="de24f-207">See also</span></span>

- [<span data-ttu-id="de24f-208">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="de24f-208">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="de24f-209">オープン拡張機能を使用したユーザーへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="de24f-209">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="de24f-210">スキーマ拡張機能を使用したグループへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="de24f-210">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update message",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
