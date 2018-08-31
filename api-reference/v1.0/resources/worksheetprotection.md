# <a name="worksheetprotection-resource-type"></a><span data-ttu-id="4d99a-101">WorksheetProtection リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4d99a-101">WorksheetProtection resource type</span></span>

<span data-ttu-id="4d99a-102">シート オブジェクトの保護を表します。</span><span class="sxs-lookup"><span data-stu-id="4d99a-102">Represents the protection of a sheet object.</span></span>


## <a name="methods"></a><span data-ttu-id="4d99a-103">メソッド</span><span class="sxs-lookup"><span data-stu-id="4d99a-103">Methods</span></span>

| <span data-ttu-id="4d99a-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="4d99a-104">Method</span></span>           | <span data-ttu-id="4d99a-105">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="4d99a-105">Return Type</span></span>    |<span data-ttu-id="4d99a-106">説明</span><span class="sxs-lookup"><span data-stu-id="4d99a-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4d99a-107">WorksheetProtection を取得する</span><span class="sxs-lookup"><span data-stu-id="4d99a-107">Get WorksheetProtection</span></span>](../api/worksheetprotection_get.md) | [<span data-ttu-id="4d99a-108">WorkbookWorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="4d99a-108">WorkbookWorksheetProtection</span></span>](worksheetprotection.md) |<span data-ttu-id="4d99a-109">worksheetProtection オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="4d99a-109">Read properties and relationships of worksheetProtection object.</span></span>|
|[<span data-ttu-id="4d99a-110">保護</span><span class="sxs-lookup"><span data-stu-id="4d99a-110">Protect</span></span>](../api/worksheetprotection_protect.md)|<span data-ttu-id="4d99a-111">なし</span><span class="sxs-lookup"><span data-stu-id="4d99a-111">None</span></span>|<span data-ttu-id="4d99a-p101">ワークシートを保護します。ワークシートが保護されている場合はスローします。</span><span class="sxs-lookup"><span data-stu-id="4d99a-p101">Protect a worksheet. It throws if the worksheet has been protected.</span></span>|
|[<span data-ttu-id="4d99a-114">保護を解除</span><span class="sxs-lookup"><span data-stu-id="4d99a-114">Unprotect</span></span>](../api/worksheetprotection_unprotect.md)|<span data-ttu-id="4d99a-115">なし</span><span class="sxs-lookup"><span data-stu-id="4d99a-115">None</span></span>|<span data-ttu-id="4d99a-116">ワークシートの保護を解除します。</span><span class="sxs-lookup"><span data-stu-id="4d99a-116">Unprotect a worksheet</span></span>|

## <a name="properties"></a><span data-ttu-id="4d99a-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4d99a-117">Properties</span></span>
| <span data-ttu-id="4d99a-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4d99a-118">Property</span></span>     | <span data-ttu-id="4d99a-119">タイプ</span><span class="sxs-lookup"><span data-stu-id="4d99a-119">Type</span></span>   |<span data-ttu-id="4d99a-120">説明</span><span class="sxs-lookup"><span data-stu-id="4d99a-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4d99a-121">options</span><span class="sxs-lookup"><span data-stu-id="4d99a-121">options</span></span>|[<span data-ttu-id="4d99a-122">WorkbookWorksheetProtectionOptions</span><span class="sxs-lookup"><span data-stu-id="4d99a-122">WorkbookWorksheetProtectionOptions</span></span>](worksheetprotectionoptions.md)|<span data-ttu-id="4d99a-p102">シートの保護のオプション。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="4d99a-p102">Sheet protection options. Read-only.</span></span>|
|<span data-ttu-id="4d99a-125">protected</span><span class="sxs-lookup"><span data-stu-id="4d99a-125">protected</span></span>|<span data-ttu-id="4d99a-126">boolean</span><span class="sxs-lookup"><span data-stu-id="4d99a-126">boolean</span></span>|<span data-ttu-id="4d99a-p103">ワークシートが保護されているかどうかを示します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4d99a-p103">Indicates if the worksheet is protected.  Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4d99a-129">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4d99a-129">JSON representation</span></span>

<span data-ttu-id="4d99a-130">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="4d99a-130">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookWorksheetProtection"
}-->

```json
{
  "protected": true,
  "options": { "@odata.type": "microsoft.graph.workbookWorksheetProtectionOptions" }
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "WorksheetProtection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->