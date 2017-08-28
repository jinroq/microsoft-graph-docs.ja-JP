# <a name="update-eventmessage"></a><span data-ttu-id="0297c-101">eventMessage の更新</span><span class="sxs-lookup"><span data-stu-id="0297c-101">Update eventmessage</span></span>

<span data-ttu-id="0297c-102">eventmessage オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="0297c-102">Update the properties of eventmessage object.</span></span>
## <a name="permissions"></a><span data-ttu-id="0297c-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="0297c-103">Permissions</span></span>
<span data-ttu-id="0297c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0297c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="0297c-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0297c-106">Permission type</span></span>      | <span data-ttu-id="0297c-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="0297c-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0297c-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0297c-108">Delegated (work or school account)</span></span> | <span data-ttu-id="0297c-109">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0297c-109">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="0297c-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0297c-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0297c-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0297c-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="0297c-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0297c-112">Application</span></span> | <span data-ttu-id="0297c-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0297c-113">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="0297c-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0297c-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/messages/{id}
PATCH /users/{id | userPrincipalName}/messages/{id}

PATCH /me/mailFolders/{id}/messages/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="0297c-115">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0297c-115">Request headers</span></span>
| <span data-ttu-id="0297c-116">名前</span><span class="sxs-lookup"><span data-stu-id="0297c-116">Name</span></span>       | <span data-ttu-id="0297c-117">型</span><span class="sxs-lookup"><span data-stu-id="0297c-117">Type</span></span> | <span data-ttu-id="0297c-118">説明</span><span class="sxs-lookup"><span data-stu-id="0297c-118">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="0297c-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="0297c-119">Authorization</span></span>  | <span data-ttu-id="0297c-120">string</span><span class="sxs-lookup"><span data-stu-id="0297c-120">string</span></span>  | <span data-ttu-id="0297c-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="0297c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0297c-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0297c-123">Content-Type</span></span> | <span data-ttu-id="0297c-124">string</span><span class="sxs-lookup"><span data-stu-id="0297c-124">string</span></span>  | <span data-ttu-id="0297c-p103">エンティティ本文内のデータの性質です。必須。</span><span class="sxs-lookup"><span data-stu-id="0297c-p103">Nature of the data in the body of an entity. Required.</span></span> |
## <a name="request-body"></a><span data-ttu-id="0297c-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="0297c-127">Request body</span></span>
<span data-ttu-id="0297c-p104">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。以下のプロパティは書き込み可能または更新可能です。</span><span class="sxs-lookup"><span data-stu-id="0297c-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed. Writable/Updatable properties are</span></span>

| <span data-ttu-id="0297c-132">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0297c-132">Property</span></span>     | <span data-ttu-id="0297c-133">型</span><span class="sxs-lookup"><span data-stu-id="0297c-133">Type</span></span>   |<span data-ttu-id="0297c-134">説明</span><span class="sxs-lookup"><span data-stu-id="0297c-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0297c-135">categories</span><span class="sxs-lookup"><span data-stu-id="0297c-135">categories</span></span>|<span data-ttu-id="0297c-136">String</span><span class="sxs-lookup"><span data-stu-id="0297c-136">String</span></span>|<span data-ttu-id="0297c-137">メッセージに関連付けられたカテゴリ。</span><span class="sxs-lookup"><span data-stu-id="0297c-137">The categories associated with the message.</span></span>|
|<span data-ttu-id="0297c-138">importance</span><span class="sxs-lookup"><span data-stu-id="0297c-138">importance</span></span>|<span data-ttu-id="0297c-139">String</span><span class="sxs-lookup"><span data-stu-id="0297c-139">String</span></span>|<span data-ttu-id="0297c-p105">メッセージの重要度です。可能な値は、`Low`、`Normal`、`High` です。</span><span class="sxs-lookup"><span data-stu-id="0297c-p105">The importance of the message. Possible values are: `Low`, `Normal`, `High`.</span></span>|
|<span data-ttu-id="0297c-142">isDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="0297c-142">isDeliveryReceiptRequested</span></span>|<span data-ttu-id="0297c-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="0297c-143">Boolean</span></span>|<span data-ttu-id="0297c-144">メッセージの開封応答が要求されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="0297c-144">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="0297c-145">isRead</span><span class="sxs-lookup"><span data-stu-id="0297c-145">isRead</span></span>|<span data-ttu-id="0297c-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="0297c-146">Boolean</span></span>|<span data-ttu-id="0297c-147">メッセージが開封されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="0297c-147">Indicates whether the message has been read.</span></span>|
|<span data-ttu-id="0297c-148">isReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="0297c-148">isReadReceiptRequested</span></span>|<span data-ttu-id="0297c-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="0297c-149">Boolean</span></span>|<span data-ttu-id="0297c-150">メッセージの開封応答が要求されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="0297c-150">Indicates whether a read receipt is requested for the message.</span></span>|

## <a name="response"></a><span data-ttu-id="0297c-151">応答</span><span class="sxs-lookup"><span data-stu-id="0297c-151">Response</span></span>

<span data-ttu-id="0297c-152">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で、更新された [eventMessage](../resources/eventmessage.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="0297c-152">If successful, this method returns a `200 OK` response code and updated [eventMessage](../resources/eventmessage.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0297c-153">例</span><span class="sxs-lookup"><span data-stu-id="0297c-153">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0297c-154">要求</span><span class="sxs-lookup"><span data-stu-id="0297c-154">Request</span></span>
<span data-ttu-id="0297c-155">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0297c-155">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_eventmessage"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/messages/{id}
Content-type: application/json
Content-length: 248

{
  "isRead": "true",
}
```
##### <a name="response"></a><span data-ttu-id="0297c-156">応答</span><span class="sxs-lookup"><span data-stu-id="0297c-156">Response</span></span>
<span data-ttu-id="0297c-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0297c-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.eventmessage"
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
  "meetingMessageType": "meetingMessageType-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update eventmessage",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
