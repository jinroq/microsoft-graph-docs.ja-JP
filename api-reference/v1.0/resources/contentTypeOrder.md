---
author: daspek
ms.author: dspektor
ms.date: 09/13/2017
title: ContentTypeOrder
localization_priority: Normal
description: contentTypeOrder リソースは、コンテンツ タイプが選択 UI に表示される順序を指定します。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 5c77f2dd3763199fea8f0a1377a1b46f8aa4881d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36032838"
---
# <a name="contenttypeorder-resource-type"></a><span data-ttu-id="cf386-103">ContentTypeOrder リソースの種類</span><span class="sxs-lookup"><span data-stu-id="cf386-103">ContentTypeOrder resource type</span></span>

<span data-ttu-id="cf386-104">**contentTypeOrder** リソースは、コンテンツ タイプが選択 UI に表示される順序を指定します。</span><span class="sxs-lookup"><span data-stu-id="cf386-104">The **contentTypeOrder** resource specifies in which order the Content Type will appear in the selection UI.</span></span>

## <a name="json-representation"></a><span data-ttu-id="cf386-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="cf386-105">JSON representation</span></span>

<span data-ttu-id="cf386-106">以下は、**contentTypeOrder** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="cf386-106">Here is a JSON representation of a **contentTypeOrder** resource.</span></span>
<!-- { "blockType": "resource", "@type": "microsoft.graph.contentTypeOrder", "@type.aka": "oneDrive.contentTypeOrderFacet" } -->

```json
{
  "default": true,
  "position": 2
}
```

## <a name="properties"></a><span data-ttu-id="cf386-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cf386-107">Properties</span></span>

| <span data-ttu-id="cf386-108">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="cf386-108">Property name</span></span> | <span data-ttu-id="cf386-109">種類</span><span class="sxs-lookup"><span data-stu-id="cf386-109">Type</span></span>    | <span data-ttu-id="cf386-110">説明</span><span class="sxs-lookup"><span data-stu-id="cf386-110">Description</span></span>
|:--------------|:--------|:----------------------------------------------------
| <span data-ttu-id="cf386-111">**default**</span><span class="sxs-lookup"><span data-stu-id="cf386-111">**default**</span></span>   | <span data-ttu-id="cf386-112">boolean</span><span class="sxs-lookup"><span data-stu-id="cf386-112">boolean</span></span> | <span data-ttu-id="cf386-113">既定のコンテンツ タイプかどうか。</span><span class="sxs-lookup"><span data-stu-id="cf386-113">Whether this is the default Content Type</span></span>
| <span data-ttu-id="cf386-114">**position**</span><span class="sxs-lookup"><span data-stu-id="cf386-114">**position**</span></span>  | <span data-ttu-id="cf386-115">Int32</span><span class="sxs-lookup"><span data-stu-id="cf386-115">Int32</span></span>   | <span data-ttu-id="cf386-116">コンテンツ タイプが選択 UI で表示される位置を指定します。</span><span class="sxs-lookup"><span data-stu-id="cf386-116">Specifies the position in which the Content Type appears in the selection UI.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ContentTypeOrder"
} -->
