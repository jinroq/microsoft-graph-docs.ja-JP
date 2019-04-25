---
title: educationPowerPointResource リソースの種類
description: 'educationResource のサブクラス。 これは PowerPoint リソースです。 PowerPoint ファイルは、に関連付けられた**fileResource**ディレクトリにアップロードする必要があります。 '
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: b61f210ce0efde36b83632268e12d18d3b96b661
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32542929"
---
# <a name="educationpowerpointresource-resource-type"></a><span data-ttu-id="35e8a-105">educationPowerPointResource リソースの種類</span><span class="sxs-lookup"><span data-stu-id="35e8a-105">educationPowerPointResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="35e8a-106">[educationResource](educationresource.md)のサブクラス。</span><span class="sxs-lookup"><span data-stu-id="35e8a-106">A subclass of [educationResource](educationresource.md).</span></span> <span data-ttu-id="35e8a-107">これは PowerPoint リソースです。</span><span class="sxs-lookup"><span data-stu-id="35e8a-107">This is a PowerPoint resource.</span></span> <span data-ttu-id="35e8a-108">PowerPoint ファイルは、割り当てまたは送信に関連付けられている**fileResource**ディレクトリにアップロードする必要があります。</span><span class="sxs-lookup"><span data-stu-id="35e8a-108">The PowerPoint file must be uploaded in the **fileResource** directory associated with the assignment or submission.</span></span>


## <a name="properties"></a><span data-ttu-id="35e8a-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="35e8a-109">Properties</span></span>
| <span data-ttu-id="35e8a-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="35e8a-110">Property</span></span>     | <span data-ttu-id="35e8a-111">型</span><span class="sxs-lookup"><span data-stu-id="35e8a-111">Type</span></span>   |<span data-ttu-id="35e8a-112">説明</span><span class="sxs-lookup"><span data-stu-id="35e8a-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="35e8a-113">fileUrl</span><span class="sxs-lookup"><span data-stu-id="35e8a-113">fileUrl</span></span>|<span data-ttu-id="35e8a-114">String</span><span class="sxs-lookup"><span data-stu-id="35e8a-114">String</span></span>|<span data-ttu-id="35e8a-115">ディスク上のファイルの場所。</span><span class="sxs-lookup"><span data-stu-id="35e8a-115">Location of the file on disk.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="35e8a-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="35e8a-116">JSON representation</span></span>

<span data-ttu-id="35e8a-117">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="35e8a-117">The following is a JSON representation of the resource.</span></span>

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
