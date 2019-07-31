---
title: educationOneNoteResource リソースの種類
description: 'EducationResource のサブクラス。 OneNote ページの場所を表します。  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 659ca7f55309499314f94ea62e9433c919856dc6
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972650"
---
# <a name="educationonenoteresource-resource-type"></a><span data-ttu-id="6a5d9-104">educationOneNoteResource リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6a5d9-104">educationOneNoteResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6a5d9-105">[EducationResource](educationresource.md)のサブクラス。</span><span class="sxs-lookup"><span data-stu-id="6a5d9-105">A subclass of [educationResource](educationresource.md).</span></span> <span data-ttu-id="6a5d9-106">OneNote ページの場所を表します。</span><span class="sxs-lookup"><span data-stu-id="6a5d9-106">This represents the location of the OneNote page.</span></span>  

## <a name="properties"></a><span data-ttu-id="6a5d9-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6a5d9-107">Properties</span></span>
| <span data-ttu-id="6a5d9-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6a5d9-108">Property</span></span>     | <span data-ttu-id="6a5d9-109">型</span><span class="sxs-lookup"><span data-stu-id="6a5d9-109">Type</span></span>   |<span data-ttu-id="6a5d9-110">説明</span><span class="sxs-lookup"><span data-stu-id="6a5d9-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6a5d9-111">pageUrl</span><span class="sxs-lookup"><span data-stu-id="6a5d9-111">pageUrl</span></span>|<span data-ttu-id="6a5d9-112">String</span><span class="sxs-lookup"><span data-stu-id="6a5d9-112">String</span></span>|<span data-ttu-id="6a5d9-113">OneNote のページへの Microsoft Graph の URL。</span><span class="sxs-lookup"><span data-stu-id="6a5d9-113">The Microsoft Graph URL to the page in OneNote.</span></span>|
|<span data-ttu-id="6a5d9-114">sectionName</span><span class="sxs-lookup"><span data-stu-id="6a5d9-114">sectionName</span></span>|<span data-ttu-id="6a5d9-115">String</span><span class="sxs-lookup"><span data-stu-id="6a5d9-115">String</span></span>|<span data-ttu-id="6a5d9-116">配布先のセクション名を指定します。</span><span class="sxs-lookup"><span data-stu-id="6a5d9-116">Section name that distributions should be copied into or were copied into.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6a5d9-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6a5d9-117">JSON representation</span></span>

<span data-ttu-id="6a5d9-118">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6a5d9-118">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
