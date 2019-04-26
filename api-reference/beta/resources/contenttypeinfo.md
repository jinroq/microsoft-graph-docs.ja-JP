---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: ContentTypeInfo
localization_priority: Normal
ms.openlocfilehash: 107dfb3577489521d2e10e0c8fd2fe52c4f90b10
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341229"
---
# <a name="contenttypeinfo-resource-type"></a><span data-ttu-id="92113-102">ContentTypeInfo リソースの種類</span><span class="sxs-lookup"><span data-stu-id="92113-102">ContentTypeInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="92113-103">**ContentTypeInfo** リソースは、アイテムの SharePoint でのコンテンツ タイプを示します。</span><span class="sxs-lookup"><span data-stu-id="92113-103">The **contentTypeInfo** resource indicates the SharePoint content type of an item.</span></span>

## <a name="json-representation"></a><span data-ttu-id="92113-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="92113-104">JSON representation</span></span>

<span data-ttu-id="92113-105">以下は、**contentTypeInfo** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="92113-105">Here is a JSON representation of a **contentTypeInfo** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.contentTypeInfo", "@type.aka": "oneDrive.contentTypeFacet" } -->

```json
{
  "id": "string",
  "name": "string"
}
```

## <a name="properties"></a><span data-ttu-id="92113-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="92113-106">Properties</span></span>

| <span data-ttu-id="92113-107">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="92113-107">Property name</span></span>  | <span data-ttu-id="92113-108">種類</span><span class="sxs-lookup"><span data-stu-id="92113-108">Type</span></span>    | <span data-ttu-id="92113-109">説明</span><span class="sxs-lookup"><span data-stu-id="92113-109">Description</span></span>
|:---------------|:--------|:--------------------------------------------------
| <span data-ttu-id="92113-110">**id**</span><span class="sxs-lookup"><span data-stu-id="92113-110">**id**</span></span>         | <span data-ttu-id="92113-111">string</span><span class="sxs-lookup"><span data-stu-id="92113-111">string</span></span>  | <span data-ttu-id="92113-112">コンテンツ タイプの ID。</span><span class="sxs-lookup"><span data-stu-id="92113-112">The id of the content type.</span></span>
| <span data-ttu-id="92113-113">**name**</span><span class="sxs-lookup"><span data-stu-id="92113-113">**name**</span></span>       | <span data-ttu-id="92113-114">string</span><span class="sxs-lookup"><span data-stu-id="92113-114">string</span></span>  | <span data-ttu-id="92113-115">コンテンツ タイプの名前。</span><span class="sxs-lookup"><span data-stu-id="92113-115">The name of the content type.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ContentTypeInfo",
  "suppressions": []
}
-->
