# <a name="update-message"></a><span data-ttu-id="db3d0-101">メッセージを更新する</span><span class="sxs-lookup"><span data-stu-id="db3d0-101">Update message</span></span>

<span data-ttu-id="db3d0-102">メッセージ オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="db3d0-102">Update the properties of message object.</span></span>
## <a name="permissions"></a><span data-ttu-id="db3d0-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="db3d0-103">Permissions</span></span>
<span data-ttu-id="db3d0-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="db3d0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="db3d0-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="db3d0-106">Permission type</span></span>      | <span data-ttu-id="db3d0-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="db3d0-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="db3d0-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="db3d0-108">Delegated (work or school account)</span></span> | <span data-ttu-id="db3d0-109">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="db3d0-109">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="db3d0-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="db3d0-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="db3d0-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="db3d0-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="db3d0-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="db3d0-112">Application</span></span> | <span data-ttu-id="db3d0-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="db3d0-113">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="db3d0-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="db3d0-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/messages/{id}
PATCH /users/{id | userPrincipalName}/messages/{id}
PATCH /me/mailFolders/{id}/messages/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="db3d0-115">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="db3d0-115">Request headers</span></span>
| <span data-ttu-id="db3d0-116">名前</span><span class="sxs-lookup"><span data-stu-id="db3d0-116">Name</span></span>       | <span data-ttu-id="db3d0-117">型</span><span class="sxs-lookup"><span data-stu-id="db3d0-117">Type</span></span> | <span data-ttu-id="db3d0-118">説明</span><span class="sxs-lookup"><span data-stu-id="db3d0-118">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="db3d0-119">承認</span><span class="sxs-lookup"><span data-stu-id="db3d0-119">Authorization</span></span>  | <span data-ttu-id="db3d0-120">文字列</span><span class="sxs-lookup"><span data-stu-id="db3d0-120">string</span></span>  | <span data-ttu-id="db3d0-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="db3d0-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="db3d0-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="db3d0-123">Content-Type</span></span> | <span data-ttu-id="db3d0-124">文字列</span><span class="sxs-lookup"><span data-stu-id="db3d0-124">string</span></span>  | <span data-ttu-id="db3d0-p103">エンティティ本文内のデータの性質です。必須。</span><span class="sxs-lookup"><span data-stu-id="db3d0-p103">Nature of the data in the body of an entity. Required.</span></span> |
## <a name="request-body"></a><span data-ttu-id="db3d0-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="db3d0-127">Request body</span></span>
<span data-ttu-id="db3d0-p104">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。以下のプロパティは書き込み可能または更新可能です。</span><span class="sxs-lookup"><span data-stu-id="db3d0-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed. Writable/Updatable properties are</span></span>

