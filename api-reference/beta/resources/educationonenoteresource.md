---
title: educationOneNoteResource リソースの種類
description: 'educationResource のサブクラス。 OneNote ページの場所を表します。  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 60b0e4647f1a601d3cbe206e264f7d288ee2110c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507197"
---
# <a name="educationonenoteresource-resource-type"></a><span data-ttu-id="731e8-104">educationOneNoteResource リソースの種類</span><span class="sxs-lookup"><span data-stu-id="731e8-104">educationOneNoteResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="731e8-105">[educationResource](educationresource.md)のサブクラス。</span><span class="sxs-lookup"><span data-stu-id="731e8-105">A subclass of [educationResource](educationresource.md).</span></span> <span data-ttu-id="731e8-106">OneNote ページの場所を表します。</span><span class="sxs-lookup"><span data-stu-id="731e8-106">This represents the location of the OneNote page.</span></span>  

## <a name="properties"></a><span data-ttu-id="731e8-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="731e8-107">Properties</span></span>
| <span data-ttu-id="731e8-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="731e8-108">Property</span></span>     | <span data-ttu-id="731e8-109">型</span><span class="sxs-lookup"><span data-stu-id="731e8-109">Type</span></span>   |<span data-ttu-id="731e8-110">説明</span><span class="sxs-lookup"><span data-stu-id="731e8-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="731e8-111">pageUrl</span><span class="sxs-lookup"><span data-stu-id="731e8-111">pageUrl</span></span>|<span data-ttu-id="731e8-112">String</span><span class="sxs-lookup"><span data-stu-id="731e8-112">String</span></span>|<span data-ttu-id="731e8-113">OneNote のページへの Microsoft Graph の URL。</span><span class="sxs-lookup"><span data-stu-id="731e8-113">The Microsoft Graph URL to the page in OneNote.</span></span>|
|<span data-ttu-id="731e8-114">sectionName</span><span class="sxs-lookup"><span data-stu-id="731e8-114">sectionName</span></span>|<span data-ttu-id="731e8-115">String</span><span class="sxs-lookup"><span data-stu-id="731e8-115">String</span></span>|<span data-ttu-id="731e8-116">配布先のセクション名を指定します。</span><span class="sxs-lookup"><span data-stu-id="731e8-116">Section name that distributions should be copied into or were copied into.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="731e8-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="731e8-117">JSON representation</span></span>

<span data-ttu-id="731e8-118">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="731e8-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationOneNoteResource"
}-->

```json
{
  "pageUrl": "String",
  "sectionName": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationOneNoteResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationonenoteresource.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
