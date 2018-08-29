# <a name="update-conversation-thread"></a><span data-ttu-id="9a7ee-101">会話スレッドを更新する</span><span class="sxs-lookup"><span data-stu-id="9a7ee-101">Update conversation thread</span></span>
<span data-ttu-id="9a7ee-102">[thread](../resources/conversationthread.md) オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="9a7ee-102">Update a [thread](../resources/conversationthread.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9a7ee-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="9a7ee-103">Permissions</span></span>
<span data-ttu-id="9a7ee-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9a7ee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="9a7ee-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9a7ee-106">Permission type</span></span>      | <span data-ttu-id="9a7ee-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="9a7ee-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9a7ee-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9a7ee-108">Delegated (work or school account)</span></span> | <span data-ttu-id="9a7ee-109">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a7ee-109">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="9a7ee-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9a7ee-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9a7ee-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9a7ee-111">Not supported.</span></span>    |
|<span data-ttu-id="9a7ee-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9a7ee-112">Application</span></span> | <span data-ttu-id="9a7ee-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9a7ee-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9a7ee-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9a7ee-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /groups/{id}/threads/{id}
```

## <a name="request-headers"></a><span data-ttu-id="9a7ee-115">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9a7ee-115">Request headers</span></span>
| <span data-ttu-id="9a7ee-116">名前</span><span class="sxs-lookup"><span data-stu-id="9a7ee-116">Name</span></span>       | <span data-ttu-id="9a7ee-117">型</span><span class="sxs-lookup"><span data-stu-id="9a7ee-117">Type</span></span> | <span data-ttu-id="9a7ee-118">説明</span><span class="sxs-lookup"><span data-stu-id="9a7ee-118">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="9a7ee-119">承認</span><span class="sxs-lookup"><span data-stu-id="9a7ee-119">Authorization</span></span>  | <span data-ttu-id="9a7ee-120">文字列</span><span class="sxs-lookup"><span data-stu-id="9a7ee-120">string</span></span>  | <span data-ttu-id="9a7ee-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="9a7ee-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9a7ee-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="9a7ee-123">Request body</span></span>
<span data-ttu-id="9a7ee-p103">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="9a7ee-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="9a7ee-127">応答</span><span class="sxs-lookup"><span data-stu-id="9a7ee-127">Response</span></span>
<span data-ttu-id="9a7ee-128">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="9a7ee-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="9a7ee-129">例</span><span class="sxs-lookup"><span data-stu-id="9a7ee-129">Example</span></span>
#### <a name="request"></a><span data-ttu-id="9a7ee-130">要求</span><span class="sxs-lookup"><span data-stu-id="9a7ee-130">Request</span></span>
<span data-ttu-id="9a7ee-131">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9a7ee-131">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["02bd9fd6-8f93-4758-87c3-1fb73740a315", "AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgMkABAAG5c7eC4NYEynIoXsuxXB9RAAG5c7eC4NYEynIoXsuxXB9Q=="],
  "name": "update_group_thread"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/threads/AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgMkABAAG5c7eC4NYEynIoXsuxXB9RAAG5c7eC4NYEynIoXsuxXB9Q==
Content-type: application/json
Content-length: 655

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

#### <a name="response"></a><span data-ttu-id="9a7ee-132">応答</span><span class="sxs-lookup"><span data-stu-id="9a7ee-132">Response</span></span>
<span data-ttu-id="9a7ee-133">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9a7ee-133">The following is an example of the response.</span></span>

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
  "description": "Update group thread",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->