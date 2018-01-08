# <a name="update-event"></a><span data-ttu-id="60811-101">イベントを更新する</span><span class="sxs-lookup"><span data-stu-id="60811-101">Update event</span></span>
<span data-ttu-id="60811-102">[event](../resources/event.md) オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="60811-102">Update an [event](../resources/event.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="60811-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="60811-103">Permissions</span></span>
<span data-ttu-id="60811-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="60811-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="60811-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="60811-106">Permission type</span></span>      | <span data-ttu-id="60811-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="60811-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="60811-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="60811-108">Delegated (work or school account)</span></span> | <span data-ttu-id="60811-109">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="60811-109">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="60811-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="60811-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="60811-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="60811-111">Not supported.</span></span>    |
|<span data-ttu-id="60811-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="60811-112">Application</span></span> | <span data-ttu-id="60811-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="60811-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="60811-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="60811-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /groups/{id}/events/{id}
PATCH /groups/{id}/calendar/events/{id}
```

## <a name="request-headers"></a><span data-ttu-id="60811-115">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="60811-115">Request headers</span></span>
| <span data-ttu-id="60811-116">名前</span><span class="sxs-lookup"><span data-stu-id="60811-116">Name</span></span>       | <span data-ttu-id="60811-117">型</span><span class="sxs-lookup"><span data-stu-id="60811-117">Type</span></span> | <span data-ttu-id="60811-118">説明</span><span class="sxs-lookup"><span data-stu-id="60811-118">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="60811-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="60811-119">Authorization</span></span>  | <span data-ttu-id="60811-120">string</span><span class="sxs-lookup"><span data-stu-id="60811-120">string</span></span>  | <span data-ttu-id="60811-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="60811-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="60811-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="60811-123">Request body</span></span>
<span data-ttu-id="60811-p103">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="60811-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="60811-127">応答</span><span class="sxs-lookup"><span data-stu-id="60811-127">Response</span></span>
<span data-ttu-id="60811-128">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="60811-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="60811-129">例</span><span class="sxs-lookup"><span data-stu-id="60811-129">Example</span></span>
#### <a name="request"></a><span data-ttu-id="60811-130">要求</span><span class="sxs-lookup"><span data-stu-id="60811-130">Request</span></span>
<span data-ttu-id="60811-131">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="60811-131">The following is an example of the request body.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_group_event"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/groups/{id}/events/{id}
Content-type: application/json
Content-length: 211

{
  "originalStartTimeZone": "originalStartTimeZone-value",
  "originalEndTimeZone": "originalEndTimeZone-value",
  "responseStatus": {
    "response": "",
    "time": "datetime-value"
  },
  "iCalUId": "iCalUId-value",
  "reminderMinutesBeforeStart": 99,
  "isReminderOn": true
}
```

#### <a name="response"></a><span data-ttu-id="60811-132">応答</span><span class="sxs-lookup"><span data-stu-id="60811-132">Response</span></span>
<span data-ttu-id="60811-133">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="60811-133">The following is an example of a response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update event",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->