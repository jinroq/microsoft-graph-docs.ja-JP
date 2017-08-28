# <a name="update-conversationthread"></a><span data-ttu-id="cc3c5-101">Update conversationthread</span><span class="sxs-lookup"><span data-stu-id="cc3c5-101">Update conversationthread</span></span>

<span data-ttu-id="cc3c5-102">スレッドへの以降の投稿を許可あるいは拒否するために、スレッドをロックまたはロック解除します。</span><span class="sxs-lookup"><span data-stu-id="cc3c5-102">Lock or unlock a thread, to allow or avoid further posting to the thread.</span></span>
## <a name="permissions"></a><span data-ttu-id="cc3c5-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="cc3c5-103">Permissions</span></span>
<span data-ttu-id="cc3c5-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cc3c5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="cc3c5-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="cc3c5-106">Permission type</span></span>      | <span data-ttu-id="cc3c5-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="cc3c5-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cc3c5-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="cc3c5-108">Delegated (work or school account)</span></span> | <span data-ttu-id="cc3c5-109">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cc3c5-109">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="cc3c5-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="cc3c5-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cc3c5-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cc3c5-111">Not supported.</span></span>    |
|<span data-ttu-id="cc3c5-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="cc3c5-112">Application</span></span> | <span data-ttu-id="cc3c5-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cc3c5-113">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cc3c5-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="cc3c5-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /groups/{id}/threads/{id}
PATCH /groups/{id}/conversations/{id}/threads/{id}

```
## <a name="request-headers"></a><span data-ttu-id="cc3c5-115">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cc3c5-115">Request headers</span></span>
| <span data-ttu-id="cc3c5-116">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cc3c5-116">Header</span></span>       | <span data-ttu-id="cc3c5-117">値</span><span class="sxs-lookup"><span data-stu-id="cc3c5-117">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="cc3c5-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="cc3c5-118">Authorization</span></span>  | <span data-ttu-id="cc3c5-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="cc3c5-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="cc3c5-121">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cc3c5-121">Content-Type</span></span>  | <span data-ttu-id="cc3c5-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="cc3c5-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="cc3c5-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="cc3c5-124">Request body</span></span>
<span data-ttu-id="cc3c5-p104">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="cc3c5-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="cc3c5-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cc3c5-128">Property</span></span>     | <span data-ttu-id="cc3c5-129">型</span><span class="sxs-lookup"><span data-stu-id="cc3c5-129">Type</span></span>   |<span data-ttu-id="cc3c5-130">説明</span><span class="sxs-lookup"><span data-stu-id="cc3c5-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cc3c5-131">isLocked</span><span class="sxs-lookup"><span data-stu-id="cc3c5-131">isLocked</span></span>|<span data-ttu-id="cc3c5-132">Boolean</span><span class="sxs-lookup"><span data-stu-id="cc3c5-132">Boolean</span></span>|<span data-ttu-id="cc3c5-p105">スレッドがロックされているかどうかを示します。転記を禁止するために `true` に設定します。</span><span class="sxs-lookup"><span data-stu-id="cc3c5-p105">Indicates if the thread is locked. Set to `true` to disallow posting.</span></span>|

## <a name="response"></a><span data-ttu-id="cc3c5-135">応答</span><span class="sxs-lookup"><span data-stu-id="cc3c5-135">Response</span></span>

<span data-ttu-id="cc3c5-136">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で、更新された [conversationThread](../resources/conversationthread.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="cc3c5-136">If successful, this method returns a `200 OK` response code and updated [conversationThread](../resources/conversationthread.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="cc3c5-137">例</span><span class="sxs-lookup"><span data-stu-id="cc3c5-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cc3c5-138">要求</span><span class="sxs-lookup"><span data-stu-id="cc3c5-138">Request</span></span>
<span data-ttu-id="cc3c5-139">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="cc3c5-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_conversationthread"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}
Content-type: application/json
Content-length: 419

{
  "@odata.type":"#Microsoft.OutlookServices.ConversationThread",
  "isLocked": true
}
```
##### <a name="response"></a><span data-ttu-id="cc3c5-140">応答</span><span class="sxs-lookup"><span data-stu-id="cc3c5-140">Response</span></span>
<span data-ttu-id="cc3c5-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="cc3c5-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationThread"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 419

{
  "toRecipients": [
    {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    }
  ],
  "topic": "topic-value",
  "hasAttachments": true,
  "lastDeliveredDateTime": "datetime-value",
  "uniqueSenders": [
    "uniqueSenders-value"
  ],
  "ccRecipients": [
    {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    }
  ],
  "isLocked": true 
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update conversationthread",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
