# <a name="get-schemaextension"></a><span data-ttu-id="5e181-101">schemaExtension を取得する</span><span class="sxs-lookup"><span data-stu-id="5e181-101">Get schemaExtension</span></span>
<span data-ttu-id="5e181-102">指定された [schemaExtension](../resources/schemaextension.md) 定義のプロパティを取得します。</span><span class="sxs-lookup"><span data-stu-id="5e181-102">Get the properties of the specified [schemaExtension](../resources/schemaextension.md) definition.</span></span>

## <a name="permissions"></a><span data-ttu-id="5e181-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="5e181-103">Permissions</span></span>
<span data-ttu-id="5e181-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5e181-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="5e181-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5e181-106">Permission type</span></span>      | <span data-ttu-id="5e181-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="5e181-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5e181-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5e181-108">Delegated (work or school account)</span></span> | <span data-ttu-id="5e181-109">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5e181-109">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5e181-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5e181-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5e181-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5e181-111">Not supported.</span></span>    |
|<span data-ttu-id="5e181-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5e181-112">Application</span></span> | <span data-ttu-id="5e181-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5e181-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5e181-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5e181-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /schemaExtensions/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="5e181-115">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="5e181-115">Optional query parameters</span></span>
<span data-ttu-id="5e181-116">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="5e181-116">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5e181-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5e181-117">Request headers</span></span>
| <span data-ttu-id="5e181-118">名前</span><span class="sxs-lookup"><span data-stu-id="5e181-118">Name</span></span>      |<span data-ttu-id="5e181-119">説明</span><span class="sxs-lookup"><span data-stu-id="5e181-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5e181-120">承認</span><span class="sxs-lookup"><span data-stu-id="5e181-120">Authorization</span></span>  | <span data-ttu-id="5e181-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="5e181-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5e181-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5e181-123">Content-Type</span></span>   | <span data-ttu-id="5e181-124">アプリケーション /json</span><span class="sxs-lookup"><span data-stu-id="5e181-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="5e181-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="5e181-125">Request body</span></span>
<span data-ttu-id="5e181-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="5e181-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5e181-127">応答</span><span class="sxs-lookup"><span data-stu-id="5e181-127">Response</span></span>

<span data-ttu-id="5e181-128">成功した場合、このメソッドは応答本文で `200 OK` 応答コードと [schemaExtension](../resources/schemaextension.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="5e181-128">If successful, this method returns a `200 OK` response code and [schemaExtension](../resources/schemaextension.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5e181-129">例</span><span class="sxs-lookup"><span data-stu-id="5e181-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5e181-130">要求</span><span class="sxs-lookup"><span data-stu-id="5e181-130">Request</span></span>
<span data-ttu-id="5e181-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="5e181-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_schemaextension"
}-->
```http
GET https://graph.microsoft.com/v1.0/schemaExtensions/graphlearn_test
```
##### <a name="response"></a><span data-ttu-id="5e181-132">応答</span><span class="sxs-lookup"><span data-stu-id="5e181-132">Response</span></span>
<span data-ttu-id="5e181-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="5e181-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.schemaExtension"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
    "id":"graphlearn_test",
    "description": "Yet another test schema",
    "targetTypes": [
        "User", "Group"
    ],
    "status": "InDevelopment",
    "owner": "24d3b144-21ae-4080-943f-7067b395b913",
    "properties": [
        {
            "name": "testName",
            "type": "String"
        }
    ]
}
```

## <a name="see-also"></a><span data-ttu-id="5e181-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="5e181-136">See also</span></span>

- [<span data-ttu-id="5e181-137">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="5e181-137">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="5e181-138">スキーマ拡張機能を使用したグループへのカスタム データの追加</span><span class="sxs-lookup"><span data-stu-id="5e181-138">Add custom data to groups using schema extensions</span></span>](../../../concepts/extensibility_schema_groups.md)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get schemaExtension",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->