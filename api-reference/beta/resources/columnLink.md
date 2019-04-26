---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: ColumnLink
localization_priority: Normal
ms.openlocfilehash: c6fc12dcfaeffcb3cd4fb08a6863611ae33541d5
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341435"
---
# <a name="columnlink-resource-type"></a><span data-ttu-id="76582-102">ColumnLink リソースの種類</span><span class="sxs-lookup"><span data-stu-id="76582-102">ColumnLink resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="76582-103">[contentType][] の **columnLink** は **columnDefinition** サイトをそのコンテンツ タイプに接続します。</span><span class="sxs-lookup"><span data-stu-id="76582-103">A **columnLink** on a [contentType][] attaches a site **columnDefinition** to that content type.</span></span>

[contentType]: contenttype.md

## <a name="json-representation"></a><span data-ttu-id="76582-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="76582-105">JSON representation</span></span>

<span data-ttu-id="76582-106">以下は、**columnLink** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="76582-106">Here is a JSON representation of a **columnLink** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.columnLink" } -->

```json
{
  "id": "string",
  "name": "string"
}
```

## <a name="properties"></a><span data-ttu-id="76582-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="76582-107">Properties</span></span>

| <span data-ttu-id="76582-108">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="76582-108">Property name</span></span> | <span data-ttu-id="76582-109">種類</span><span class="sxs-lookup"><span data-stu-id="76582-109">Type</span></span>   | <span data-ttu-id="76582-110">説明</span><span class="sxs-lookup"><span data-stu-id="76582-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="76582-111">**id**</span><span class="sxs-lookup"><span data-stu-id="76582-111">**id**</span></span>        | <span data-ttu-id="76582-112">string</span><span class="sxs-lookup"><span data-stu-id="76582-112">string</span></span> | <span data-ttu-id="76582-113">列の一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="76582-113">The unique identifier for the column.</span></span>
| <span data-ttu-id="76582-114">**name**</span><span class="sxs-lookup"><span data-stu-id="76582-114">**name**</span></span>      | <span data-ttu-id="76582-115">string</span><span class="sxs-lookup"><span data-stu-id="76582-115">string</span></span> | <span data-ttu-id="76582-116">このコンテンツ タイプの列の名前。</span><span class="sxs-lookup"><span data-stu-id="76582-116">The name of the column  in this content type.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ColumnLink",
  "suppressions": []
}
-->
