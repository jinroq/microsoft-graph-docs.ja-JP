# <a name="itemreference-resource-type"></a><span data-ttu-id="6e4e0-101">ItemReference リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6e4e0-101">ItemReference resource type</span></span>

<span data-ttu-id="6e4e0-102">**ItemReference** リソースは、[DriveItem](driveitem.md) を処理するために必要な情報を API を介して提供します。</span><span class="sxs-lookup"><span data-stu-id="6e4e0-102">The **ItemReference** resource provides information necessary to address a [DriveItem](driveitem.md) via the API.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6e4e0-103">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6e4e0-103">JSON representation</span></span>

<span data-ttu-id="6e4e0-104">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="6e4e0-104">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "path", "shareId", "sharepointIds" ],
  "@odata.type": "microsoft.graph.itemReference"
}-->

```json
{
  "driveId": "string",
  "id": "string",
  "name": "string",
  "path": "string",
  "shareId": "string",
  "sharepointIds": { "@odata.type": "microsoft.graph.sharepointIds" }
}
```

## <a name="properties"></a><span data-ttu-id="6e4e0-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6e4e0-105">Properties</span></span>

| <span data-ttu-id="6e4e0-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6e4e0-106">Property</span></span>      | <span data-ttu-id="6e4e0-107">型</span><span class="sxs-lookup"><span data-stu-id="6e4e0-107">Type</span></span>                              | <span data-ttu-id="6e4e0-108">説明</span><span class="sxs-lookup"><span data-stu-id="6e4e0-108">Description</span></span>                                                                                                |
| :------------ | :-------------------------------- | :--------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="6e4e0-109">driveId</span><span class="sxs-lookup"><span data-stu-id="6e4e0-109">driveId</span></span>       | <span data-ttu-id="6e4e0-110">String</span><span class="sxs-lookup"><span data-stu-id="6e4e0-110">String</span></span>                            | <span data-ttu-id="6e4e0-p101">アイテムを含むドライブ インスタンスの一意識別子。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="6e4e0-p101">Unique identifier of the drive instance that contains the item. Read-only.</span></span>                                 |
| <span data-ttu-id="6e4e0-113">id</span><span class="sxs-lookup"><span data-stu-id="6e4e0-113">id</span></span>            | <span data-ttu-id="6e4e0-114">String</span><span class="sxs-lookup"><span data-stu-id="6e4e0-114">String</span></span>                            | <span data-ttu-id="6e4e0-p102">ドライブ内のアイテムの一意識別子。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="6e4e0-p102">Unique identifier of the item in the drive. Read-only.</span></span>                                                     |
| <span data-ttu-id="6e4e0-117">name</span><span class="sxs-lookup"><span data-stu-id="6e4e0-117">name</span></span>          | <span data-ttu-id="6e4e0-118">String</span><span class="sxs-lookup"><span data-stu-id="6e4e0-118">String</span></span>                            | <span data-ttu-id="6e4e0-p103">参照中のアイテムの名前。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="6e4e0-p103">The name of the item being referenced. Read-only.</span></span>                                                          |
| <span data-ttu-id="6e4e0-121">path</span><span class="sxs-lookup"><span data-stu-id="6e4e0-121">path</span></span>          | <span data-ttu-id="6e4e0-122">String</span><span class="sxs-lookup"><span data-stu-id="6e4e0-122">String</span></span>                            | <span data-ttu-id="6e4e0-p104">アイテムへの移動に使用可能なパス。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="6e4e0-p104">Path that can be used to navigate to the item. Read-only.</span></span>                                                  |
| <span data-ttu-id="6e4e0-125">shareId</span><span class="sxs-lookup"><span data-stu-id="6e4e0-125">shareId</span></span>       | <span data-ttu-id="6e4e0-126">String</span><span class="sxs-lookup"><span data-stu-id="6e4e0-126">String</span></span>                            | <span data-ttu-id="6e4e0-127">[共有](../api/shares_get.md) API 経由でアクセスできる共有リソースの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="6e4e0-127">A unique identifier for a shared resource that can be accessed via the [Shares](../api/shares_get.md) API.</span></span> |
| <span data-ttu-id="6e4e0-128">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="6e4e0-128">sharepointIds</span></span> | [<span data-ttu-id="6e4e0-129">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="6e4e0-129">sharepointIds</span></span>](sharepointids.md) | <span data-ttu-id="6e4e0-p105">SharePoint REST 互換性に役立つ識別子を返します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="6e4e0-p105">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>                                   |

## <a name="remarks"></a><span data-ttu-id="6e4e0-132">注釈</span><span class="sxs-lookup"><span data-stu-id="6e4e0-132">Remarks</span></span>

<span data-ttu-id="6e4e0-133">**itemReference** リソースからの **driveItem** を処理するには、次の形式の URL を構築します。</span><span class="sxs-lookup"><span data-stu-id="6e4e0-133">To address a **driveItem** from an **itemReference** resource, construct a URL of the format:</span></span>

```http
GET https://graph.microsoft.com/v1.0/drives/{driveId}/items/{id}
```

<span data-ttu-id="6e4e0-134">**path** の値は、対象ドライブを基準にした API パスです。例: `/drive/root:/Documents/myfile.docx`。</span><span class="sxs-lookup"><span data-stu-id="6e4e0-134">The **path** value is an API path relative to the target drive, for example: `/drive/root:/Documents/myfile.docx`.</span></span>

<span data-ttu-id="6e4e0-135">階層リンクの人が認識できるパスを取得するために、パスの文字列内にある最初の `:` までのすべてを無視しても問題ありません。</span><span class="sxs-lookup"><span data-stu-id="6e4e0-135">To retrieve the human-readable path for a breadcrumb, you can safely ignore everything up to the first `:` in the path string.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "itemReference resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
