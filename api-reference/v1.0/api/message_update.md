# <a name="update-message"></a><span data-ttu-id="2ffa3-101">メッセージを更新する</span><span class="sxs-lookup"><span data-stu-id="2ffa3-101">Update message</span></span>

<span data-ttu-id="2ffa3-102">メッセージ オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="2ffa3-102">Update the properties of message object.</span></span>
## <a name="permissions"></a><span data-ttu-id="2ffa3-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="2ffa3-103">Permissions</span></span>
<span data-ttu-id="2ffa3-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2ffa3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="2ffa3-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2ffa3-106">Permission type</span></span>      | <span data-ttu-id="2ffa3-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="2ffa3-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2ffa3-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2ffa3-108">Delegated (work or school account)</span></span> | <span data-ttu-id="2ffa3-109">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2ffa3-109">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="2ffa3-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2ffa3-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2ffa3-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2ffa3-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="2ffa3-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2ffa3-112">Application</span></span> | <span data-ttu-id="2ffa3-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2ffa3-113">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="2ffa3-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2ffa3-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/messages/{id}
PATCH /users/{id | userPrincipalName}/messages/{id}
PATCH /me/mailFolders/{id}/messages/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="2ffa3-115">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2ffa3-115">Request headers</span></span>
| <span data-ttu-id="2ffa3-116">名前</span><span class="sxs-lookup"><span data-stu-id="2ffa3-116">Name</span></span>       | <span data-ttu-id="2ffa3-117">型</span><span class="sxs-lookup"><span data-stu-id="2ffa3-117">Type</span></span> | <span data-ttu-id="2ffa3-118">説明</span><span class="sxs-lookup"><span data-stu-id="2ffa3-118">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="2ffa3-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="2ffa3-119">Authorization</span></span>  | <span data-ttu-id="2ffa3-120">string</span><span class="sxs-lookup"><span data-stu-id="2ffa3-120">string</span></span>  | <span data-ttu-id="2ffa3-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="2ffa3-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2ffa3-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2ffa3-123">Content-Type</span></span> | <span data-ttu-id="2ffa3-124">string</span><span class="sxs-lookup"><span data-stu-id="2ffa3-124">string</span></span>  | <span data-ttu-id="2ffa3-p103">エンティティ本文内のデータの性質です。必須。</span><span class="sxs-lookup"><span data-stu-id="2ffa3-p103">Nature of the data in the body of an entity. Required.</span></span> |
## <a name="request-body"></a><span data-ttu-id="2ffa3-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="2ffa3-127">Request body</span></span>
<span data-ttu-id="2ffa3-p104">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。以下のプロパティは書き込み可能または更新可能です。</span><span class="sxs-lookup"><span data-stu-id="2ffa3-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed. Writable/Updatable properties are</span></span>

