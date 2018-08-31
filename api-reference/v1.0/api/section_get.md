# <a name="get-section"></a><span data-ttu-id="aec70-101">Get section</span><span class="sxs-lookup"><span data-stu-id="aec70-101">Get section</span></span>

<span data-ttu-id="aec70-102">[onenoteSection](../resources/section.md) オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="aec70-102">Retrieve the properties and relationships of [plannertaskdetails](../resources/section.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="aec70-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="aec70-103">Permissions</span></span>
<span data-ttu-id="aec70-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="aec70-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="aec70-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="aec70-106">Permission type</span></span>      | <span data-ttu-id="aec70-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="aec70-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aec70-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="aec70-108">Delegated (work or school account)</span></span> | <span data-ttu-id="aec70-109">Notes.Create、Notes.Read、Notes.ReadWrite、Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aec70-109">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="aec70-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="aec70-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aec70-111">Notes.Create、Notes.Read、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="aec70-111">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="aec70-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="aec70-112">Application</span></span> | <span data-ttu-id="aec70-113">Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aec70-113">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="aec70-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="aec70-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/sections/{id}
GET /users/{id | userPrincipalName}/onenote/sections/{id}
GET /groups/{id}/onenote/sections/{id}
GET /sites/{id}/onenote/sections/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="aec70-115">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="aec70-115">Optional query parameters</span></span>
<span data-ttu-id="aec70-116">このメソッドは、応答をカスタマイズするための `select` および `expand` [OData クエリ パラメーター](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="aec70-116">This method supports the `select` and `expand` [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="aec70-p102">既定のクエリが `parentNotebook` を展開し、`id`、`displayName`、`self` プロパティを選択します。セクションの有効な `expand` 値は、`parentNotebook` と `parentSectionGroup` です。</span><span class="sxs-lookup"><span data-stu-id="aec70-p102">The default query expands `parentNotebook` and selects its `id`, `displayName`, and `self` properties. Valid `expand` values for sections are `parentNotebook` and `parentSectionGroup`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="aec70-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="aec70-119">Request headers</span></span>
| <span data-ttu-id="aec70-120">名前</span><span class="sxs-lookup"><span data-stu-id="aec70-120">Name</span></span>       | <span data-ttu-id="aec70-121">型</span><span class="sxs-lookup"><span data-stu-id="aec70-121">Type</span></span> | <span data-ttu-id="aec70-122">説明</span><span class="sxs-lookup"><span data-stu-id="aec70-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="aec70-123">承認</span><span class="sxs-lookup"><span data-stu-id="aec70-123">Authorization</span></span>  | <span data-ttu-id="aec70-124">文字列</span><span class="sxs-lookup"><span data-stu-id="aec70-124">string</span></span>  | <span data-ttu-id="aec70-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="aec70-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="aec70-127">承諾</span><span class="sxs-lookup"><span data-stu-id="aec70-127">Accept</span></span> | <span data-ttu-id="aec70-128">string</span><span class="sxs-lookup"><span data-stu-id="aec70-128">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="aec70-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="aec70-129">Request body</span></span>
<span data-ttu-id="aec70-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="aec70-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aec70-131">応答</span><span class="sxs-lookup"><span data-stu-id="aec70-131">Response</span></span>

<span data-ttu-id="aec70-132">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [onenoteSection](../resources/section.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="aec70-132">If successful, this method returns a `200 OK` response code and a [managedDeviceMobileAppConfigurationAssignment](../resources/section.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="aec70-133">例</span><span class="sxs-lookup"><span data-stu-id="aec70-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="aec70-134">要求</span><span class="sxs-lookup"><span data-stu-id="aec70-134">Request</span></span>
<span data-ttu-id="aec70-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="aec70-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_section"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/sections/{id}
```
##### <a name="response"></a><span data-ttu-id="aec70-136">応答</span><span class="sxs-lookup"><span data-stu-id="aec70-136">Response</span></span>
<span data-ttu-id="aec70-p104">以下は、応答の例です。注:ここに示す応答オブジェクトは切り詰めて簡略化されています。実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="aec70-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenoteSection"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 272

{
  "isDefault": true,
  "pagesUrl": "pagesUrl-value",
  "displayName": "name-value",
  "createdBy": {
    "user": {
      "id": "id-value",
      "displayName": "displayName-value"
    }
  },
  "lastModifiedBy": {
    "user": {
      "id": "id-value",
      "displayName": "displayName-value"
    }
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get section",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->