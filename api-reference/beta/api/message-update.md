---
title: メッセージを更新する
description: メッセージ オブジェクトのプロパティを更新します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 5a42e9d6a10e79a4ae801cca464c912dc6fade7b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515686"
---
# <a name="update-message"></a><span data-ttu-id="bff04-103">メッセージを更新する</span><span class="sxs-lookup"><span data-stu-id="bff04-103">Update message</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bff04-104">メッセージ オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="bff04-104">Update the properties of a message object.</span></span>
## <a name="permissions"></a><span data-ttu-id="bff04-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="bff04-105">Permissions</span></span>
<span data-ttu-id="bff04-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bff04-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bff04-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="bff04-108">Permission type</span></span>      | <span data-ttu-id="bff04-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="bff04-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bff04-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="bff04-110">Delegated (work or school account)</span></span> | <span data-ttu-id="bff04-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bff04-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="bff04-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="bff04-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bff04-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bff04-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="bff04-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="bff04-114">Application</span></span> | <span data-ttu-id="bff04-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bff04-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="bff04-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="bff04-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/messages/{id}
PATCH /users/{id | userPrincipalName}/messages/{id}
PATCH /me/mailFolders/{id}/messages/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="bff04-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bff04-117">Request headers</span></span>
| <span data-ttu-id="bff04-118">名前</span><span class="sxs-lookup"><span data-stu-id="bff04-118">Name</span></span>       | <span data-ttu-id="bff04-119">型</span><span class="sxs-lookup"><span data-stu-id="bff04-119">Type</span></span> | <span data-ttu-id="bff04-120">説明</span><span class="sxs-lookup"><span data-stu-id="bff04-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="bff04-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="bff04-121">Authorization</span></span>  | <span data-ttu-id="bff04-122">string</span><span class="sxs-lookup"><span data-stu-id="bff04-122">string</span></span>  | <span data-ttu-id="bff04-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="bff04-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="bff04-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bff04-125">Content-Type</span></span> | <span data-ttu-id="bff04-126">string</span><span class="sxs-lookup"><span data-stu-id="bff04-126">string</span></span>  | <span data-ttu-id="bff04-p103">エンティティ本文内のデータの性質です。必須。</span><span class="sxs-lookup"><span data-stu-id="bff04-p103">Nature of the data in the body of an entity. Required.</span></span> |
## <a name="request-body"></a><span data-ttu-id="bff04-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="bff04-129">Request body</span></span>
<span data-ttu-id="bff04-130">要求本文で、更新する関連フィールドの値を指定します。</span><span class="sxs-lookup"><span data-stu-id="bff04-130">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="bff04-131">要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変更に基づいて再計算されます。</span><span class="sxs-lookup"><span data-stu-id="bff04-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="bff04-132">最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="bff04-132">For best performance you shouldn't include existing values that haven't changed.</span></span> <span data-ttu-id="bff04-133">次のプロパティを更新することができます。</span><span class="sxs-lookup"><span data-stu-id="bff04-133">The following properties can be updated.</span></span>

