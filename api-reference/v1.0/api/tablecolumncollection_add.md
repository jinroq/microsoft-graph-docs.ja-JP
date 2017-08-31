# <a name="tablecolumncollection-add"></a><span data-ttu-id="72cf2-101">TableColumnCollection: 追加</span><span class="sxs-lookup"><span data-stu-id="72cf2-101">TableColumnCollection: add</span></span>

<span data-ttu-id="72cf2-102">テーブルに新しい列を追加します。</span><span class="sxs-lookup"><span data-stu-id="72cf2-102">Adds a new column to the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="72cf2-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="72cf2-103">Permissions</span></span>
<span data-ttu-id="72cf2-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="72cf2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="72cf2-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="72cf2-106">Permission type</span></span>      | <span data-ttu-id="72cf2-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="72cf2-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="72cf2-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="72cf2-108">Delegated (work or school account)</span></span> | <span data-ttu-id="72cf2-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="72cf2-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="72cf2-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="72cf2-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="72cf2-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="72cf2-111">Not supported.</span></span>    |
|<span data-ttu-id="72cf2-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="72cf2-112">Application</span></span> | <span data-ttu-id="72cf2-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="72cf2-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="72cf2-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="72cf2-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/add
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/add

```
## <a name="request-headers"></a><span data-ttu-id="72cf2-115">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="72cf2-115">Request headers</span></span>
| <span data-ttu-id="72cf2-116">名前</span><span class="sxs-lookup"><span data-stu-id="72cf2-116">Name</span></span>       | <span data-ttu-id="72cf2-117">説明</span><span class="sxs-lookup"><span data-stu-id="72cf2-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="72cf2-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="72cf2-118">Authorization</span></span>  | <span data-ttu-id="72cf2-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="72cf2-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="72cf2-121">要求本文</span><span class="sxs-lookup"><span data-stu-id="72cf2-121">Request body</span></span>
<span data-ttu-id="72cf2-122">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="72cf2-122">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="72cf2-123">パラメーター</span><span class="sxs-lookup"><span data-stu-id="72cf2-123">Parameter</span></span>    | <span data-ttu-id="72cf2-124">型</span><span class="sxs-lookup"><span data-stu-id="72cf2-124">Type</span></span>   |<span data-ttu-id="72cf2-125">説明</span><span class="sxs-lookup"><span data-stu-id="72cf2-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="72cf2-126">index</span><span class="sxs-lookup"><span data-stu-id="72cf2-126">index</span></span>|<span data-ttu-id="72cf2-127">number</span><span class="sxs-lookup"><span data-stu-id="72cf2-127">number</span></span>|<span data-ttu-id="72cf2-p103">新しい列の相対位置を指定します。この位置の前の列は右にシフトされます。インデックス値は、最後の列のインデックス値と等しいか、小さくなります。そのため、テーブルの末尾に列を追加するためには使用できません。0 を起点とする番号になります。</span><span class="sxs-lookup"><span data-stu-id="72cf2-p103">Specifies the relative position of the new column. The previous column at this position is shifted to the right. The index value should be equal to or less than the last column's index value, so it cannot be used to append a column at the end of the table. Zero-indexed.</span></span>|
|<span data-ttu-id="72cf2-132">values</span><span class="sxs-lookup"><span data-stu-id="72cf2-132">values</span></span>|<span data-ttu-id="72cf2-133">(boolean、string、または number)</span><span class="sxs-lookup"><span data-stu-id="72cf2-133">(boolean or string or number)</span></span>|<span data-ttu-id="72cf2-p104">省略可能。テーブルの列の、書式設定されていない値の 2 次元の配列。</span><span class="sxs-lookup"><span data-stu-id="72cf2-p104">Optional. A 2-dimensional array of unformatted values of the table column.</span></span>|

## <a name="response"></a><span data-ttu-id="72cf2-136">応答</span><span class="sxs-lookup"><span data-stu-id="72cf2-136">Response</span></span>

<span data-ttu-id="72cf2-137">成功した場合、このメソッドは `200, OK` 応答コードと、応答本文で [TableColumn](../resources/tablecolumn.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="72cf2-137">If successful, this method returns `200, OK` response code and [TableColumn](../resources/tablecolumn.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="72cf2-138">例</span><span class="sxs-lookup"><span data-stu-id="72cf2-138">Example</span></span>
<span data-ttu-id="72cf2-139">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="72cf2-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="72cf2-140">要求</span><span class="sxs-lookup"><span data-stu-id="72cf2-140">Request</span></span>
<span data-ttu-id="72cf2-141">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="72cf2-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablecolumncollection_add"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns/add
Content-type: application/json
Content-length: 51

{
  "index": {
  },
  "values": [
    {
    }
  ]
}
```

##### <a name="response"></a><span data-ttu-id="72cf2-142">応答</span><span class="sxs-lookup"><span data-stu-id="72cf2-142">Response</span></span>
<span data-ttu-id="72cf2-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="72cf2-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tableColumn"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 81

{
  "id": 99,
  "name": "name-value",
  "index": 99,
  "values": "values-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "TableColumnCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->