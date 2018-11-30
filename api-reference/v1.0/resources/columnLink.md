---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: ColumnLink
ms.openlocfilehash: a3eae28dcd9fef3ddfba9b39103bec31ff71c9da
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27020270"
---
# <a name="columnlink-resource-type"></a><span data-ttu-id="04d76-102">ColumnLink リソースの種類</span><span class="sxs-lookup"><span data-stu-id="04d76-102">ColumnLink resource type</span></span>

<span data-ttu-id="04d76-103">[contentType][] の **columnLink** は **columnDefinition** サイトをそのコンテンツ タイプに接続します。</span><span class="sxs-lookup"><span data-stu-id="04d76-103">A **columnLink** on a [contentType][] attaches a site **columnDefinition** to that content type.</span></span>

[contentType]: contenttype.md

## <a name="json-representation"></a><span data-ttu-id="04d76-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="04d76-105">JSON representation</span></span>

<span data-ttu-id="04d76-106">以下は、**columnLink** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="04d76-106">Here is a JSON representation of a **columnLink** resource.</span></span>
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

## <a name="properties"></a><span data-ttu-id="04d76-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="04d76-107">Properties</span></span>

| <span data-ttu-id="04d76-108">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="04d76-108">Property name</span></span> | <span data-ttu-id="04d76-109">種類</span><span class="sxs-lookup"><span data-stu-id="04d76-109">Type</span></span>   | <span data-ttu-id="04d76-110">説明</span><span class="sxs-lookup"><span data-stu-id="04d76-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="04d76-111">**id**</span><span class="sxs-lookup"><span data-stu-id="04d76-111">**id**</span></span>        | <span data-ttu-id="04d76-112">string</span><span class="sxs-lookup"><span data-stu-id="04d76-112">string</span></span> | <span data-ttu-id="04d76-113">列の一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="04d76-113">The unique identifier for the column.</span></span>
| <span data-ttu-id="04d76-114">**name**</span><span class="sxs-lookup"><span data-stu-id="04d76-114">**name**</span></span>      | <span data-ttu-id="04d76-115">string</span><span class="sxs-lookup"><span data-stu-id="04d76-115">string</span></span> | <span data-ttu-id="04d76-116">このコンテンツ タイプの列の名前。</span><span class="sxs-lookup"><span data-stu-id="04d76-116">The name of the column  in this content type.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ColumnLink"
} -->