| <span data-ttu-id="bff04-134">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bff04-134">Property</span></span>     | <span data-ttu-id="bff04-135">型</span><span class="sxs-lookup"><span data-stu-id="bff04-135">Type</span></span>   |<span data-ttu-id="bff04-136">説明</span><span class="sxs-lookup"><span data-stu-id="bff04-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bff04-137">bccRecipients</span><span class="sxs-lookup"><span data-stu-id="bff04-137">bccRecipients</span></span>|<span data-ttu-id="bff04-138">Recipient</span><span class="sxs-lookup"><span data-stu-id="bff04-138">Recipient</span></span>|<span data-ttu-id="bff04-139">メッセージの BCC 受信者。</span><span class="sxs-lookup"><span data-stu-id="bff04-139">The Bcc recipients for the message.</span></span> |
|<span data-ttu-id="bff04-140">body</span><span class="sxs-lookup"><span data-stu-id="bff04-140">body</span></span>|<span data-ttu-id="bff04-141">ItemBody</span><span class="sxs-lookup"><span data-stu-id="bff04-141">ItemBody</span></span>|<span data-ttu-id="bff04-p105">メッセージの本文。IsDraft = true の場合にのみ更新可能です。</span><span class="sxs-lookup"><span data-stu-id="bff04-p105">The body of the message. Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="bff04-144">categories</span><span class="sxs-lookup"><span data-stu-id="bff04-144">categories</span></span>|<span data-ttu-id="bff04-145">String コレクション</span><span class="sxs-lookup"><span data-stu-id="bff04-145">String collection</span></span>|<span data-ttu-id="bff04-146">メッセージに関連付けられたカテゴリ。</span><span class="sxs-lookup"><span data-stu-id="bff04-146">The categories associated with the message.</span></span>|
|<span data-ttu-id="bff04-147">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="bff04-147">ccRecipients</span></span>|<span data-ttu-id="bff04-148">Recipient collection</span><span class="sxs-lookup"><span data-stu-id="bff04-148">Recipient collection</span></span>|<span data-ttu-id="bff04-149">メッセージの CC 受信者。</span><span class="sxs-lookup"><span data-stu-id="bff04-149">The Cc recipients for the message.</span></span> |
|<span data-ttu-id="bff04-150">from</span><span class="sxs-lookup"><span data-stu-id="bff04-150">from</span></span>|<span data-ttu-id="bff04-151">Recipient</span><span class="sxs-lookup"><span data-stu-id="bff04-151">Recipient</span></span>|<span data-ttu-id="bff04-152">メッセージのメールボックス所有者と送信者。</span><span class="sxs-lookup"><span data-stu-id="bff04-152">The mailbox owner and sender of the message.</span></span> <span data-ttu-id="bff04-153">使用される実際のメールボックスに対応する必要があります。</span><span class="sxs-lookup"><span data-stu-id="bff04-153">Must correspond to the actual mailbox used.</span></span> |
|<span data-ttu-id="bff04-154">importance</span><span class="sxs-lookup"><span data-stu-id="bff04-154">importance</span></span>|<span data-ttu-id="bff04-155">String</span><span class="sxs-lookup"><span data-stu-id="bff04-155">String</span></span>|<span data-ttu-id="bff04-p107">メッセージの重要度です。可能な値は、`Low`、`Normal`、`High` です。</span><span class="sxs-lookup"><span data-stu-id="bff04-p107">The importance of the message. Possible values are: `Low`, `Normal`, `High`.</span></span>|
|<span data-ttu-id="bff04-158">inferenceClassification</span><span class="sxs-lookup"><span data-stu-id="bff04-158">inferenceClassification</span></span> | <span data-ttu-id="bff04-159">String</span><span class="sxs-lookup"><span data-stu-id="bff04-159">String</span></span> | <span data-ttu-id="bff04-p108">推定される関連性や重要性、または明示的なオーバーライドに基づく、ユーザーのメッセージの分類です。使用可能な値: `focused` または `other`。</span><span class="sxs-lookup"><span data-stu-id="bff04-p108">The classification of the message for the user, based on inferred relevance or importance, or on an explicit override. Possible values are: `focused` or `other`.</span></span> |
|<span data-ttu-id="bff04-162">internetMessageId</span><span class="sxs-lookup"><span data-stu-id="bff04-162">internetMessageId</span></span> |<span data-ttu-id="bff04-163">String</span><span class="sxs-lookup"><span data-stu-id="bff04-163">String</span></span> |<span data-ttu-id="bff04-p109">[RFC2822](https://www.ietf.org/rfc/rfc2822.txt) によって指定された形式のメッセージ ID。IsDraft = true の場合にのみ更新可能です。</span><span class="sxs-lookup"><span data-stu-id="bff04-p109">The message ID in the format specified by [RFC2822](https://www.ietf.org/rfc/rfc2822.txt). Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="bff04-166">isDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="bff04-166">isDeliveryReceiptRequested</span></span>|<span data-ttu-id="bff04-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="bff04-167">Boolean</span></span>|<span data-ttu-id="bff04-168">メッセージの開封応答が要求されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="bff04-168">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="bff04-169">isRead</span><span class="sxs-lookup"><span data-stu-id="bff04-169">isRead</span></span>|<span data-ttu-id="bff04-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="bff04-170">Boolean</span></span>|<span data-ttu-id="bff04-171">メッセージが開封されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="bff04-171">Indicates whether the message has been read.</span></span>|
|<span data-ttu-id="bff04-172">isReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="bff04-172">isReadReceiptRequested</span></span>|<span data-ttu-id="bff04-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="bff04-173">Boolean</span></span>|<span data-ttu-id="bff04-174">メッセージの開封確認メッセージが要求されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="bff04-174">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="bff04-175">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="bff04-175">multiValueExtendedProperties</span></span>|<span data-ttu-id="bff04-176">[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) collection</span><span class="sxs-lookup"><span data-stu-id="bff04-176">[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="bff04-177">複数値のコレクションでは、メッセージに対して定義されたプロパティを拡張します。</span><span class="sxs-lookup"><span data-stu-id="bff04-177">The collection of multi-value extended properties defined for the message.</span></span> <span data-ttu-id="bff04-178">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="bff04-178">Nullable.</span></span>|
|<span data-ttu-id="bff04-179">replyTo</span><span class="sxs-lookup"><span data-stu-id="bff04-179">replyTo</span></span>|<span data-ttu-id="bff04-180">Recipient collection</span><span class="sxs-lookup"><span data-stu-id="bff04-180">Recipient collection</span></span>|<span data-ttu-id="bff04-181">返信時に使用される電子メール アドレス。</span><span class="sxs-lookup"><span data-stu-id="bff04-181">The email addresses to use when replying.</span></span> <span data-ttu-id="bff04-182">更新可能な場合にのみ isDraft = true です。</span><span class="sxs-lookup"><span data-stu-id="bff04-182">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="bff04-183">sender</span><span class="sxs-lookup"><span data-stu-id="bff04-183">sender</span></span>|<span data-ttu-id="bff04-184">Recipient</span><span class="sxs-lookup"><span data-stu-id="bff04-184">Recipient</span></span>|<span data-ttu-id="bff04-185">メッセージを生成するために実際に使用されるアカウント。</span><span class="sxs-lookup"><span data-stu-id="bff04-185">The account that is actually used to generate the message.</span></span> <span data-ttu-id="bff04-186">[共有されているメールボックス](https://docs.microsoft.com/en-us/exchange/collaboration/shared-mailboxes/shared-mailboxes)、または[委任](https://support.office.com/en-us/article/allow-someone-else-to-manage-your-mail-and-calendar-41c40c04-3bd1-4d22-963a-28eafec25926)としてメッセージを送信するメッセージを送信するときに更新します。</span><span class="sxs-lookup"><span data-stu-id="bff04-186">Updatable when sending a message from a [shared mailbox](https://docs.microsoft.com/en-us/exchange/collaboration/shared-mailboxes/shared-mailboxes), or sending a message as a [delegate](https://support.office.com/en-us/article/allow-someone-else-to-manage-your-mail-and-calendar-41c40c04-3bd1-4d22-963a-28eafec25926).</span></span> <span data-ttu-id="bff04-187">いずれの場合も、値は、使用される実際のメールボックスに対応する必要があります。</span><span class="sxs-lookup"><span data-stu-id="bff04-187">In any case, the value must correspond to the actual mailbox used.</span></span>|
|<span data-ttu-id="bff04-188">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="bff04-188">singleValueExtendedProperties</span></span>|<span data-ttu-id="bff04-189">[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) collection</span><span class="sxs-lookup"><span data-stu-id="bff04-189">[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="bff04-190">単一値のコレクションでは、メッセージに対して定義されたプロパティを拡張します。</span><span class="sxs-lookup"><span data-stu-id="bff04-190">The collection of single-value extended properties defined for the message.</span></span> <span data-ttu-id="bff04-191">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="bff04-191">Nullable.</span></span>|
|<span data-ttu-id="bff04-192">subject</span><span class="sxs-lookup"><span data-stu-id="bff04-192">subject</span></span>|<span data-ttu-id="bff04-193">String</span><span class="sxs-lookup"><span data-stu-id="bff04-193">String</span></span>|<span data-ttu-id="bff04-p114">メッセージの件名です。IsDraft = true の場合にのみ更新可能です。</span><span class="sxs-lookup"><span data-stu-id="bff04-p114">The subject of the message. Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="bff04-196">toRecipients</span><span class="sxs-lookup"><span data-stu-id="bff04-196">toRecipients</span></span>|<span data-ttu-id="bff04-197">Recipient collection</span><span class="sxs-lookup"><span data-stu-id="bff04-197">Recipient collection</span></span>|<span data-ttu-id="bff04-198">メッセージの宛先。</span><span class="sxs-lookup"><span data-stu-id="bff04-198">The To recipients for the message.</span></span> |

<span data-ttu-id="bff04-199">**メッセージ** リソースは[拡張機能](/graph/extensibility-overview)をサポートしているため、`PATCH` 操作を使用して、既存の**メッセージ** インスタンスで拡張機能のカスタム プロパティにあるアプリ固有のデータを追加、更新、または削除することができます。</span><span class="sxs-lookup"><span data-stu-id="bff04-199">Since the **message** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **message** instance.</span></span>

## <a name="response"></a><span data-ttu-id="bff04-200">応答</span><span class="sxs-lookup"><span data-stu-id="bff04-200">Response</span></span>

<span data-ttu-id="bff04-201">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [message](../resources/message.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="bff04-201">If successful, this method returns a `200 OK` response code and updated [message](../resources/message.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="bff04-202">例</span><span class="sxs-lookup"><span data-stu-id="bff04-202">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bff04-203">要求</span><span class="sxs-lookup"><span data-stu-id="bff04-203">Request</span></span>
<span data-ttu-id="bff04-204">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="bff04-204">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="bff04-205">応答</span><span class="sxs-lookup"><span data-stu-id="bff04-205">Response</span></span>
<span data-ttu-id="bff04-p115">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="bff04-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="bff04-209">関連項目</span><span class="sxs-lookup"><span data-stu-id="bff04-209">See also</span></span>

- [<span data-ttu-id="bff04-210">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="bff04-210">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="bff04-211">オープン拡張機能を使用したユーザーへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="bff04-211">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- <span data-ttu-id="bff04-212">スキーマ拡張機能を使用したグループへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="bff04-212">[Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)</span></span>

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
