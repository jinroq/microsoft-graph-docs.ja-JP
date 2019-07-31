---
author: daspek
description: contentTypeOrder リソースは、コンテンツ タイプが選択 UI に表示される順序を指定します。
ms.date: 09/13/2017
title: ContentTypeOrder
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 464ac5978f505e74ca99226080c35574917fd550
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973206"
---
# <a name="contenttypeorder-resource-type"></a><span data-ttu-id="9b481-103">ContentTypeOrder リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9b481-103">ContentTypeOrder resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9b481-104">**contentTypeOrder** リソースは、コンテンツ タイプが選択 UI に表示される順序を指定します。</span><span class="sxs-lookup"><span data-stu-id="9b481-104">The **contentTypeOrder** resource specifies in which order the Content Type will appear in the selection UI.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9b481-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9b481-105">JSON representation</span></span>

<span data-ttu-id="9b481-106">以下は、**contentTypeOrder** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="9b481-106">Here is a JSON representation of a **contentTypeOrder** resource.</span></span>
<!-- { "blockType": "resource", "@type": "microsoft.graph.contentTypeOrder", "@type.aka": "oneDrive.contentTypeOrderFacet" } -->

```json
{
  "default": true,
  "position": 2
}
```

## <a name="properties"></a><span data-ttu-id="9b481-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9b481-107">Properties</span></span>

| <span data-ttu-id="9b481-108">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="9b481-108">Property name</span></span> | <span data-ttu-id="9b481-109">種類</span><span class="sxs-lookup"><span data-stu-id="9b481-109">Type</span></span>    | <span data-ttu-id="9b481-110">説明</span><span class="sxs-lookup"><span data-stu-id="9b481-110">Description</span></span>
|:--------------|:--------|:----------------------------------------------------
| <span data-ttu-id="9b481-111">**default**</span><span class="sxs-lookup"><span data-stu-id="9b481-111">**default**</span></span>   | <span data-ttu-id="9b481-112">boolean</span><span class="sxs-lookup"><span data-stu-id="9b481-112">boolean</span></span> | <span data-ttu-id="9b481-113">既定のコンテンツ タイプかどうか。</span><span class="sxs-lookup"><span data-stu-id="9b481-113">Whether this is the default Content Type</span></span>
| <span data-ttu-id="9b481-114">**position**</span><span class="sxs-lookup"><span data-stu-id="9b481-114">**position**</span></span>  | <span data-ttu-id="9b481-115">Int32</span><span class="sxs-lookup"><span data-stu-id="9b481-115">Int32</span></span>   | <span data-ttu-id="9b481-116">コンテンツ タイプが選択 UI で表示される位置を指定します。</span><span class="sxs-lookup"><span data-stu-id="9b481-116">Specifies the position in which the Content Type appears in the selection UI.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ContentTypeOrder",
  "suppressions": []
}
-->