| <span data-ttu-id="db3d0-132">プロパティ</span><span class="sxs-lookup"><span data-stu-id="db3d0-132">Property</span></span>     | <span data-ttu-id="db3d0-133">タイプ</span><span class="sxs-lookup"><span data-stu-id="db3d0-133">Type</span></span>   |<span data-ttu-id="db3d0-134">説明</span><span class="sxs-lookup"><span data-stu-id="db3d0-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="db3d0-135">bccRecipients</span><span class="sxs-lookup"><span data-stu-id="db3d0-135">bccRecipients</span></span>|<span data-ttu-id="db3d0-136">Recipient</span><span class="sxs-lookup"><span data-stu-id="db3d0-136">Recipient</span></span>|<span data-ttu-id="db3d0-137">メッセージの BCC 受信者。</span><span class="sxs-lookup"><span data-stu-id="db3d0-137">The Bcc recipients for the message.</span></span> <span data-ttu-id="db3d0-138">isDraft = trueの場合にのみ更新可能です。</span><span class="sxs-lookup"><span data-stu-id="db3d0-138">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="db3d0-139">categories</span><span class="sxs-lookup"><span data-stu-id="db3d0-139">categories</span></span>|<span data-ttu-id="db3d0-140">String コレクション</span><span class="sxs-lookup"><span data-stu-id="db3d0-140">String collection</span></span>|<span data-ttu-id="db3d0-141">メッセージに関連付けられたカテゴリ。</span><span class="sxs-lookup"><span data-stu-id="db3d0-141">The categories associated with the message.</span></span>|
|<span data-ttu-id="db3d0-142">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="db3d0-142">ccRecipients</span></span>|<span data-ttu-id="db3d0-143">Recipient collection</span><span class="sxs-lookup"><span data-stu-id="db3d0-143">Recipient collection</span></span>|<span data-ttu-id="db3d0-144">メッセージの CC 受信者。</span><span class="sxs-lookup"><span data-stu-id="db3d0-144">The Cc recipients for the message.</span></span> <span data-ttu-id="db3d0-145">isDraft = trueの場合にのみ更新可能です。</span><span class="sxs-lookup"><span data-stu-id="db3d0-145">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="db3d0-146">from</span><span class="sxs-lookup"><span data-stu-id="db3d0-146">from</span></span>|<span data-ttu-id="db3d0-147">Recipient</span><span class="sxs-lookup"><span data-stu-id="db3d0-147">Recipient</span></span>|<span data-ttu-id="db3d0-148">メッセージのメールボックス所有者と送信者。</span><span class="sxs-lookup"><span data-stu-id="db3d0-148">The mailbox owner and sender of the message.</span></span> <span data-ttu-id="db3d0-149">isDraft = trueの場合にのみ更新可能です。</span><span class="sxs-lookup"><span data-stu-id="db3d0-149">Updatable only if isDraft = true.</span></span> <span data-ttu-id="db3d0-150">値は、使用される実際のメールボックスに対応する必要があります。</span><span class="sxs-lookup"><span data-stu-id="db3d0-150">Must correspond to the actual mailbox used.</span></span>|
|<span data-ttu-id="db3d0-151">importance</span><span class="sxs-lookup"><span data-stu-id="db3d0-151">importance</span></span>|<span data-ttu-id="db3d0-152">文字列</span><span class="sxs-lookup"><span data-stu-id="db3d0-152">String</span></span>|<span data-ttu-id="db3d0-153">メッセージの重要度。</span><span class="sxs-lookup"><span data-stu-id="db3d0-153">The importance of the message: , , .</span></span> <span data-ttu-id="db3d0-154">使用可能な値: `Low`、`Normal`、`High`。</span><span class="sxs-lookup"><span data-stu-id="db3d0-154">The possible values are `Low`, `Normal`, or `High`.</span></span>|
|<span data-ttu-id="db3d0-155">inferenceClassification</span><span class="sxs-lookup"><span data-stu-id="db3d0-155">inferenceClassification</span></span> | <span data-ttu-id="db3d0-156">文字列</span><span class="sxs-lookup"><span data-stu-id="db3d0-156">String</span></span> | <span data-ttu-id="db3d0-157">推定される関連性や重要性、または明示的なオーバーライドに基づく、ユーザーの対象メッセージの分類。</span><span class="sxs-lookup"><span data-stu-id="db3d0-157">The classification of this message for the user, based on inferred relevance or importance, or on an explicit override.</span></span> <span data-ttu-id="db3d0-158">使用可能な値: `focused` または `other`。</span><span class="sxs-lookup"><span data-stu-id="db3d0-158">The possible values are `focused`, , or `other`.</span></span> |
|<span data-ttu-id="db3d0-159">internetMessageId</span><span class="sxs-lookup"><span data-stu-id="db3d0-159">internetMessageId</span></span> |<span data-ttu-id="db3d0-160">文字列</span><span class="sxs-lookup"><span data-stu-id="db3d0-160">String</span></span> |<span data-ttu-id="db3d0-161">[RFC2822](http://www.ietf.org/rfc/rfc2822.txt) によって指定された形式のメッセージ ID。</span><span class="sxs-lookup"><span data-stu-id="db3d0-161">The message ID in the format specified by [RFC2822](http://www.ietf.org/rfc/rfc2822.txt).</span></span> <span data-ttu-id="db3d0-162">isDraft = trueの場合にのみ更新可能です。</span><span class="sxs-lookup"><span data-stu-id="db3d0-162">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="db3d0-163">isRead</span><span class="sxs-lookup"><span data-stu-id="db3d0-163">isRead</span></span>|<span data-ttu-id="db3d0-164">ブーリアン</span><span class="sxs-lookup"><span data-stu-id="db3d0-164">Boolean</span></span>|<span data-ttu-id="db3d0-165">メッセージが読み取られたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="db3d0-165">Indicates whether the message has been read.</span></span>|
|<span data-ttu-id="db3d0-166">replyTo</span><span class="sxs-lookup"><span data-stu-id="db3d0-166">replyTo</span></span>|<span data-ttu-id="db3d0-167">Recipient collection</span><span class="sxs-lookup"><span data-stu-id="db3d0-167">Recipient collection</span></span>|<span data-ttu-id="db3d0-168">返信時に使用される電子メール アドレス。</span><span class="sxs-lookup"><span data-stu-id="db3d0-168">The email addresses to use when replying.</span></span> <span data-ttu-id="db3d0-169">isDraft = trueの場合にのみ更新可能です。</span><span class="sxs-lookup"><span data-stu-id="db3d0-169">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="db3d0-170">sender</span><span class="sxs-lookup"><span data-stu-id="db3d0-170">sender</span></span>|<span data-ttu-id="db3d0-171">Recipient</span><span class="sxs-lookup"><span data-stu-id="db3d0-171">Recipient</span></span>|<span data-ttu-id="db3d0-172">メッセージを生成するために実際に使用されるアカウント。</span><span class="sxs-lookup"><span data-stu-id="db3d0-172">The account that is actually used to generate the message.</span></span> <span data-ttu-id="db3d0-173">isDraft = true の場合、そして[共有されているメールボックス](https://docs.microsoft.com/en-us/exchange/collaboration/shared-mailboxes/shared-mailboxes)からメッセージを送信、または [デリゲート](https://support.office.com/en-us/article/allow-someone-else-to-manage-your-mail-and-calendar-41c40c04-3bd1-4d22-963a-28eafec25926)としてメッセージを送信した場合にのみ更新可能です。</span><span class="sxs-lookup"><span data-stu-id="db3d0-173">Updatable only if isDraft = true, and when sending a message from a [shared mailbox](https://docs.microsoft.com/en-us/exchange/collaboration/shared-mailboxes/shared-mailboxes), or sending a message as a [delegate](https://support.office.com/en-us/article/allow-someone-else-to-manage-your-mail-and-calendar-41c40c04-3bd1-4d22-963a-28eafec25926).</span></span> <span data-ttu-id="db3d0-174">値は、使用される実際のメールボックスに対応する必要があります。</span><span class="sxs-lookup"><span data-stu-id="db3d0-174">In any case, the value must correspond to the actual mailbox used.</span></span>|
|<span data-ttu-id="db3d0-175">toRecipients</span><span class="sxs-lookup"><span data-stu-id="db3d0-175">toRecipients</span></span>|<span data-ttu-id="db3d0-176">Recipient collection</span><span class="sxs-lookup"><span data-stu-id="db3d0-176">Recipient collection</span></span>|<span data-ttu-id="db3d0-177">メッセージの宛先。</span><span class="sxs-lookup"><span data-stu-id="db3d0-177">The  To recipients for the message.</span></span> <span data-ttu-id="db3d0-178">isDraft = trueの場合にのみ更新可能です。</span><span class="sxs-lookup"><span data-stu-id="db3d0-178">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="db3d0-179">本文</span><span class="sxs-lookup"><span data-stu-id="db3d0-179">body</span></span>|<span data-ttu-id="db3d0-180">ItemBody</span><span class="sxs-lookup"><span data-stu-id="db3d0-180">ItemBody</span></span>|<span data-ttu-id="db3d0-181">メッセージの本文。</span><span class="sxs-lookup"><span data-stu-id="db3d0-181">The body of the message.</span></span> <span data-ttu-id="db3d0-182">isDraft = trueの場合にのみ更新可能です。</span><span class="sxs-lookup"><span data-stu-id="db3d0-182">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="db3d0-183">isDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="db3d0-183">isDeliveryReceiptRequested</span></span>|<span data-ttu-id="db3d0-184">ブーリアン</span><span class="sxs-lookup"><span data-stu-id="db3d0-184">Boolean</span></span>|<span data-ttu-id="db3d0-185">メッセージの開封応答が要求されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="db3d0-185">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="db3d0-186">isReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="db3d0-186">isReadReceiptRequested</span></span>|<span data-ttu-id="db3d0-187">ブーリアン</span><span class="sxs-lookup"><span data-stu-id="db3d0-187">Boolean</span></span>|<span data-ttu-id="db3d0-188">メッセージの開封応答が要求されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="db3d0-188">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="db3d0-189">subject</span><span class="sxs-lookup"><span data-stu-id="db3d0-189">subject</span></span>|<span data-ttu-id="db3d0-190">文字列</span><span class="sxs-lookup"><span data-stu-id="db3d0-190">String</span></span>|<span data-ttu-id="db3d0-191">メッセージの件名を指定します。</span><span class="sxs-lookup"><span data-stu-id="db3d0-191">The subject of the message.</span></span> <span data-ttu-id="db3d0-192">isDraft = trueの場合にのみ更新可能です。</span><span class="sxs-lookup"><span data-stu-id="db3d0-192">Updatable only if isDraft = true.</span></span>|

<span data-ttu-id="db3d0-193">**メッセージ** リソースは[拡張機能](../../../concepts/extensibility_overview.md)をサポートしているため、`PATCH` 操作を使用して、既存の**メッセージ** インスタンスで拡張機能のカスタム プロパティにあるアプリ固有のデータを追加、更新、または削除することができます。</span><span class="sxs-lookup"><span data-stu-id="db3d0-193">Since the **message** resource supports [extensions](../../../concepts/extensibility_overview.md), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **message** instance.</span></span>

## <a name="response"></a><span data-ttu-id="db3d0-194">応答</span><span class="sxs-lookup"><span data-stu-id="db3d0-194">Response</span></span>

<span data-ttu-id="db3d0-195">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [message](../resources/message.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="db3d0-195">If successful, this method returns a `200 OK` response code and updated [message](../resources/message.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="db3d0-196">例</span><span class="sxs-lookup"><span data-stu-id="db3d0-196">Example</span></span>
##### <a name="request"></a><span data-ttu-id="db3d0-197">要求</span><span class="sxs-lookup"><span data-stu-id="db3d0-197">Request</span></span>
<span data-ttu-id="db3d0-198">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="db3d0-198">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="db3d0-199">応答</span><span class="sxs-lookup"><span data-stu-id="db3d0-199">Response</span></span>
<span data-ttu-id="db3d0-p116">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="db3d0-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="db3d0-203">関連項目</span><span class="sxs-lookup"><span data-stu-id="db3d0-203">See also</span></span>

- [<span data-ttu-id="db3d0-204">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="db3d0-204">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="db3d0-205">オープン拡張機能を使用したユーザーへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="db3d0-205">Add custom data to users using open extensions (preview)</span></span>](../../../concepts/extensibility_open_users.md)
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
