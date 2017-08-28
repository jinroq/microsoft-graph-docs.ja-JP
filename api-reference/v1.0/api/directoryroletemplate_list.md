# <a name="list-directoryroletemplates"></a><span data-ttu-id="e853b-101">directoryRoleTemplates を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="e853b-101">List directoryRoleTemplates</span></span>

<span data-ttu-id="e853b-102">directoryRoleTemplate オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="e853b-102">Retrieve a list of directoryRoleTemplate objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="e853b-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e853b-103">Permissions</span></span>
<span data-ttu-id="e853b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e853b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="e853b-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e853b-106">Permission type</span></span>      | <span data-ttu-id="e853b-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e853b-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e853b-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e853b-108">Delegated (work or school account)</span></span> | <span data-ttu-id="e853b-109">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e853b-109">One of the following scopes is required to execute this API: Directory.Read.All; Directory.ReadWrite.All; Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e853b-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e853b-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e853b-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e853b-111">Not supported.</span></span>    |
|<span data-ttu-id="e853b-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e853b-112">Application</span></span> | <span data-ttu-id="e853b-113">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e853b-113">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e853b-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e853b-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoleTemplates
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e853b-115">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="e853b-115">Optional query parameters</span></span>
<span data-ttu-id="e853b-116">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)をサポート**していません** (例: $filter はここではサポートされていません)。</span><span class="sxs-lookup"><span data-stu-id="e853b-116">This method does **not** support the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response (e.g. $filter is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="e853b-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e853b-117">Request headers</span></span>
| <span data-ttu-id="e853b-118">名前</span><span class="sxs-lookup"><span data-stu-id="e853b-118">Name</span></span>       | <span data-ttu-id="e853b-119">型</span><span class="sxs-lookup"><span data-stu-id="e853b-119">Type</span></span> | <span data-ttu-id="e853b-120">説明</span><span class="sxs-lookup"><span data-stu-id="e853b-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e853b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e853b-121">Authorization</span></span>  | <span data-ttu-id="e853b-122">string</span><span class="sxs-lookup"><span data-stu-id="e853b-122">string</span></span>  | <span data-ttu-id="e853b-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e853b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e853b-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="e853b-125">Request body</span></span>
<span data-ttu-id="e853b-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="e853b-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e853b-127">応答</span><span class="sxs-lookup"><span data-stu-id="e853b-127">Response</span></span>

<span data-ttu-id="e853b-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryRoleTemplate](../resources/directoryroletemplate.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="e853b-128">If successful, this method returns a `200 OK` response code and collection of [directoryRoleTemplate](../resources/directoryroletemplate.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e853b-129">例</span><span class="sxs-lookup"><span data-stu-id="e853b-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e853b-130">要求</span><span class="sxs-lookup"><span data-stu-id="e853b-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_directoryroletemplates"
}-->
```http
GET https://graph.microsoft.com/v1.0/directoryRoleTemplates
```
##### <a name="response"></a><span data-ttu-id="e853b-131">応答</span><span class="sxs-lookup"><span data-stu-id="e853b-131">Response</span></span>
<span data-ttu-id="e853b-p103">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e853b-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryRoleTemplate",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "description": "description-value",
      "displayName": "displayName-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List directoryRoleTemplates",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