| <span data-ttu-id="2ffa3-132">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2ffa3-132">Property</span></span>     | <span data-ttu-id="2ffa3-133">型</span><span class="sxs-lookup"><span data-stu-id="2ffa3-133">Type</span></span>   |<span data-ttu-id="2ffa3-134">説明</span><span class="sxs-lookup"><span data-stu-id="2ffa3-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2ffa3-135">bccRecipients</span><span class="sxs-lookup"><span data-stu-id="2ffa3-135">bccRecipients</span></span>|<span data-ttu-id="2ffa3-136">Recipient</span><span class="sxs-lookup"><span data-stu-id="2ffa3-136">Recipient</span></span>|<span data-ttu-id="2ffa3-p105">メッセージの BCC 受信者。IsDraft = true の場合にのみ更新可能です。</span><span class="sxs-lookup"><span data-stu-id="2ffa3-p105">The Bcc recipients for the message. Updatable only if IsDraft = true.</span></span>|
|<span data-ttu-id="2ffa3-139">categories</span><span class="sxs-lookup"><span data-stu-id="2ffa3-139">categories</span></span>|<span data-ttu-id="2ffa3-140">String collection</span><span class="sxs-lookup"><span data-stu-id="2ffa3-140">String collection</span></span>|<span data-ttu-id="2ffa3-141">メッセージに関連付けられたカテゴリ。</span><span class="sxs-lookup"><span data-stu-id="2ffa3-141">The categories associated with the message.</span></span>|
|<span data-ttu-id="2ffa3-142">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="2ffa3-142">ccRecipients</span></span>|<span data-ttu-id="2ffa3-143">Recipient collection</span><span class="sxs-lookup"><span data-stu-id="2ffa3-143">Recipient collection</span></span>|<span data-ttu-id="2ffa3-p106">メッセージの Cc 受信者です。IsDraft = true の場合にのみ更新可能です。</span><span class="sxs-lookup"><span data-stu-id="2ffa3-p106">The Cc recipients for the message. Updatable only if IsDraft = true.</span></span>|
|<span data-ttu-id="2ffa3-146">from</span><span class="sxs-lookup"><span data-stu-id="2ffa3-146">from</span></span>|<span data-ttu-id="2ffa3-147">Recipient</span><span class="sxs-lookup"><span data-stu-id="2ffa3-147">Recipient</span></span>|<span data-ttu-id="2ffa3-p107">メッセージのメールボックス所有者と送信者。IsDraft = true の場合にのみ更新可能です。</span><span class="sxs-lookup"><span data-stu-id="2ffa3-p107">The mailbox owner and sender of the message. Updatable only if IsDraft = true.</span></span>|
|<span data-ttu-id="2ffa3-150">importance</span><span class="sxs-lookup"><span data-stu-id="2ffa3-150">importance</span></span>|<span data-ttu-id="2ffa3-151">String</span><span class="sxs-lookup"><span data-stu-id="2ffa3-151">String</span></span>|<span data-ttu-id="2ffa3-p108">メッセージの重要度です。可能な値は、`Low`、`Normal`、`High` です。</span><span class="sxs-lookup"><span data-stu-id="2ffa3-p108">The importance of the message. Possible values are: `Low`, `Normal`, `High`.</span></span>|
|<span data-ttu-id="2ffa3-154">inferenceClassification</span><span class="sxs-lookup"><span data-stu-id="2ffa3-154">inferenceClassification</span></span> | <span data-ttu-id="2ffa3-155">String</span><span class="sxs-lookup"><span data-stu-id="2ffa3-155">String</span></span> | <span data-ttu-id="2ffa3-p109">推定される関連性や重要性、または明示的なオーバーライドに基づく、ユーザーのメッセージの分類です。使用可能な値: `focused` または `other`。</span><span class="sxs-lookup"><span data-stu-id="2ffa3-p109">The classification of the message for the user, based on inferred relevance or importance, or on an explicit override. Possible values are: `focused` or `other`.</span></span> |
|<span data-ttu-id="2ffa3-158">internetMessageId</span><span class="sxs-lookup"><span data-stu-id="2ffa3-158">internetMessageId</span></span> |<span data-ttu-id="2ffa3-159">String</span><span class="sxs-lookup"><span data-stu-id="2ffa3-159">String</span></span> |<span data-ttu-id="2ffa3-p110">[RFC2822](http://www.ietf.org/rfc/rfc2822.txt) によって指定された形式のメッセージ ID。IsDraft = true の場合にのみ更新可能です。</span><span class="sxs-lookup"><span data-stu-id="2ffa3-p110">The message ID in the format specified by [RFC2822](http://www.ietf.org/rfc/rfc2822.txt). Updatable only if IsDraft = true.</span></span>|
|<span data-ttu-id="2ffa3-162">isRead</span><span class="sxs-lookup"><span data-stu-id="2ffa3-162">isRead</span></span>|<span data-ttu-id="2ffa3-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="2ffa3-163">Boolean</span></span>|<span data-ttu-id="2ffa3-164">メッセージが読み取られたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="2ffa3-164">Indicates whether the message has been read.</span></span>|
|<span data-ttu-id="2ffa3-165">replyTo</span><span class="sxs-lookup"><span data-stu-id="2ffa3-165">replyTo</span></span>|<span data-ttu-id="2ffa3-166">Recipient collection</span><span class="sxs-lookup"><span data-stu-id="2ffa3-166">Recipient collection</span></span>|<span data-ttu-id="2ffa3-p111">返信時に使用される電子メール アドレス。IsDraft = true の場合にのみ更新可能です。</span><span class="sxs-lookup"><span data-stu-id="2ffa3-p111">The email addresses to use when replying. Updatable only if IsDraft = true.</span></span>|
|<span data-ttu-id="2ffa3-169">sender</span><span class="sxs-lookup"><span data-stu-id="2ffa3-169">sender</span></span>|<span data-ttu-id="2ffa3-170">Recipient</span><span class="sxs-lookup"><span data-stu-id="2ffa3-170">Recipient</span></span>|<span data-ttu-id="2ffa3-p112">メッセージを生成するために実際に使用されるアカウント。IsDraft = true の場合にのみ更新可能です。</span><span class="sxs-lookup"><span data-stu-id="2ffa3-p112">The account that is actually used to generate the message. Updatable only if IsDraft = true.</span></span>|
|<span data-ttu-id="2ffa3-173">toRecipients</span><span class="sxs-lookup"><span data-stu-id="2ffa3-173">toRecipients</span></span>|<span data-ttu-id="2ffa3-174">Recipient collection</span><span class="sxs-lookup"><span data-stu-id="2ffa3-174">Recipient collection</span></span>|<span data-ttu-id="2ffa3-p113">メッセージの宛先受信者。IsDraft = true の場合にのみ更新可能です。</span><span class="sxs-lookup"><span data-stu-id="2ffa3-p113">The To recipients for the message. Updatable only if IsDraft = true.</span></span>|
|<span data-ttu-id="2ffa3-177">body</span><span class="sxs-lookup"><span data-stu-id="2ffa3-177">body</span></span>|<span data-ttu-id="2ffa3-178">ItemBody</span><span class="sxs-lookup"><span data-stu-id="2ffa3-178">ItemBody</span></span>|<span data-ttu-id="2ffa3-p114">メッセージの本文。IsDraft = true の場合にのみ更新可能です。</span><span class="sxs-lookup"><span data-stu-id="2ffa3-p114">The body of the message. Updatable only if IsDraft = true.</span></span>|
|<span data-ttu-id="2ffa3-181">isDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="2ffa3-181">isDeliveryReceiptRequested</span></span>|<span data-ttu-id="2ffa3-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="2ffa3-182">Boolean</span></span>|<span data-ttu-id="2ffa3-183">メッセージの開封応答が要求されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="2ffa3-183">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="2ffa3-184">isReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="2ffa3-184">isReadReceiptRequested</span></span>|<span data-ttu-id="2ffa3-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="2ffa3-185">Boolean</span></span>|<span data-ttu-id="2ffa3-186">メッセージの開封応答が要求されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="2ffa3-186">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="2ffa3-187">subject</span><span class="sxs-lookup"><span data-stu-id="2ffa3-187">subject</span></span>|<span data-ttu-id="2ffa3-188">String</span><span class="sxs-lookup"><span data-stu-id="2ffa3-188">String</span></span>|<span data-ttu-id="2ffa3-p115">メッセージの件名です。IsDraft = true の場合にのみ更新可能です。</span><span class="sxs-lookup"><span data-stu-id="2ffa3-p115">The subject of the message. Updatable only if IsDraft = true.</span></span>|

<span data-ttu-id="2ffa3-191">**メッセージ** リソースは[拡張機能](../../../concepts/extensibility_overview.md)をサポートしているため、`PATCH` 操作を使用して、既存の**メッセージ** インスタンスで拡張機能のカスタム プロパティにあるアプリ固有のデータを追加、更新、または削除することができます。</span><span class="sxs-lookup"><span data-stu-id="2ffa3-191">Since the **message** resource supports [extensions](../../../concepts/extensibility_overview.md), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **message** instance.</span></span>

## <a name="response"></a><span data-ttu-id="2ffa3-192">応答</span><span class="sxs-lookup"><span data-stu-id="2ffa3-192">Response</span></span>

<span data-ttu-id="2ffa3-193">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [message](../resources/message.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="2ffa3-193">If successful, this method returns a `200 OK` response code and updated [message](../resources/message.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2ffa3-194">例</span><span class="sxs-lookup"><span data-stu-id="2ffa3-194">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2ffa3-195">要求</span><span class="sxs-lookup"><span data-stu-id="2ffa3-195">Request</span></span>
<span data-ttu-id="2ffa3-196">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2ffa3-196">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="2ffa3-197">応答</span><span class="sxs-lookup"><span data-stu-id="2ffa3-197">Response</span></span>
<span data-ttu-id="2ffa3-p116">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="2ffa3-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="2ffa3-201">関連項目</span><span class="sxs-lookup"><span data-stu-id="2ffa3-201">See also</span></span>

- [<span data-ttu-id="2ffa3-202">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="2ffa3-202">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="2ffa3-203">オープン拡張機能を使用したユーザーへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="2ffa3-203">Add custom data to users using open extensions (preview)</span></span>](../../../concepts/extensibility_open_users.md)
<!--
- [Add custom data to groups using schema extensions (preview)](../../../concepts/extensibility_schema_groups.md)
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
