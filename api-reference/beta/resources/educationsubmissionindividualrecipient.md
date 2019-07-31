---
title: educationSubmissionIndividualRecipient リソースの種類
description: 'EducationSubmissionRecipient のサブクラスで、送信がクラス内の個々に割り当てられていることを示します。  '
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 2eecdc7e7ddd30ecad9a520b42cd11df9565fa71
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972510"
---
# <a name="educationsubmissionindividualrecipient-resource-type"></a><span data-ttu-id="e67f0-103">educationSubmissionIndividualRecipient リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e67f0-103">educationSubmissionIndividualRecipient resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e67f0-104">[EducationSubmissionRecipient](educationsubmissionrecipient.md)のサブクラスで、送信がクラス内の個々に割り当てられていることを示します。</span><span class="sxs-lookup"><span data-stu-id="e67f0-104">A subclass of [educationSubmissionRecipient](educationsubmissionrecipient.md) that indicates that a submission is assigned to an individual in the class.</span></span>  


## <a name="properties"></a><span data-ttu-id="e67f0-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e67f0-105">Properties</span></span>
| <span data-ttu-id="e67f0-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e67f0-106">Property</span></span>     | <span data-ttu-id="e67f0-107">型</span><span class="sxs-lookup"><span data-stu-id="e67f0-107">Type</span></span>   |<span data-ttu-id="e67f0-108">説明</span><span class="sxs-lookup"><span data-stu-id="e67f0-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e67f0-109">userId</span><span class="sxs-lookup"><span data-stu-id="e67f0-109">userId</span></span>|<span data-ttu-id="e67f0-110">String</span><span class="sxs-lookup"><span data-stu-id="e67f0-110">String</span></span>|<span data-ttu-id="e67f0-111">提出物が割り当てられているユーザーのユーザー ID。</span><span class="sxs-lookup"><span data-stu-id="e67f0-111">User ID of the user to whom the submission is assigned.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e67f0-112">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e67f0-112">JSON representation</span></span>

<span data-ttu-id="e67f0-113">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e67f0-113">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
