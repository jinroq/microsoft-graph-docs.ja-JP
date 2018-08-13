# <a name="list-registeredowners"></a><span data-ttu-id="8b246-101">registeredOwners を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="8b246-101">List registeredOwners</span></span>

<span data-ttu-id="8b246-102">デバイスの登録済み所有者の一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="8b246-102">Retrieve a list of users that are registered owners of the device.</span></span> <span data-ttu-id="8b246-103">登録済み所有者は、デバイスがクラウドに参加済みか、または個人用デバイスが登録済みのユーザーです。</span><span class="sxs-lookup"><span data-stu-id="8b246-103">A registered owner is the user that cloud joined the device or registered their personal device.</span></span> <span data-ttu-id="8b246-104">登録済み所有者は、登録時に設定されます。</span><span class="sxs-lookup"><span data-stu-id="8b246-104">The registered owner is set at the time of registration.</span></span> <span data-ttu-id="8b246-105">現在、所有者は 1 人しかいることができません。</span><span class="sxs-lookup"><span data-stu-id="8b246-105">Currently, there can be only one owner.</span></span>

## <a name="permissions"></a><span data-ttu-id="8b246-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8b246-106">Permissions</span></span>
<span data-ttu-id="8b246-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8b246-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="8b246-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8b246-109">Permission type</span></span>      | <span data-ttu-id="8b246-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="8b246-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8b246-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8b246-111">Delegated (work or school account)</span></span> | <span data-ttu-id="8b246-112">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8b246-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="8b246-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8b246-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8b246-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8b246-114">Not supported.</span></span>    |
|<span data-ttu-id="8b246-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8b246-115">Application</span></span> | <span data-ttu-id="8b246-116">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b246-116">Directory.Read.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8b246-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8b246-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}/registeredOwners
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8b246-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="8b246-118">Optional query parameters</span></span>
<span data-ttu-id="8b246-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](http://developer.microsoft.com/ja-JP/graph/docs/overview/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="8b246-119">This method supports the [OData Query Parameters](http://developer.microsoft.com/ja-JP/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="8b246-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8b246-120">Request headers</span></span>
| <span data-ttu-id="8b246-121">名前</span><span class="sxs-lookup"><span data-stu-id="8b246-121">Name</span></span>       | <span data-ttu-id="8b246-122">型</span><span class="sxs-lookup"><span data-stu-id="8b246-122">Type</span></span> | <span data-ttu-id="8b246-123">説明</span><span class="sxs-lookup"><span data-stu-id="8b246-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="8b246-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="8b246-124">Authorization</span></span>  | <span data-ttu-id="8b246-125">string</span><span class="sxs-lookup"><span data-stu-id="8b246-125">string</span></span>  | <span data-ttu-id="8b246-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="8b246-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8b246-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="8b246-128">Request body</span></span>
<span data-ttu-id="8b246-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="8b246-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8b246-130">応答</span><span class="sxs-lookup"><span data-stu-id="8b246-130">Response</span></span>

<span data-ttu-id="8b246-131">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryObject](../resources/directoryobject.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="8b246-131">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8b246-132">例</span><span class="sxs-lookup"><span data-stu-id="8b246-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8b246-133">要求</span><span class="sxs-lookup"><span data-stu-id="8b246-133">Request</span></span>
<span data-ttu-id="8b246-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8b246-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_registeredowners"
}-->
```http
GET https://graph.microsoft.com/v1.0/devices/{id}/registeredOwners
```
##### <a name="response"></a><span data-ttu-id="8b246-135">応答</span><span class="sxs-lookup"><span data-stu-id="8b246-135">Response</span></span>
<span data-ttu-id="8b246-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8b246-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List registeredOwners",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->