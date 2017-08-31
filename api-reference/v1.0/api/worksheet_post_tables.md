# <a name="create-table"></a><span data-ttu-id="26770-101">テーブルを作成する</span><span class="sxs-lookup"><span data-stu-id="26770-101">Create Table</span></span>

<span data-ttu-id="26770-102">この API を使用して、新しいテーブルを作成します。</span><span class="sxs-lookup"><span data-stu-id="26770-102">Use this API to create a new Table.</span></span>
## <a name="permissions"></a><span data-ttu-id="26770-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="26770-103">Permissions</span></span>
<span data-ttu-id="26770-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="26770-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="26770-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="26770-106">Permission type</span></span>      | <span data-ttu-id="26770-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="26770-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="26770-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="26770-108">Delegated (work or school account)</span></span> | <span data-ttu-id="26770-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="26770-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="26770-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="26770-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="26770-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="26770-111">Not supported.</span></span>    |
|<span data-ttu-id="26770-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="26770-112">Application</span></span> | <span data-ttu-id="26770-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="26770-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="26770-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="26770-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/tables/add

```
## <a name="request-headers"></a><span data-ttu-id="26770-115">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="26770-115">Request headers</span></span>
| <span data-ttu-id="26770-116">名前</span><span class="sxs-lookup"><span data-stu-id="26770-116">Name</span></span>       | <span data-ttu-id="26770-117">説明</span><span class="sxs-lookup"><span data-stu-id="26770-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="26770-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="26770-118">Authorization</span></span>  | <span data-ttu-id="26770-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="26770-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="26770-121">要求本文</span><span class="sxs-lookup"><span data-stu-id="26770-121">Request body</span></span>
<span data-ttu-id="26770-122">要求本文で次のパラメーターを指定します。</span><span class="sxs-lookup"><span data-stu-id="26770-122">In the request body, supply following parameters.</span></span> 

### <a name="request-parameters"></a><span data-ttu-id="26770-123">要求パラメーター</span><span class="sxs-lookup"><span data-stu-id="26770-123">Request parameters</span></span>
| <span data-ttu-id="26770-124">名前</span><span class="sxs-lookup"><span data-stu-id="26770-124">Name</span></span>           | <span data-ttu-id="26770-125">型</span><span class="sxs-lookup"><span data-stu-id="26770-125">Type</span></span>      |<span data-ttu-id="26770-126">説明</span><span class="sxs-lookup"><span data-stu-id="26770-126">Description</span></span>|
|:---------------|:----------|:----------|
| <span data-ttu-id="26770-127">Address</span><span class="sxs-lookup"><span data-stu-id="26770-127">Address</span></span>  | <span data-ttu-id="26770-128">string</span><span class="sxs-lookup"><span data-stu-id="26770-128">string</span></span>| <span data-ttu-id="26770-p103">範囲のアドレスです。この API を `worksheets/{id or name}/tables/add` パスから呼び出す場合、アドレスにシート名のプレフィックスを指定する必要はありません。ただし、これを `workbook/tables/add` パスから呼び出す場合は、テーブルを作成する必要のあるシート名を指定する必要があります (例: `sheet1!A1:D4`)。</span><span class="sxs-lookup"><span data-stu-id="26770-p103">Range address. If you are calling this API off of `worksheets/{id or name}/tables/add` path, there is no need to for sheet name prefix in the address. However, if you are calling this off of `workbook/tables/add` path, then supply the sheet name on which the table needs to be created (example: `sheet1!A1:D4`)</span></span>|
| <span data-ttu-id="26770-132">hasHeaders</span><span class="sxs-lookup"><span data-stu-id="26770-132">hasHeaders</span></span>  | <span data-ttu-id="26770-133">boolean</span><span class="sxs-lookup"><span data-stu-id="26770-133">boolean</span></span>|<span data-ttu-id="26770-p104">範囲に列ラベルがあるかどうかを示すブール値。ソースにヘッダーが含まれていない場合 (このプロパティが false に設定されている場合)、Excel はデータを下方向に 1 行シフトして、自動的にヘッダーを生成します。</span><span class="sxs-lookup"><span data-stu-id="26770-p104">Boolean value that indicates whether the range has column labels. If the source does not contain headers (i.e,. when this property set to false), Excel will automatically generate header shifting the data down by one row.</span></span>|

## <a name="response"></a><span data-ttu-id="26770-137">応答</span><span class="sxs-lookup"><span data-stu-id="26770-137">Response</span></span>

<span data-ttu-id="26770-138">成功した場合、このメソッドは `201, Created` 応答コードと、応答本文で[テーブル](../resources/table.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="26770-138">If successful, this method returns `201, Created` response code and [Table](../resources/table.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="26770-139">例</span><span class="sxs-lookup"><span data-stu-id="26770-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="26770-140">要求</span><span class="sxs-lookup"><span data-stu-id="26770-140">Request</span></span>
<span data-ttu-id="26770-141">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="26770-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_table_from_worksheet"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/tables/$/add
Content-type: application/json
Content-length: 109

{
  "address": "A1:D8",
  "hasHeaders": false
}
```
##### <a name="response"></a><span data-ttu-id="26770-142">応答</span><span class="sxs-lookup"><span data-stu-id="26770-142">Response</span></span>
<span data-ttu-id="26770-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="26770-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.table"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 109

{
  "id": "99",
  "name": "name-value",
  "showHeaders": true,
  "showTotals": true,
  "style": "style-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Table",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
