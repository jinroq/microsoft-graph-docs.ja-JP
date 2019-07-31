---
title: educationAssignmentIndividualRecipient リソースの種類
description: 'プロパティへの割り当ての中で使用されます。 個別の受信者一覧に設定すると、クラス内の学生が選択されます。 '
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 7408382cadcb53d857bb36b06702f7857d64a8f4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006452"
---
# <a name="educationassignmentindividualrecipient-resource-type"></a><span data-ttu-id="805d5-104">educationAssignmentIndividualRecipient リソースの種類</span><span class="sxs-lookup"><span data-stu-id="805d5-104">educationAssignmentIndividualRecipient resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="805d5-105">プロパティへの[割り当て](educationassignment.md)の中で使用されます。</span><span class="sxs-lookup"><span data-stu-id="805d5-105">Used inside the [assignment.assignTo](educationassignment.md) property.</span></span> <span data-ttu-id="805d5-106">個別の受信者一覧に設定した場合、クラス内の学生は、割り当てが発行されたときに送信オブジェクトを受け取ります。</span><span class="sxs-lookup"><span data-stu-id="805d5-106">When set to individual recipient list, selected students in the class will receive a submission object when the assignment is published.</span></span>

<span data-ttu-id="805d5-107">このリソースは[educationAssignmentRecipient](educationassignmentrecipient.md)のサブクラスです。</span><span class="sxs-lookup"><span data-stu-id="805d5-107">This resource is a subclass of [educationAssignmentRecipient](educationassignmentrecipient.md).</span></span>

## <a name="properties"></a><span data-ttu-id="805d5-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="805d5-108">Properties</span></span>
| <span data-ttu-id="805d5-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="805d5-109">Property</span></span>     | <span data-ttu-id="805d5-110">型</span><span class="sxs-lookup"><span data-stu-id="805d5-110">Type</span></span>   |<span data-ttu-id="805d5-111">説明</span><span class="sxs-lookup"><span data-stu-id="805d5-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="805d5-112">recipients</span><span class="sxs-lookup"><span data-stu-id="805d5-112">recipients</span></span>|<span data-ttu-id="805d5-113">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="805d5-113">String collection</span></span>|<span data-ttu-id="805d5-114">受信者の id のコレクション。</span><span class="sxs-lookup"><span data-stu-id="805d5-114">A collection of ids of the recipients.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="805d5-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="805d5-115">JSON representation</span></span>

<span data-ttu-id="805d5-116">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="805d5-116">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
