# <a name="get-page"></a><span data-ttu-id="ff5da-101">ページを取得する</span><span class="sxs-lookup"><span data-stu-id="ff5da-101">Get page</span></span>

<span data-ttu-id="ff5da-102">[ページ](../resources/page.md) オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="ff5da-102">Retrieve the properties and relationships of a [page](../resources/page.md) object.</span></span>

<span data-ttu-id="ff5da-103">**ページ情報を取得する**</span><span class="sxs-lookup"><span data-stu-id="ff5da-103">**Getting page information**</span></span>

<span data-ttu-id="ff5da-104">ページ識別子によって、ページのメタデータにアクセスします。</span><span class="sxs-lookup"><span data-stu-id="ff5da-104">Access a page's metadata by page identifier:</span></span>

```
GET /me/onenote/pages/{id}
```

<span data-ttu-id="ff5da-105">**ページ コンテンツを取得する**</span><span class="sxs-lookup"><span data-stu-id="ff5da-105">**Getting page content**</span></span>

<span data-ttu-id="ff5da-106">ページの `content` エンドポイントを使用して、ページの HTML コンテンツを取得できます。</span><span class="sxs-lookup"><span data-stu-id="ff5da-106">You can use the page's `content` endpoint to get the HTML content of a page:</span></span>

```
GET /me/onenote/pages/{id}/content[?includeIDs=true]
GET /me/onenote/pages/{id}/$value[?includeIDs=true]
```

<span data-ttu-id="ff5da-107">`includeIDs=true` クエリ オプションを使用して[ページを更新します](../api/page_update.md)。</span><span class="sxs-lookup"><span data-stu-id="ff5da-107">The `includeIDs=true` query option is used to [update pages](../api/page_update.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ff5da-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ff5da-108">Permissions</span></span>
<span data-ttu-id="ff5da-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ff5da-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ff5da-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ff5da-111">Permission type</span></span>      | <span data-ttu-id="ff5da-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ff5da-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ff5da-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ff5da-113">Delegated (work or school account)</span></span> | <span data-ttu-id="ff5da-114">Notes.Read、Notes.ReadWrite、Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff5da-114">Notes.Read, Notes.ReadWrite, Notes.Read.All, or Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="ff5da-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ff5da-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ff5da-116">Notes.Read、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ff5da-116">Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="ff5da-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ff5da-117">Application</span></span> | <span data-ttu-id="ff5da-118">Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff5da-118">Notes.Read, Notes.ReadWrite, Notes.Read.All, or Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ff5da-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ff5da-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/pages/{id}
GET /users/{id | userPrincipalName}/onenote/pages/{id}
GET /groups/{id}/onenote/pages/{id}
GET /sites/{id}/onenote/pages/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ff5da-120">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="ff5da-120">Optional query parameters</span></span>
<span data-ttu-id="ff5da-121">このメソッドは、応答をカスタマイズするための `select` および `expand` [OData クエリ パラメーター](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="ff5da-121">This method supports the `select` and `expand` [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="ff5da-p102">既定の応答は、`parentSection` を展開し、セクションの `id`、`name`、`self` プロパティを選択します。ページの有効な `expand` 値は、`parentNotebook` と `parentSection` です。</span><span class="sxs-lookup"><span data-stu-id="ff5da-p102">The default response expands `parentSection` and selects the section's `id`, `name`, and `self` properties. Valid `expand` values for pages are `parentNotebook` and `parentSection`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ff5da-124">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ff5da-124">Request headers</span></span>
| <span data-ttu-id="ff5da-125">名前</span><span class="sxs-lookup"><span data-stu-id="ff5da-125">Name</span></span>       | <span data-ttu-id="ff5da-126">型</span><span class="sxs-lookup"><span data-stu-id="ff5da-126">Type</span></span> | <span data-ttu-id="ff5da-127">説明</span><span class="sxs-lookup"><span data-stu-id="ff5da-127">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="ff5da-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="ff5da-128">Authorization</span></span>  | <span data-ttu-id="ff5da-129">string</span><span class="sxs-lookup"><span data-stu-id="ff5da-129">string</span></span>  | <span data-ttu-id="ff5da-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ff5da-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ff5da-132">承諾</span><span class="sxs-lookup"><span data-stu-id="ff5da-132">Accept</span></span> | <span data-ttu-id="ff5da-133">string</span><span class="sxs-lookup"><span data-stu-id="ff5da-133">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="ff5da-134">要求本文</span><span class="sxs-lookup"><span data-stu-id="ff5da-134">Request body</span></span>
<span data-ttu-id="ff5da-135">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="ff5da-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ff5da-136">応答</span><span class="sxs-lookup"><span data-stu-id="ff5da-136">Response</span></span>

<span data-ttu-id="ff5da-137">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [page](../resources/page.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ff5da-137">If successful, this method returns a `200 OK` response code and the [page](../resources/page.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ff5da-138">例</span><span class="sxs-lookup"><span data-stu-id="ff5da-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ff5da-139">要求</span><span class="sxs-lookup"><span data-stu-id="ff5da-139">Request</span></span>
<span data-ttu-id="ff5da-140">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ff5da-140">Here is an example of the request.</span></span>
 <!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/pages/{id}
```
##### <a name="response"></a><span data-ttu-id="ff5da-141">応答</span><span class="sxs-lookup"><span data-stu-id="ff5da-141">Response</span></span>
<span data-ttu-id="ff5da-p104">以下は、応答の例です。注:ここに示す応答オブジェクトは切り詰めて簡略化されています。実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="ff5da-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
 <!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 312

{
  "title": "title-value",
  "createdByAppId": "createdByAppId-value",
  "links": {
    "oneNoteClientUrl": {
      "href": "href-value"
    },
    "oneNoteWebUrl": {
      "href": "href-value"
    }
  },
  "contentUrl": "contentUrl-value",
  "content": "content-value",
  "lastModifiedDateTime": "2016-10-19T10:37:00Z"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get page",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
