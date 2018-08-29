# <a name="create-or-replace-a-historyitem"></a><span data-ttu-id="be8e5-101">historyItem を作成または置換する</span><span class="sxs-lookup"><span data-stu-id="be8e5-101">Create or replace a history item</span></span>

<span data-ttu-id="be8e5-102">新規作成または既存のユーザー アクティビティの既存の履歴項目を置換します。</span><span class="sxs-lookup"><span data-stu-id="be8e5-102">Create a new or replace an existing history item for an existing user activity.</span></span>

## <a name="permissions"></a><span data-ttu-id="be8e5-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="be8e5-103">Permissions</span></span>

<span data-ttu-id="be8e5-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="be8e5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="be8e5-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="be8e5-106">Permission type</span></span>      | <span data-ttu-id="be8e5-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="be8e5-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="be8e5-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="be8e5-108">Delegated (work or school account)</span></span> | <span data-ttu-id="be8e5-109">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="be8e5-109">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="be8e5-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="be8e5-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="be8e5-111">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="be8e5-111">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="be8e5-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="be8e5-112">Application</span></span> | <span data-ttu-id="be8e5-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="be8e5-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="be8e5-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="be8e5-114">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /me/activities/{id}/historyItems/{id}
```

<span data-ttu-id="be8e5-115">Id は GUID である必要があります。</span><span class="sxs-lookup"><span data-stu-id="be8e5-115">Id needs to be a GUID.</span></span>

## <a name="request-headers"></a><span data-ttu-id="be8e5-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="be8e5-116">Request headers</span></span>

|<span data-ttu-id="be8e5-117">名前</span><span class="sxs-lookup"><span data-stu-id="be8e5-117">Name</span></span> | <span data-ttu-id="be8e5-118">型</span><span class="sxs-lookup"><span data-stu-id="be8e5-118">Type</span></span> | <span data-ttu-id="be8e5-119">説明</span><span class="sxs-lookup"><span data-stu-id="be8e5-119">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="be8e5-120">承認</span><span class="sxs-lookup"><span data-stu-id="be8e5-120">Authorization</span></span> | <span data-ttu-id="be8e5-121">文字列</span><span class="sxs-lookup"><span data-stu-id="be8e5-121">string</span></span> | <span data-ttu-id="be8e5-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="be8e5-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="be8e5-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="be8e5-124">Request body</span></span>

<span data-ttu-id="be8e5-125">要求の本文には、 [historyItem](../resources/projectrome_historyitem.md) オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="be8e5-125">In the request body, supply a JSON representation of [directoryObject](../resources/projectrome_historyitem.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="be8e5-126">応答</span><span class="sxs-lookup"><span data-stu-id="be8e5-126">Response</span></span>

<span data-ttu-id="be8e5-127">成功した場合、historyItem が作成または`201 Created`   historyItem が置換されていれば、このメソッドは`200 OK`   応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="be8e5-127">If successful, this method returns the `201 Created` response code if the historyItem was created or `200 OK` if the historyItem was replaced.</span></span>

## <a name="example"></a><span data-ttu-id="be8e5-128">例</span><span class="sxs-lookup"><span data-stu-id="be8e5-128">Example</span></span>

#### <a name="request"></a><span data-ttu-id="be8e5-129">要求</span><span class="sxs-lookup"><span data-stu-id="be8e5-129">Request</span></span>

<span data-ttu-id="be8e5-130">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="be8e5-130">Here is an example of the request.</span></span>

<!-- {
    "blockType": "ignored",
    "name": "upsert_historyItem"
} -->

```http
PUT https://graph.microsoft.com/v1.0/me/activities/{activity-id}/historyItems/{item-id}
Content-type: application/json
Content-length: 364

{
    "startedDateTime": "2015-02-11T20:54:04.3457274+00:00",
    "userTimezone": "Africa/Casablanca",
    "lastActiveDateTime": "2015-02-11T20:54:04.3457274+00:00"
}
```

#### <a name="response"></a><span data-ttu-id="be8e5-131">応答</span><span class="sxs-lookup"><span data-stu-id="be8e5-131">Response</span></span>

<span data-ttu-id="be8e5-132">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="be8e5-132">Here is an example of the response.</span></span>

<!-- {
    "blockType": "ignored",
    "truncated": true,
    "@odata.type": "microsoft.graph.activityHistoryItem"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('user%40contoso.com')/activities('13881113971988980728')/historyItems/$entity",
    "status": "updated",
    "userTimezone": "Africa/Casablanca",
    "createdDateTime": "2018-02-26T20:28:22.14Z",
    "lastModifiedDateTime": "2018-02-26T20:28:22.155Z",
    "id": "9d0b74e4-4b41-43ea-b34d-f9c1bf9f809c",
    "startedDateTime": "2018-02-26T20:54:04.345Z",
    "lastActiveDateTime": "2018-02-26T20:54:24.345Z",
    "expirationDateTime": "2018-03-28T20:28:22.14Z",
    "activeDurationSeconds": 20
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Upsert historyitem",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->