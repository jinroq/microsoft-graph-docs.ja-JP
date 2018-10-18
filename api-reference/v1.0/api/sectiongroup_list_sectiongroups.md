# <a name="list-sectiongroups"></a><span data-ttu-id="b2b6b-101">sectionGroups を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="b2b6b-101">List sectionGroups</span></span>

<span data-ttu-id="b2b6b-102">指定されたセクション グループから[セクション グループ](../resources/sectiongroup.md)の一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="b2b6b-102">Retrieve a list of [section groups](../resources/sectiongroup.md) from the specified section group.</span></span>
## <a name="permissions"></a><span data-ttu-id="b2b6b-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b2b6b-103">Permissions</span></span>
<span data-ttu-id="b2b6b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b2b6b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b2b6b-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b2b6b-106">Permission type</span></span>      | <span data-ttu-id="b2b6b-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b2b6b-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b2b6b-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b2b6b-108">Delegated (work or school account)</span></span> | <span data-ttu-id="b2b6b-109">Notes.Create、Notes.Read、Notes.ReadWrite、Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2b6b-109">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="b2b6b-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b2b6b-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b2b6b-111">Notes.Create、Notes.Read、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b2b6b-111">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="b2b6b-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b2b6b-112">Application</span></span> | <span data-ttu-id="b2b6b-113">Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2b6b-113">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b2b6b-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b2b6b-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/sectionGroups/{id}/sectionGroups
GET /users/{id | userPrincipalName}/onenote/sectionGroups/{id}/sectionGroups
GET /groups/{id}/onenote/sectionGroups/{id}/sectionGroups
GET /sites/{id}/onenote/sectionGroups/{id}/sectionGroups
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b2b6b-115">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="b2b6b-115">Optional query parameters</span></span>
<span data-ttu-id="b2b6b-116">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="b2b6b-116">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="b2b6b-117">既定の並べ替え順序は `name asc` です。</span><span class="sxs-lookup"><span data-stu-id="b2b6b-117">The default sort order is `name asc`.</span></span>

<span data-ttu-id="b2b6b-p102">既定のクエリが `parentNotebook` を展開し、`id`、`displayName`、`self` プロパティを選択します。セクション グループで有効な `expand` 値は、`sections`、`sectionGroups`、`parentNotebook`、`parentSectionGroup` です。</span><span class="sxs-lookup"><span data-stu-id="b2b6b-p102">The default query expands `parentNotebook` and selects its `id`, `displayName`, and `self` properties. Valid `expand` values for section groups are `sections`, `sectionGroups`, `parentNotebook`, and `parentSectionGroup`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b2b6b-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b2b6b-120">Request headers</span></span>
| <span data-ttu-id="b2b6b-121">名前</span><span class="sxs-lookup"><span data-stu-id="b2b6b-121">Name</span></span>       | <span data-ttu-id="b2b6b-122">型</span><span class="sxs-lookup"><span data-stu-id="b2b6b-122">Type</span></span> | <span data-ttu-id="b2b6b-123">説明</span><span class="sxs-lookup"><span data-stu-id="b2b6b-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="b2b6b-124">承認</span><span class="sxs-lookup"><span data-stu-id="b2b6b-124">Authorization</span></span>  | <span data-ttu-id="b2b6b-125">文字列</span><span class="sxs-lookup"><span data-stu-id="b2b6b-125">string</span></span>  | <span data-ttu-id="b2b6b-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="b2b6b-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b2b6b-128">承諾</span><span class="sxs-lookup"><span data-stu-id="b2b6b-128">Accept</span></span> | <span data-ttu-id="b2b6b-129">文字列</span><span class="sxs-lookup"><span data-stu-id="b2b6b-129">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="b2b6b-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="b2b6b-130">Request body</span></span>
<span data-ttu-id="b2b6b-131">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="b2b6b-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b2b6b-132">応答</span><span class="sxs-lookup"><span data-stu-id="b2b6b-132">Response</span></span>

<span data-ttu-id="b2b6b-133">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [sectionGroup](../resources/sectiongroup.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="b2b6b-133">If successful, this method returns a `200 OK` response code and a collection of [sectionGroup](../resources/sectiongroup.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b2b6b-134">例</span><span class="sxs-lookup"><span data-stu-id="b2b6b-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b2b6b-135">要求</span><span class="sxs-lookup"><span data-stu-id="b2b6b-135">Request</span></span>
<span data-ttu-id="b2b6b-136">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b2b6b-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_sectiongroups"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/sectionGroups/{id}/sectionGroups
```
##### <a name="response"></a><span data-ttu-id="b2b6b-137">応答</span><span class="sxs-lookup"><span data-stu-id="b2b6b-137">Response</span></span>
<span data-ttu-id="b2b6b-p104">以下は、応答の例です。注:ここに示す応答オブジェクトは切り詰めて簡略化されています。実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="b2b6b-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sectionGroup",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 378

{
  "value": [
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
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List sectionGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->