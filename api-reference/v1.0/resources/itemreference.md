---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: ItemReference
ms.openlocfilehash: abd8b438e6c4e364a7a4b010d0808255425fa4df
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/28/2017
---
# <a name="itemreference-resource-type"></a><span data-ttu-id="36bf4-102">ItemReference リソース型</span><span class="sxs-lookup"><span data-stu-id="36bf4-102">ItemReference resource type</span></span>

<span data-ttu-id="36bf4-103">**ItemReference** リソースは、[DriveItem](driveitem.md) を処理するために必要な情報を API を介して提供します。</span><span class="sxs-lookup"><span data-stu-id="36bf4-103">The **ItemReference** resource provides information necessary to address a [DriveItem](driveitem.md) via the API.</span></span>

## <a name="json-representation"></a><span data-ttu-id="36bf4-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="36bf4-104">JSON representation</span></span>

<span data-ttu-id="36bf4-105">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="36bf4-105">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "path", "shareId", "sharepointIds" ],
  "@odata.type": "microsoft.graph.itemReference"
}-->

```json
{
  "driveId": "string",
  "driveType": "personal | business | documentLibrary",
  "id": "string",
  "name": "string",
  "path": "string",
  "shareId": "string",
  "sharepointIds": { "@odata.type": "microsoft.graph.sharepointIds" }
}
```

## <a name="properties"></a><span data-ttu-id="36bf4-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="36bf4-106">Properties</span></span>

| <span data-ttu-id="36bf4-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="36bf4-107">Property</span></span>      | <span data-ttu-id="36bf4-108">型</span><span class="sxs-lookup"><span data-stu-id="36bf4-108">Type</span></span>              | <span data-ttu-id="36bf4-109">説明</span><span class="sxs-lookup"><span data-stu-id="36bf4-109">Description</span></span>
|:--------------|:------------------|:-----------------------------------------
| <span data-ttu-id="36bf4-110">driveId</span><span class="sxs-lookup"><span data-stu-id="36bf4-110">driveId</span></span>       | <span data-ttu-id="36bf4-111">String</span><span class="sxs-lookup"><span data-stu-id="36bf4-111">String</span></span>            | <span data-ttu-id="36bf4-p101">アイテムを含むドライブ インスタンスの一意識別子。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="36bf4-p101">Unique identifier of the drive instance that contains the item. Read-only.</span></span>
| <span data-ttu-id="36bf4-114">driveType</span><span class="sxs-lookup"><span data-stu-id="36bf4-114">driveType</span></span>     | <span data-ttu-id="36bf4-115">String</span><span class="sxs-lookup"><span data-stu-id="36bf4-115">String</span></span>            | <span data-ttu-id="36bf4-116">ドライブの種類を表します。</span><span class="sxs-lookup"><span data-stu-id="36bf4-116">Identifies the type of form region.</span></span> <span data-ttu-id="36bf4-117">値については [drive][] リソースを参照してください。</span><span class="sxs-lookup"><span data-stu-id="36bf4-117">See [drive][] resource for values.</span></span>
| <span data-ttu-id="36bf4-118">id</span><span class="sxs-lookup"><span data-stu-id="36bf4-118">id</span></span>            | <span data-ttu-id="36bf4-119">String</span><span class="sxs-lookup"><span data-stu-id="36bf4-119">String</span></span>            | <span data-ttu-id="36bf4-p103">ドライブ内のアイテムの一意識別子。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="36bf4-p103">Unique identifier of the item in the drive. Read-only.</span></span>
| <span data-ttu-id="36bf4-122">name</span><span class="sxs-lookup"><span data-stu-id="36bf4-122">name</span></span>          | <span data-ttu-id="36bf4-123">String</span><span class="sxs-lookup"><span data-stu-id="36bf4-123">String</span></span>            | <span data-ttu-id="36bf4-p104">参照中のアイテムの名前。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="36bf4-p104">The name of the item being referenced. Read-only.</span></span>
| <span data-ttu-id="36bf4-126">path</span><span class="sxs-lookup"><span data-stu-id="36bf4-126">path</span></span>          | <span data-ttu-id="36bf4-127">String</span><span class="sxs-lookup"><span data-stu-id="36bf4-127">String</span></span>            | <span data-ttu-id="36bf4-p105">アイテムへの移動に使用可能なパス。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="36bf4-p105">Path that can be used to navigate to the item. Read-only.</span></span>
| <span data-ttu-id="36bf4-130">shareId</span><span class="sxs-lookup"><span data-stu-id="36bf4-130">shareId</span></span>       | <span data-ttu-id="36bf4-131">String</span><span class="sxs-lookup"><span data-stu-id="36bf4-131">String</span></span>            | <span data-ttu-id="36bf4-132">[共有][] API 経由でアクセスできる共有リソースの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="36bf4-132">A unique identifier for a shared resource that can be accessed via the [Shares][] API.</span></span>
| <span data-ttu-id="36bf4-133">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="36bf4-133">sharepointIds</span></span> | <span data-ttu-id="36bf4-134">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="36bf4-134">[sharepointIds][]</span></span> | <span data-ttu-id="36bf4-p106">SharePoint REST 互換性に役立つ識別子を返します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="36bf4-p106">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>

[drive]: ../resources/drive.md
[sharepointIds]: ../resources/sharepointids.md
[Shares]: ../api/shares_get.md

## <a name="remarks"></a><span data-ttu-id="36bf4-140">備考</span><span class="sxs-lookup"><span data-stu-id="36bf4-140">Remarks</span></span>

<span data-ttu-id="36bf4-141">**itemReference** リソースからの **driveItem** を処理するには、次の形式の URL を構築します。</span><span class="sxs-lookup"><span data-stu-id="36bf4-141">To address a **driveItem** from an **itemReference** resource, construct a URL of the format:</span></span>

```http
GET https://graph.microsoft.com/v1.0/drives/{driveId}/items/{id}
```

<span data-ttu-id="36bf4-142">**path** の値は、対象ドライブを基準にした API パスです。例: `/drive/root:/Documents/myfile.docx`。</span><span class="sxs-lookup"><span data-stu-id="36bf4-142">The **path** value is an API path relative to the target drive, for example: `/drive/root:/Documents/myfile.docx`.</span></span>

<span data-ttu-id="36bf4-143">階層リンクの人が認識できるパスを取得するために、パスの文字列内にある最初の `:` までのすべてを無視しても問題ありません。</span><span class="sxs-lookup"><span data-stu-id="36bf4-143">To retrieve the human-readable path for a breadcrumb, you can safely ignore everything up to the first `:` in the path string.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ItemReference returns a pointer to another item.",
  "section": "documentation",
  "tocPath": "Resources/ItemReference"
} -->
