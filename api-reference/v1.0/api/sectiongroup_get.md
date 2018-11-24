# <a name="get-sectiongroup"></a><span data-ttu-id="477b4-101">Get sectionGroup</span><span class="sxs-lookup"><span data-stu-id="477b4-101">Get sectionGroup</span></span>

<span data-ttu-id="477b4-102">[sectionGroup](../resources/sectiongroup.md) オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="477b4-102">Retrieve the properties and relationships of a [sectionGroup](../resources/sectiongroup.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="477b4-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="477b4-103">Permissions</span></span>
<span data-ttu-id="477b4-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="477b4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="477b4-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="477b4-106">Permission type</span></span>      | <span data-ttu-id="477b4-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="477b4-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="477b4-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="477b4-108">Delegated (work or school account)</span></span> | <span data-ttu-id="477b4-109">Notes.Create、Notes.Read、Notes.ReadWrite、Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="477b4-109">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="477b4-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="477b4-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="477b4-111">Notes.Create、Notes.Read、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="477b4-111">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="477b4-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="477b4-112">Application</span></span> | <span data-ttu-id="477b4-113">Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="477b4-113">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="477b4-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="477b4-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/sectionGroups/{id}
GET /users/{id | userPrincipalName}/onenote/sectionGroups/{id}
GET /groups/{id}/onenote/sectionGroups/{id}
GET /sites/{id}/onenote/sectionGroups/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="477b4-115">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="477b4-115">Optional query parameters</span></span>
<span data-ttu-id="477b4-116">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="477b4-116">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="477b4-p102">既定のクエリが `parentNotebook` を展開し、`id`、`name`、`self` プロパティを選択します。セクション グループの有効な `expand` 値は、`parentNotebook` と `parentSectionGroup` です。</span><span class="sxs-lookup"><span data-stu-id="477b4-p102">The default query expands `parentNotebook` and selects its `id`, `name`, and `self` properties. Valid `expand` values for section groups are `parentNotebook` and `parentSectionGroup`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="477b4-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="477b4-119">Request headers</span></span>
| <span data-ttu-id="477b4-120">名前</span><span class="sxs-lookup"><span data-stu-id="477b4-120">Name</span></span>       | <span data-ttu-id="477b4-121">型</span><span class="sxs-lookup"><span data-stu-id="477b4-121">Type</span></span> | <span data-ttu-id="477b4-122">説明</span><span class="sxs-lookup"><span data-stu-id="477b4-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="477b4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="477b4-123">Authorization</span></span>  | <span data-ttu-id="477b4-124">string</span><span class="sxs-lookup"><span data-stu-id="477b4-124">string</span></span>  | <span data-ttu-id="477b4-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="477b4-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="477b4-127">承諾</span><span class="sxs-lookup"><span data-stu-id="477b4-127">Accept</span></span> | <span data-ttu-id="477b4-128">string</span><span class="sxs-lookup"><span data-stu-id="477b4-128">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="477b4-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="477b4-129">Request body</span></span>
<span data-ttu-id="477b4-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="477b4-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="477b4-131">応答</span><span class="sxs-lookup"><span data-stu-id="477b4-131">Response</span></span>

<span data-ttu-id="477b4-132">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [sectionGroup](../resources/sectiongroup.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="477b4-132">If successful, this method returns a `200 OK` response code and a [sectionGroup](../resources/sectiongroup.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="477b4-133">例</span><span class="sxs-lookup"><span data-stu-id="477b4-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="477b4-134">要求</span><span class="sxs-lookup"><span data-stu-id="477b4-134">Request</span></span>
<span data-ttu-id="477b4-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="477b4-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_sectiongroup"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/sectionGroups/{id}
```
##### <a name="response"></a><span data-ttu-id="477b4-136">応答</span><span class="sxs-lookup"><span data-stu-id="477b4-136">Response</span></span>
<span data-ttu-id="477b4-p104">以下は、応答の例です。注:ここに示す応答オブジェクトは切り詰めて簡略化されています。実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="477b4-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sectionGroup"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 305

{
  "sectionsUrl": "sectionsUrl-value",
  "sectionGroupsUrl": "sectionGroupsUrl-value",
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
  "description": "Get sectionGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->