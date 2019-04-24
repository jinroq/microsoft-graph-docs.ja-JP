---
title: educationSubmissionIndividualRecipient リソースの種類
description: 'educationSubmissionRecipient のサブクラスで、送信がクラス内の個々に割り当てられていることを示します。  '
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 8660ec569362d8170d15de86073c0ef59c9ec0a0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507061"
---
# <a name="educationsubmissionindividualrecipient-resource-type"></a><span data-ttu-id="6be15-103">educationSubmissionIndividualRecipient リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6be15-103">educationSubmissionIndividualRecipient resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6be15-104">[educationSubmissionRecipient](educationsubmissionrecipient.md)のサブクラスで、送信がクラス内の個々に割り当てられていることを示します。</span><span class="sxs-lookup"><span data-stu-id="6be15-104">A subclass of [educationSubmissionRecipient](educationsubmissionrecipient.md) that indicates that a submission is assigned to an individual in the class.</span></span>  


## <a name="properties"></a><span data-ttu-id="6be15-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6be15-105">Properties</span></span>
| <span data-ttu-id="6be15-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6be15-106">Property</span></span>     | <span data-ttu-id="6be15-107">型</span><span class="sxs-lookup"><span data-stu-id="6be15-107">Type</span></span>   |<span data-ttu-id="6be15-108">説明</span><span class="sxs-lookup"><span data-stu-id="6be15-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6be15-109">userId</span><span class="sxs-lookup"><span data-stu-id="6be15-109">userId</span></span>|<span data-ttu-id="6be15-110">String</span><span class="sxs-lookup"><span data-stu-id="6be15-110">String</span></span>|<span data-ttu-id="6be15-111">提出物が割り当てられているユーザーのユーザー ID。</span><span class="sxs-lookup"><span data-stu-id="6be15-111">User ID of the user to whom the submission is assigned.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6be15-112">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6be15-112">JSON representation</span></span>

<span data-ttu-id="6be15-113">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6be15-113">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSubmissionIndividualRecipient"
}-->

```json
{
  "userId": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationSubmissionIndividualRecipient resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationsubmissionindividualrecipient.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
