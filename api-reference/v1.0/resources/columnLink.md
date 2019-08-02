---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: ColumnLink
localization_priority: Normal
description: contentType の columnLink は columnDefinition サイトをそのコンテンツ タイプに接続します。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: d3914c4b3cfe18d2dead778116b86134caaf6caa
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029695"
---
# <a name="columnlink-resource-type"></a><span data-ttu-id="19bc2-103">ColumnLink リソースの種類</span><span class="sxs-lookup"><span data-stu-id="19bc2-103">ColumnLink resource type</span></span>

<span data-ttu-id="19bc2-104">[contentType][] の **columnLink** は **columnDefinition** サイトをそのコンテンツ タイプに接続します。</span><span class="sxs-lookup"><span data-stu-id="19bc2-104">A **columnLink** on a [contentType][] attaches a site **columnDefinition** to that content type.</span></span>

[contentType]: contenttype.md

## <a name="json-representation"></a><span data-ttu-id="19bc2-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="19bc2-106">JSON representation</span></span>

<span data-ttu-id="19bc2-107">以下は、**columnLink** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="19bc2-107">Here is a JSON representation of a **columnLink** resource.</span></span>
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

## <a name="properties"></a><span data-ttu-id="19bc2-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="19bc2-108">Properties</span></span>

| <span data-ttu-id="19bc2-109">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="19bc2-109">Property name</span></span> | <span data-ttu-id="19bc2-110">種類</span><span class="sxs-lookup"><span data-stu-id="19bc2-110">Type</span></span>   | <span data-ttu-id="19bc2-111">説明</span><span class="sxs-lookup"><span data-stu-id="19bc2-111">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="19bc2-112">**id**</span><span class="sxs-lookup"><span data-stu-id="19bc2-112">**id**</span></span>        | <span data-ttu-id="19bc2-113">string</span><span class="sxs-lookup"><span data-stu-id="19bc2-113">string</span></span> | <span data-ttu-id="19bc2-114">列の一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="19bc2-114">The unique identifier for the column.</span></span>
| <span data-ttu-id="19bc2-115">**name**</span><span class="sxs-lookup"><span data-stu-id="19bc2-115">**name**</span></span>      | <span data-ttu-id="19bc2-116">string</span><span class="sxs-lookup"><span data-stu-id="19bc2-116">string</span></span> | <span data-ttu-id="19bc2-117">このコンテンツ タイプの列の名前。</span><span class="sxs-lookup"><span data-stu-id="19bc2-117">The name of the column  in this content type.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ColumnLink"
} -->
