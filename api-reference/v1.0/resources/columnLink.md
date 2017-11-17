---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: ColumnLink
ms.openlocfilehash: ef7fef6fb6ca35f1117433b452de0841691282a0
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/28/2017
---
# <a name="columnlink-resource-type"></a><span data-ttu-id="62058-102">ColumnLink リソース型</span><span class="sxs-lookup"><span data-stu-id="62058-102">ColumnLink resource type</span></span>

<span data-ttu-id="62058-103">[contentType][] の **columnLink** は **columnDefinition** サイトをそのコンテンツ タイプに接続します。</span><span class="sxs-lookup"><span data-stu-id="62058-103">A **columnLink** on a [contentType][] attaches a site **columnDefinition** to that content type.</span></span>

[contentType]: contentType.md

## <a name="json-representation"></a><span data-ttu-id="62058-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="62058-105">JSON representation</span></span>

<span data-ttu-id="62058-106">以下は、**columnLink** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="62058-106">Here is a JSON representation of a **baseItem** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.columnLink" } -->

```json
{
  "id": "string",
  "name": "string"
}
```

## <a name="properties"></a><span data-ttu-id="62058-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="62058-107">Properties</span></span>

| <span data-ttu-id="62058-108">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="62058-108">Property name</span></span> | <span data-ttu-id="62058-109">種類</span><span class="sxs-lookup"><span data-stu-id="62058-109">Type</span></span>   | <span data-ttu-id="62058-110">説明</span><span class="sxs-lookup"><span data-stu-id="62058-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="62058-111">**id**</span><span class="sxs-lookup"><span data-stu-id="62058-111">**id**</span></span>        | <span data-ttu-id="62058-112">string</span><span class="sxs-lookup"><span data-stu-id="62058-112">string</span></span> | <span data-ttu-id="62058-113">列の一意識別子。</span><span class="sxs-lookup"><span data-stu-id="62058-113">The unique identifier for the column.</span></span>
| <span data-ttu-id="62058-114">**name**</span><span class="sxs-lookup"><span data-stu-id="62058-114">**name**</span></span>      | <span data-ttu-id="62058-115">string</span><span class="sxs-lookup"><span data-stu-id="62058-115">string</span></span> | <span data-ttu-id="62058-116">このコンテンツ タイプの列の名前。</span><span class="sxs-lookup"><span data-stu-id="62058-116">The name of the column  in this content type.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ColumnLink"
} -->
