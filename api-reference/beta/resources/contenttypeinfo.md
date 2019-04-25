---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: ContentTypeInfo
localization_priority: Normal
ms.openlocfilehash: 196a71be06b4e3c02330aba21559341650caa550
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535403"
---
# <a name="contenttypeinfo-resource-type"></a><span data-ttu-id="b5caa-102">ContentTypeInfo リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b5caa-102">ContentTypeInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b5caa-103">**ContentTypeInfo** リソースは、アイテムの SharePoint でのコンテンツ タイプを示します。</span><span class="sxs-lookup"><span data-stu-id="b5caa-103">The **contentTypeInfo** resource indicates the SharePoint content type of an item.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b5caa-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b5caa-104">JSON representation</span></span>

<span data-ttu-id="b5caa-105">以下は、**contentTypeInfo** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b5caa-105">Here is a JSON representation of a **contentTypeInfo** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.contentTypeInfo", "@type.aka": "oneDrive.contentTypeFacet" } -->

```json
{
  "id": "string",
  "name": "string"
}
```

## <a name="properties"></a><span data-ttu-id="b5caa-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b5caa-106">Properties</span></span>

| <span data-ttu-id="b5caa-107">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="b5caa-107">Property name</span></span>  | <span data-ttu-id="b5caa-108">種類</span><span class="sxs-lookup"><span data-stu-id="b5caa-108">Type</span></span>    | <span data-ttu-id="b5caa-109">説明</span><span class="sxs-lookup"><span data-stu-id="b5caa-109">Description</span></span>
|:---------------|:--------|:--------------------------------------------------
| <span data-ttu-id="b5caa-110">**id**</span><span class="sxs-lookup"><span data-stu-id="b5caa-110">**id**</span></span>         | <span data-ttu-id="b5caa-111">string</span><span class="sxs-lookup"><span data-stu-id="b5caa-111">string</span></span>  | <span data-ttu-id="b5caa-112">コンテンツ タイプの ID。</span><span class="sxs-lookup"><span data-stu-id="b5caa-112">The id of the content type.</span></span>
| <span data-ttu-id="b5caa-113">**name**</span><span class="sxs-lookup"><span data-stu-id="b5caa-113">**name**</span></span>       | <span data-ttu-id="b5caa-114">string</span><span class="sxs-lookup"><span data-stu-id="b5caa-114">string</span></span>  | <span data-ttu-id="b5caa-115">コンテンツ タイプの名前。</span><span class="sxs-lookup"><span data-stu-id="b5caa-115">The name of the content type.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ContentTypeInfo",
  "suppressions": [
    "Error: /api-reference/beta/resources/contenttypeinfo.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
