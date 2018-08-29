# <a name="worksheetcollection-add"></a><span data-ttu-id="cdd54-101">WorksheetCollection: add</span><span class="sxs-lookup"><span data-stu-id="cdd54-101">WorksheetCollection: add</span></span>

<span data-ttu-id="cdd54-p101">新しいワークシートをブックに追加します。ワークシートは、既存のワークシートの末尾に追加されます。新しく追加したワークシートをアクティブにする場合は、そのワークシートに対して ".activate() を呼び出します。</span><span class="sxs-lookup"><span data-stu-id="cdd54-p101">Adds a new worksheet to the workbook. The worksheet will be added at the end of existing worksheets. If you wish to activate the newly added worksheet, call ".activate() on it.</span></span>
## <a name="permissions"></a><span data-ttu-id="cdd54-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="cdd54-105">Permissions</span></span>
<span data-ttu-id="cdd54-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cdd54-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="cdd54-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="cdd54-108">Permission type</span></span>      | <span data-ttu-id="cdd54-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="cdd54-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cdd54-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="cdd54-110">Delegated (work or school account)</span></span> | <span data-ttu-id="cdd54-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cdd54-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="cdd54-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="cdd54-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cdd54-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cdd54-113">Not supported.</span></span>    |
|<span data-ttu-id="cdd54-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="cdd54-114">Application</span></span> | <span data-ttu-id="cdd54-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cdd54-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cdd54-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="cdd54-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/

```
## <a name="request-headers"></a><span data-ttu-id="cdd54-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cdd54-117">Request headers</span></span>
| <span data-ttu-id="cdd54-118">名前</span><span class="sxs-lookup"><span data-stu-id="cdd54-118">Name</span></span>       | <span data-ttu-id="cdd54-119">説明</span><span class="sxs-lookup"><span data-stu-id="cdd54-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="cdd54-120">承認</span><span class="sxs-lookup"><span data-stu-id="cdd54-120">Authorization</span></span>  | <span data-ttu-id="cdd54-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="cdd54-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="cdd54-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="cdd54-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="cdd54-p104">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="cdd54-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="cdd54-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="cdd54-126">Request body</span></span>
<span data-ttu-id="cdd54-127">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="cdd54-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="cdd54-128">パラメーター</span><span class="sxs-lookup"><span data-stu-id="cdd54-128">Parameter</span></span>    | <span data-ttu-id="cdd54-129">型</span><span class="sxs-lookup"><span data-stu-id="cdd54-129">Type</span></span>   |<span data-ttu-id="cdd54-130">説明</span><span class="sxs-lookup"><span data-stu-id="cdd54-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cdd54-131">name</span><span class="sxs-lookup"><span data-stu-id="cdd54-131">name</span></span>|<span data-ttu-id="cdd54-132">文字列</span><span class="sxs-lookup"><span data-stu-id="cdd54-132">string</span></span>|<span data-ttu-id="cdd54-p105">省略可能。追加するワークシートの名前。指定する場合、名前は一意である必要があります。指定されていない場合は、Excel が新しいワークシートの名前を決定します。</span><span class="sxs-lookup"><span data-stu-id="cdd54-p105">Optional. The name of the worksheet to be added. If specified, name should be unqiue. If not specified, Excel determines the name of the new worksheet.</span></span>|

## <a name="response"></a><span data-ttu-id="cdd54-137">応答</span><span class="sxs-lookup"><span data-stu-id="cdd54-137">Response</span></span>

<span data-ttu-id="cdd54-138">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で[WorkbookWorksheet](../resources/worksheet.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="cdd54-138">If successful, this method returns `200 OK` response code and [groupSetting](../resources/worksheet.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cdd54-139">例</span><span class="sxs-lookup"><span data-stu-id="cdd54-139">Example</span></span>
<span data-ttu-id="cdd54-140">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="cdd54-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="cdd54-141">要求</span><span class="sxs-lookup"><span data-stu-id="cdd54-141">Request</span></span>
<span data-ttu-id="cdd54-142">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="cdd54-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "worksheetcollection_add"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/add
Content-type: application/json
Content-length: 26

{
  "name": "name-value"
}
```

##### <a name="response"></a><span data-ttu-id="cdd54-143">応答</span><span class="sxs-lookup"><span data-stu-id="cdd54-143">Response</span></span>
<span data-ttu-id="cdd54-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="cdd54-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookWorksheet"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 100

{
  "id": "id-value",
  "position": 99,
  "name": "name-value",
  "visibility": "visibility-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "WorksheetCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->