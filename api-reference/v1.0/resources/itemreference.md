---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: ItemReference
localization_priority: Normal
ms.openlocfilehash: 068e6420344cfa384972abe31157b3306f5b2a4f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27862217"
---
# <a name="itemreference-resource-type"></a><span data-ttu-id="3cbc6-102">ItemReference リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3cbc6-102">ItemReference resource type</span></span>

<span data-ttu-id="3cbc6-103">**ItemReference** リソースは、[DriveItem](driveitem.md) を処理するために必要な情報を API を介して提供します。</span><span class="sxs-lookup"><span data-stu-id="3cbc6-103">The **ItemReference** resource provides information necessary to address a [DriveItem](driveitem.md) via the API.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3cbc6-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3cbc6-104">JSON representation</span></span>

<span data-ttu-id="3cbc6-105">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="3cbc6-105">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="3cbc6-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3cbc6-106">Properties</span></span>

| <span data-ttu-id="3cbc6-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3cbc6-107">Property</span></span>      | <span data-ttu-id="3cbc6-108">型</span><span class="sxs-lookup"><span data-stu-id="3cbc6-108">Type</span></span>              | <span data-ttu-id="3cbc6-109">説明</span><span class="sxs-lookup"><span data-stu-id="3cbc6-109">Description</span></span>
|:--------------|:------------------|:-----------------------------------------
| <span data-ttu-id="3cbc6-110">driveId</span><span class="sxs-lookup"><span data-stu-id="3cbc6-110">driveId</span></span>       | <span data-ttu-id="3cbc6-111">String</span><span class="sxs-lookup"><span data-stu-id="3cbc6-111">String</span></span>            | <span data-ttu-id="3cbc6-p101">アイテムを含むドライブ インスタンスの一意識別子。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="3cbc6-p101">Unique identifier of the drive instance that contains the item. Read-only.</span></span>
| <span data-ttu-id="3cbc6-114">driveType</span><span class="sxs-lookup"><span data-stu-id="3cbc6-114">driveType</span></span>     | <span data-ttu-id="3cbc6-115">String</span><span class="sxs-lookup"><span data-stu-id="3cbc6-115">String</span></span>            | <span data-ttu-id="3cbc6-116">ドライブの種類を表します。</span><span class="sxs-lookup"><span data-stu-id="3cbc6-116">Identifies the type of drive.</span></span> <span data-ttu-id="3cbc6-117">値については [drive][] リソースを参照してください。</span><span class="sxs-lookup"><span data-stu-id="3cbc6-117">See [drive][] resource for values.</span></span>
| <span data-ttu-id="3cbc6-118">id</span><span class="sxs-lookup"><span data-stu-id="3cbc6-118">id</span></span>            | <span data-ttu-id="3cbc6-119">String</span><span class="sxs-lookup"><span data-stu-id="3cbc6-119">String</span></span>            | <span data-ttu-id="3cbc6-p103">ドライブ内のアイテムの一意識別子。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="3cbc6-p103">Unique identifier of the item in the drive. Read-only.</span></span>
| <span data-ttu-id="3cbc6-122">name</span><span class="sxs-lookup"><span data-stu-id="3cbc6-122">name</span></span>          | <span data-ttu-id="3cbc6-123">String</span><span class="sxs-lookup"><span data-stu-id="3cbc6-123">String</span></span>            | <span data-ttu-id="3cbc6-p104">参照中のアイテムの名前。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="3cbc6-p104">The name of the item being referenced. Read-only.</span></span>
| <span data-ttu-id="3cbc6-126">path</span><span class="sxs-lookup"><span data-stu-id="3cbc6-126">path</span></span>          | <span data-ttu-id="3cbc6-127">String</span><span class="sxs-lookup"><span data-stu-id="3cbc6-127">String</span></span>            | <span data-ttu-id="3cbc6-p105">アイテムへの移動に使用可能なパス。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="3cbc6-p105">Path that can be used to navigate to the item. Read-only.</span></span>
| <span data-ttu-id="3cbc6-130">shareId</span><span class="sxs-lookup"><span data-stu-id="3cbc6-130">shareId</span></span>       | <span data-ttu-id="3cbc6-131">String</span><span class="sxs-lookup"><span data-stu-id="3cbc6-131">String</span></span>            | <span data-ttu-id="3cbc6-132">[共有][] API 経由でアクセスできる共有リソースの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="3cbc6-132">A unique identifier for a shared resource that can be accessed via the [Shares][] API.</span></span>
| <span data-ttu-id="3cbc6-133">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="3cbc6-133">sharepointIds</span></span> | <span data-ttu-id="3cbc6-134">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="3cbc6-134">[sharepointIds][]</span></span> | <span data-ttu-id="3cbc6-p106">SharePoint REST 互換性に役立つ識別子を返します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="3cbc6-p106">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>

[drive]: ../resources/drive.md
[sharepointIds]: ../resources/sharepointids.md
[共有]: ../api/shares-get.md
[Shares]: ../api/shares-get.md

## <a name="remarks"></a><span data-ttu-id="3cbc6-140">備考</span><span class="sxs-lookup"><span data-stu-id="3cbc6-140">Remarks</span></span>

<span data-ttu-id="3cbc6-141">**itemReference** リソースからの **driveItem** を処理するには、次の形式の URL を構築します。</span><span class="sxs-lookup"><span data-stu-id="3cbc6-141">To address a **driveItem** from an **itemReference** resource, construct a URL of the format:</span></span>

```http
GET https://graph.microsoft.com/v1.0/drives/{driveId}/items/{id}
```

<span data-ttu-id="3cbc6-142">**path** の値は、対象ドライブを基準にした API パスです。例: `/drive/root:/Documents/myfile.docx`。</span><span class="sxs-lookup"><span data-stu-id="3cbc6-142">The **path** value is an API path relative to the target drive, for example: `/drive/root:/Documents/myfile.docx`.</span></span>

<span data-ttu-id="3cbc6-143">階層リンクの人が認識できるパスを取得するために、パスの文字列内にある最初の `:` までのすべてを無視しても問題ありません。</span><span class="sxs-lookup"><span data-stu-id="3cbc6-143">To retrieve the human-readable path for a breadcrumb, you can safely ignore everything up to the first `:` in the path string.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ItemReference returns a pointer to another item.",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/itemreference.md:
      Found potential enums in resource example that weren't defined in a table:(personal,business,documentLibrary) are in resource, but () are in table"
  ],
  "tocPath": "Resources/ItemReference"
} -->
