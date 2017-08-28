# <a name="get-contract"></a><span data-ttu-id="43dbf-101">契約書を取得する</span><span class="sxs-lookup"><span data-stu-id="43dbf-101">Get Contract</span></span>

<span data-ttu-id="43dbf-102">[契約](../resources/contract.md)オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="43dbf-102">Retrieve the properties and relationships of [contract](../resources/contract.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="43dbf-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="43dbf-103">Permissions</span></span>

<span data-ttu-id="43dbf-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="43dbf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="43dbf-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="43dbf-106">Permission type</span></span>      | <span data-ttu-id="43dbf-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="43dbf-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="43dbf-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="43dbf-108">Delegated (work or school account)</span></span> | <span data-ttu-id="43dbf-109">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="43dbf-109">One of the following scopes is required to execute this API: Directory.Read.All; Directory.ReadWrite.All; Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="43dbf-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="43dbf-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="43dbf-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="43dbf-111">Not supported.</span></span>    |
|<span data-ttu-id="43dbf-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="43dbf-112">Application</span></span> | <span data-ttu-id="43dbf-113">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43dbf-113">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="43dbf-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="43dbf-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /contracts/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="43dbf-115">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="43dbf-115">Optional query parameters</span></span>

<span data-ttu-id="43dbf-116">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](http://graph.microsoft.io/docs/overview/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="43dbf-116">This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="43dbf-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="43dbf-117">Request headers</span></span>

| <span data-ttu-id="43dbf-118">名前</span><span class="sxs-lookup"><span data-stu-id="43dbf-118">Name</span></span>      |<span data-ttu-id="43dbf-119">説明</span><span class="sxs-lookup"><span data-stu-id="43dbf-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="43dbf-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="43dbf-120">Authorization</span></span>  | <span data-ttu-id="43dbf-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="43dbf-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="43dbf-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="43dbf-123">Request body</span></span>

<span data-ttu-id="43dbf-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="43dbf-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="43dbf-125">応答</span><span class="sxs-lookup"><span data-stu-id="43dbf-125">Response</span></span>

<span data-ttu-id="43dbf-126">成功した場合、このメソッドは応答本文で `200 OK` 応答コードと [Contract](../resources/contract.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="43dbf-126">If successful, this method returns a `200 OK` response code and [Contract](../resources/contract.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="43dbf-127">例</span><span class="sxs-lookup"><span data-stu-id="43dbf-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="43dbf-128">要求</span><span class="sxs-lookup"><span data-stu-id="43dbf-128">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_contract"
}-->
```http
GET https://graph.microsoft.com/v1.0/contracts/{id}
```

##### <a name="response"></a><span data-ttu-id="43dbf-129">応答</span><span class="sxs-lookup"><span data-stu-id="43dbf-129">Response</span></span>
<span data-ttu-id="43dbf-p103">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="43dbf-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.Contract"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 186

{
  "contractType": "contractType-value",
  "customerId": "customerId-value",
  "defaultDomainName": "defaultDomainName-value",
  "displayName": "displayName-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get Contract",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->