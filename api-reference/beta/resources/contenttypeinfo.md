---
author: daspek
description: ContentTypeInfo リソースは、アイテムの SharePoint でのコンテンツ タイプを示します。
ms.date: 09/12/2017
title: ContentTypeInfo
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 04316b01c905acb4fe38923f8d664ea892773e8e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36012850"
---
# <a name="contenttypeinfo-resource-type"></a><span data-ttu-id="0f4af-103">ContentTypeInfo リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0f4af-103">ContentTypeInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0f4af-104">**ContentTypeInfo** リソースは、アイテムの SharePoint でのコンテンツ タイプを示します。</span><span class="sxs-lookup"><span data-stu-id="0f4af-104">The **contentTypeInfo** resource indicates the SharePoint content type of an item.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0f4af-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0f4af-105">JSON representation</span></span>

<span data-ttu-id="0f4af-106">以下は、**contentTypeInfo** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0f4af-106">Here is a JSON representation of a **contentTypeInfo** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.contentTypeInfo", "@type.aka": "oneDrive.contentTypeFacet" } -->

```json
{
  "id": "string",
  "name": "string"
}
```

## <a name="properties"></a><span data-ttu-id="0f4af-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0f4af-107">Properties</span></span>

| <span data-ttu-id="0f4af-108">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="0f4af-108">Property name</span></span>  | <span data-ttu-id="0f4af-109">種類</span><span class="sxs-lookup"><span data-stu-id="0f4af-109">Type</span></span>    | <span data-ttu-id="0f4af-110">説明</span><span class="sxs-lookup"><span data-stu-id="0f4af-110">Description</span></span>
|:---------------|:--------|:--------------------------------------------------
| <span data-ttu-id="0f4af-111">**id**</span><span class="sxs-lookup"><span data-stu-id="0f4af-111">**id**</span></span>         | <span data-ttu-id="0f4af-112">string</span><span class="sxs-lookup"><span data-stu-id="0f4af-112">string</span></span>  | <span data-ttu-id="0f4af-113">コンテンツ タイプの ID。</span><span class="sxs-lookup"><span data-stu-id="0f4af-113">The id of the content type.</span></span>
| <span data-ttu-id="0f4af-114">**name**</span><span class="sxs-lookup"><span data-stu-id="0f4af-114">**name**</span></span>       | <span data-ttu-id="0f4af-115">string</span><span class="sxs-lookup"><span data-stu-id="0f4af-115">string</span></span>  | <span data-ttu-id="0f4af-116">コンテンツ タイプの名前。</span><span class="sxs-lookup"><span data-stu-id="0f4af-116">The name of the content type.</span></span>

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
