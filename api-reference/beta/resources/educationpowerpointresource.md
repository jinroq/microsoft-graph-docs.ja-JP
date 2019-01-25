---
title: educationPowerPointResource リソースの種類
description: 'EducationResource のサブクラスです。 これは、PowerPoint のリソースです。 関連付けられている**fileResource**ディレクトリに、PowerPoint ファイルをアップロードする必要があります、 '
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: b61f210ce0efde36b83632268e12d18d3b96b661
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512200"
---
# <a name="educationpowerpointresource-resource-type"></a><span data-ttu-id="7faff-105">educationPowerPointResource リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7faff-105">educationPowerPointResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7faff-106">[EducationResource](educationresource.md)のサブクラスです。</span><span class="sxs-lookup"><span data-stu-id="7faff-106">A subclass of [educationResource](educationresource.md).</span></span> <span data-ttu-id="7faff-107">これは、PowerPoint のリソースです。</span><span class="sxs-lookup"><span data-stu-id="7faff-107">This is a PowerPoint resource.</span></span> <span data-ttu-id="7faff-108">送信または割り当てに関連付けられている**fileResource**ディレクトリには、PowerPoint ファイルをアップロードする必要があります。</span><span class="sxs-lookup"><span data-stu-id="7faff-108">The PowerPoint file must be uploaded in the **fileResource** directory associated with the assignment or submission.</span></span>


## <a name="properties"></a><span data-ttu-id="7faff-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7faff-109">Properties</span></span>
| <span data-ttu-id="7faff-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7faff-110">Property</span></span>     | <span data-ttu-id="7faff-111">型</span><span class="sxs-lookup"><span data-stu-id="7faff-111">Type</span></span>   |<span data-ttu-id="7faff-112">説明</span><span class="sxs-lookup"><span data-stu-id="7faff-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7faff-113">FileURL</span><span class="sxs-lookup"><span data-stu-id="7faff-113">fileUrl</span></span>|<span data-ttu-id="7faff-114">String</span><span class="sxs-lookup"><span data-stu-id="7faff-114">String</span></span>|<span data-ttu-id="7faff-115">ディスク上のファイルの場所です。</span><span class="sxs-lookup"><span data-stu-id="7faff-115">Location of the file on disk.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7faff-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7faff-116">JSON representation</span></span>

<span data-ttu-id="7faff-117">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7faff-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationPowerPointResource"
}-->

```json
{
  "fileUrl": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationPowerPointResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationpowerpointresource.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
