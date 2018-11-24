# <a name="list-directoryroles"></a><span data-ttu-id="2c7b5-101">directoryRoles を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="2c7b5-101">List directoryRoles</span></span>

<span data-ttu-id="2c7b5-102">テナントでアクティブになっているディレクトリ ロールを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="2c7b5-102">List the directory roles that are activated in the tenant.</span></span>
## <a name="permissions"></a><span data-ttu-id="2c7b5-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="2c7b5-103">Permissions</span></span>
<span data-ttu-id="2c7b5-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2c7b5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="2c7b5-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2c7b5-106">Permission type</span></span>      | <span data-ttu-id="2c7b5-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="2c7b5-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2c7b5-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2c7b5-108">Delegated (work or school account)</span></span> | <span data-ttu-id="2c7b5-109">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2c7b5-109">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="2c7b5-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2c7b5-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2c7b5-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2c7b5-111">Not supported.</span></span>    |
|<span data-ttu-id="2c7b5-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2c7b5-112">Application</span></span> | <span data-ttu-id="2c7b5-113">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c7b5-113">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2c7b5-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2c7b5-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles
```
## <a name="optional-query-parameters"></a><span data-ttu-id="2c7b5-115">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="2c7b5-115">Optional query parameters</span></span>
<span data-ttu-id="2c7b5-116">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポート**していません** (例: $filter はここではサポートされていません)。</span><span class="sxs-lookup"><span data-stu-id="2c7b5-116">This method does **not** support the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response (e.g. $filter is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="2c7b5-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2c7b5-117">Request headers</span></span>
| <span data-ttu-id="2c7b5-118">名前</span><span class="sxs-lookup"><span data-stu-id="2c7b5-118">Name</span></span>       | <span data-ttu-id="2c7b5-119">型</span><span class="sxs-lookup"><span data-stu-id="2c7b5-119">Type</span></span> | <span data-ttu-id="2c7b5-120">説明</span><span class="sxs-lookup"><span data-stu-id="2c7b5-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="2c7b5-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="2c7b5-121">Authorization</span></span>  | <span data-ttu-id="2c7b5-122">string</span><span class="sxs-lookup"><span data-stu-id="2c7b5-122">string</span></span>  | <span data-ttu-id="2c7b5-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="2c7b5-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2c7b5-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="2c7b5-125">Request body</span></span>
<span data-ttu-id="2c7b5-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="2c7b5-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2c7b5-127">応答</span><span class="sxs-lookup"><span data-stu-id="2c7b5-127">Response</span></span>

<span data-ttu-id="2c7b5-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryRole](../resources/directoryrole.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="2c7b5-128">If successful, this method returns a `200 OK` response code and collection of [directoryRole](../resources/directoryrole.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2c7b5-129">例</span><span class="sxs-lookup"><span data-stu-id="2c7b5-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2c7b5-130">要求</span><span class="sxs-lookup"><span data-stu-id="2c7b5-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_directoryroles"
}-->
```http
GET https://graph.microsoft.com/v1.0/directoryRoles
```
##### <a name="response"></a><span data-ttu-id="2c7b5-131">応答</span><span class="sxs-lookup"><span data-stu-id="2c7b5-131">Response</span></span>
<span data-ttu-id="2c7b5-p103">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="2c7b5-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryRole",
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
      "roleTemplateId": "roleTemplateId-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List directoryRoles",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
