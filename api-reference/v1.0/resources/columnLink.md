---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: ColumnLink
localization_priority: Normal
ms.openlocfilehash: 435696cc596f73830104ea8ec0619bf40a462d62
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32565787"
---
# <a name="columnlink-resource-type"></a><span data-ttu-id="30cb4-102">ColumnLink リソースの種類</span><span class="sxs-lookup"><span data-stu-id="30cb4-102">ColumnLink resource type</span></span>

<span data-ttu-id="30cb4-103">[contentType][] の **columnLink** は **columnDefinition** サイトをそのコンテンツ タイプに接続します。</span><span class="sxs-lookup"><span data-stu-id="30cb4-103">A **columnLink** on a [contentType][] attaches a site **columnDefinition** to that content type.</span></span>

[contentType]: contenttype.md

## <a name="json-representation"></a><span data-ttu-id="30cb4-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="30cb4-105">JSON representation</span></span>

<span data-ttu-id="30cb4-106">以下は、**columnLink** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="30cb4-106">Here is a JSON representation of a **columnLink** resource.</span></span>
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

## <a name="properties"></a><span data-ttu-id="30cb4-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="30cb4-107">Properties</span></span>

| <span data-ttu-id="30cb4-108">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="30cb4-108">Property name</span></span> | <span data-ttu-id="30cb4-109">種類</span><span class="sxs-lookup"><span data-stu-id="30cb4-109">Type</span></span>   | <span data-ttu-id="30cb4-110">説明</span><span class="sxs-lookup"><span data-stu-id="30cb4-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="30cb4-111">**id**</span><span class="sxs-lookup"><span data-stu-id="30cb4-111">**id**</span></span>        | <span data-ttu-id="30cb4-112">string</span><span class="sxs-lookup"><span data-stu-id="30cb4-112">string</span></span> | <span data-ttu-id="30cb4-113">列の一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="30cb4-113">The unique identifier for the column.</span></span>
| <span data-ttu-id="30cb4-114">**name**</span><span class="sxs-lookup"><span data-stu-id="30cb4-114">**name**</span></span>      | <span data-ttu-id="30cb4-115">string</span><span class="sxs-lookup"><span data-stu-id="30cb4-115">string</span></span> | <span data-ttu-id="30cb4-116">このコンテンツ タイプの列の名前。</span><span class="sxs-lookup"><span data-stu-id="30cb4-116">The name of the column  in this content type.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ColumnLink"
} -->
