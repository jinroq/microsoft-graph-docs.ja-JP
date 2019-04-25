---
title: educationAssignmentIndividualRecipient リソースの種類
description: 'プロパティへの割り当ての中で使用されます。 個別の受信者一覧に設定すると、クラス内の学生が選択されます。 '
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: 736345901faeeb4d3fab4d417752b684f1e19307
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543015"
---
# <a name="educationassignmentindividualrecipient-resource-type"></a><span data-ttu-id="cce3a-104">educationAssignmentIndividualRecipient リソースの種類</span><span class="sxs-lookup"><span data-stu-id="cce3a-104">educationAssignmentIndividualRecipient resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cce3a-105">プロパティへの[割り当て](educationassignment.md)の中で使用されます。</span><span class="sxs-lookup"><span data-stu-id="cce3a-105">Used inside the [assignment.assignTo](educationassignment.md) property.</span></span> <span data-ttu-id="cce3a-106">個別の受信者一覧に設定した場合、クラス内の学生は、割り当てが発行されたときに送信オブジェクトを受け取ります。</span><span class="sxs-lookup"><span data-stu-id="cce3a-106">When set to individual recipient list, selected students in the class will receive a submission object when the assignment is published.</span></span>

<span data-ttu-id="cce3a-107">このリソースは[educationAssignmentRecipient](educationassignmentrecipient.md)のサブクラスです。</span><span class="sxs-lookup"><span data-stu-id="cce3a-107">This resource is a subclass of [educationAssignmentRecipient](educationassignmentrecipient.md).</span></span>

## <a name="properties"></a><span data-ttu-id="cce3a-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cce3a-108">Properties</span></span>
| <span data-ttu-id="cce3a-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cce3a-109">Property</span></span>     | <span data-ttu-id="cce3a-110">型</span><span class="sxs-lookup"><span data-stu-id="cce3a-110">Type</span></span>   |<span data-ttu-id="cce3a-111">説明</span><span class="sxs-lookup"><span data-stu-id="cce3a-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cce3a-112">recipients</span><span class="sxs-lookup"><span data-stu-id="cce3a-112">recipients</span></span>|<span data-ttu-id="cce3a-113">String collection</span><span class="sxs-lookup"><span data-stu-id="cce3a-113">String collection</span></span>|<span data-ttu-id="cce3a-114">受信者の id のコレクション。</span><span class="sxs-lookup"><span data-stu-id="cce3a-114">A collection of ids of the recipients.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cce3a-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="cce3a-115">JSON representation</span></span>

<span data-ttu-id="cce3a-116">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="cce3a-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationAssignmentIndividualRecipient"
}-->

```json
{
  "recipients": ["String"]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationAssignmentIndividualRecipient resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationassignmentindividualrecipient.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
