---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: ColumnLink
ms.openlocfilehash: cdae360afb6e626ee481a7e98ed5f90e657203b2
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/21/2018
ms.locfileid: "23265121"
---
# <a name="columnlink-resource-type"></a><span data-ttu-id="6f087-102">ColumnLink リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6f087-102">ColumnLink resource type</span></span>

<span data-ttu-id="6f087-103">[contentType][] の **columnLink** は **columnDefinition** サイトをそのコンテンツ タイプに接続します。</span><span class="sxs-lookup"><span data-stu-id="6f087-103">A **columnLink** on a [contentType][] attaches a site **columnDefinition** to that content type.</span></span>

[contentType]: contentType.md

## <a name="json-representation"></a><span data-ttu-id="6f087-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6f087-105">JSON representation</span></span>

<span data-ttu-id="6f087-106">以下は、**columnLink** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="6f087-106">Here is a JSON representation of a **columnLink** resource.</span></span>
<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.columnLink" } -->

```json
{
  "id": "string",
  "name": "string"
}
```

## <a name="properties"></a><span data-ttu-id="6f087-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6f087-107">Properties</span></span>

| <span data-ttu-id="6f087-108">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="6f087-108">Property name</span></span> | <span data-ttu-id="6f087-109">型</span><span class="sxs-lookup"><span data-stu-id="6f087-109">Type</span></span>   | <span data-ttu-id="6f087-110">説明</span><span class="sxs-lookup"><span data-stu-id="6f087-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="6f087-111">**ID**</span><span class="sxs-lookup"><span data-stu-id="6f087-111">**id**</span></span>        | <span data-ttu-id="6f087-112">文字列</span><span class="sxs-lookup"><span data-stu-id="6f087-112">string</span></span> | <span data-ttu-id="6f087-113">列の一意識別子。</span><span class="sxs-lookup"><span data-stu-id="6f087-113">The unique identifier for the column.</span></span>
| <span data-ttu-id="6f087-114">**name**</span><span class="sxs-lookup"><span data-stu-id="6f087-114">**name**</span></span>      | <span data-ttu-id="6f087-115">文字列</span><span class="sxs-lookup"><span data-stu-id="6f087-115">string</span></span> | <span data-ttu-id="6f087-116">このコンテンツ タイプの列の名前。</span><span class="sxs-lookup"><span data-stu-id="6f087-116">The name of the column  in this content type.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ColumnLink"
} -->
