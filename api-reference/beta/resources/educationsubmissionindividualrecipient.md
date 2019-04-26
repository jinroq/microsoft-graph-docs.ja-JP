---
title: educationSubmissionIndividualRecipient リソースの種類
description: 'educationSubmissionRecipient のサブクラスで、送信がクラス内の個々に割り当てられていることを示します。  '
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: de58dc743cd50f0e31021b4651bb0a3b3b192197
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340556"
---
# <a name="educationsubmissionindividualrecipient-resource-type"></a><span data-ttu-id="52051-103">educationSubmissionIndividualRecipient リソースの種類</span><span class="sxs-lookup"><span data-stu-id="52051-103">educationSubmissionIndividualRecipient resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="52051-104">[educationSubmissionRecipient](educationsubmissionrecipient.md)のサブクラスで、送信がクラス内の個々に割り当てられていることを示します。</span><span class="sxs-lookup"><span data-stu-id="52051-104">A subclass of [educationSubmissionRecipient](educationsubmissionrecipient.md) that indicates that a submission is assigned to an individual in the class.</span></span>  


## <a name="properties"></a><span data-ttu-id="52051-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="52051-105">Properties</span></span>
| <span data-ttu-id="52051-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="52051-106">Property</span></span>     | <span data-ttu-id="52051-107">型</span><span class="sxs-lookup"><span data-stu-id="52051-107">Type</span></span>   |<span data-ttu-id="52051-108">説明</span><span class="sxs-lookup"><span data-stu-id="52051-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="52051-109">userId</span><span class="sxs-lookup"><span data-stu-id="52051-109">userId</span></span>|<span data-ttu-id="52051-110">String</span><span class="sxs-lookup"><span data-stu-id="52051-110">String</span></span>|<span data-ttu-id="52051-111">提出物が割り当てられているユーザーのユーザー ID。</span><span class="sxs-lookup"><span data-stu-id="52051-111">User ID of the user to whom the submission is assigned.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="52051-112">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="52051-112">JSON representation</span></span>

<span data-ttu-id="52051-113">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="52051-113">The following is a JSON representation of the resource.</span></span>

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
