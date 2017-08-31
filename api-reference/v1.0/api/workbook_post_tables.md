# <a name="create-table"></a><span data-ttu-id="eeb01-101">テーブルを作成する</span><span class="sxs-lookup"><span data-stu-id="eeb01-101">Create Table</span></span>

<span data-ttu-id="eeb01-102">この API を使用して、新しいテーブルを作成します。</span><span class="sxs-lookup"><span data-stu-id="eeb01-102">Use this API to create a new Table.</span></span>
## <a name="permissions"></a><span data-ttu-id="eeb01-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="eeb01-103">Permissions</span></span>
<span data-ttu-id="eeb01-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="eeb01-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="eeb01-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="eeb01-106">Permission type</span></span>      | <span data-ttu-id="eeb01-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="eeb01-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eeb01-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="eeb01-108">Delegated (work or school account)</span></span> | <span data-ttu-id="eeb01-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="eeb01-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="eeb01-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="eeb01-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eeb01-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="eeb01-111">Not supported.</span></span>    |
|<span data-ttu-id="eeb01-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="eeb01-112">Application</span></span> | <span data-ttu-id="eeb01-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="eeb01-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="eeb01-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="eeb01-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/$/add

```
## <a name="request-headers"></a><span data-ttu-id="eeb01-115">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="eeb01-115">Request headers</span></span>
| <span data-ttu-id="eeb01-116">名前</span><span class="sxs-lookup"><span data-stu-id="eeb01-116">Name</span></span>       | <span data-ttu-id="eeb01-117">説明</span><span class="sxs-lookup"><span data-stu-id="eeb01-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="eeb01-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="eeb01-118">Authorization</span></span>  | <span data-ttu-id="eeb01-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="eeb01-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="eeb01-121">要求本文</span><span class="sxs-lookup"><span data-stu-id="eeb01-121">Request body</span></span>
<span data-ttu-id="eeb01-122">要求本文で、[テーブル](../resources/table.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="eeb01-122">In the request body, supply a JSON representation of [Table](../resources/table.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="eeb01-123">応答</span><span class="sxs-lookup"><span data-stu-id="eeb01-123">Response</span></span>

<span data-ttu-id="eeb01-124">成功した場合、このメソッドは `201, Created` 応答コードと、応答本文で[テーブル](../resources/table.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="eeb01-124">If successful, this method returns `201, Created` response code and [Table](../resources/table.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eeb01-125">例</span><span class="sxs-lookup"><span data-stu-id="eeb01-125">Example</span></span>
##### <a name="request"></a><span data-ttu-id="eeb01-126">要求</span><span class="sxs-lookup"><span data-stu-id="eeb01-126">Request</span></span>
<span data-ttu-id="eeb01-127">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="eeb01-127">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_table_from_workbook"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/$/add
Content-type: application/json
Content-length: 109

{
  "id": 99,
  "name": "name-value",
  "showHeaders": true,
  "showTotals": true,
  "style": "style-value"
}
```
<span data-ttu-id="eeb01-128">要求本文で、[テーブル](../resources/table.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="eeb01-128">In the request body, supply a JSON representation of [Table](../resources/table.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="eeb01-129">応答</span><span class="sxs-lookup"><span data-stu-id="eeb01-129">Response</span></span>
<span data-ttu-id="eeb01-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="eeb01-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
