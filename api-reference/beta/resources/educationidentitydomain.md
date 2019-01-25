---
title: educationIdentityDomain リソースの種類
description: '教育のユーザーの種類とユーザーのアカウントが属するドメインとの間のマッピングを表します。 ドメインのリソースは、ユーザー作成の構成の一部です。 '
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 0c6004d18897b8f8284c06a3b09830072148df87
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528180"
---
# <a name="educationidentitydomain-resource-type"></a><span data-ttu-id="8ee7d-104">educationIdentityDomain リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8ee7d-104">educationIdentityDomain resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8ee7d-105">教育のユーザーの種類とユーザーのアカウントが属するドメインとの間のマッピングを表します。</span><span class="sxs-lookup"><span data-stu-id="8ee7d-105">Represents the mapping between an education user type and the domain the user's account belongs to.</span></span> <span data-ttu-id="8ee7d-106">ドメインのリソースは、[作成時の id の構成](educationidentitycreationconfiguration.md)の一部です。</span><span class="sxs-lookup"><span data-stu-id="8ee7d-106">The domain resource is part of the [identity creation configuration](educationidentitycreationconfiguration.md).</span></span> 

## <a name="properties"></a><span data-ttu-id="8ee7d-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8ee7d-107">Properties</span></span>

| <span data-ttu-id="8ee7d-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8ee7d-108">Property</span></span> | <span data-ttu-id="8ee7d-109">型</span><span class="sxs-lookup"><span data-stu-id="8ee7d-109">Type</span></span> | <span data-ttu-id="8ee7d-110">説明</span><span class="sxs-lookup"><span data-stu-id="8ee7d-110">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="8ee7d-111">appliesTo</span><span class="sxs-lookup"><span data-stu-id="8ee7d-111">**appliesTo**</span></span> | <span data-ttu-id="8ee7d-112">string</span><span class="sxs-lookup"><span data-stu-id="8ee7d-112">string</span></span> |  <span data-ttu-id="8ee7d-113">ライセンスを割り当てるにはユーザーのロールの種類です。</span><span class="sxs-lookup"><span data-stu-id="8ee7d-113">The user role type to assign to license.</span></span> <span data-ttu-id="8ee7d-114">使用可能な値は、`student`、`teacher` です。</span><span class="sxs-lookup"><span data-stu-id="8ee7d-114">Possible values are: `student`, `teacher`.</span></span>      |
| <span data-ttu-id="8ee7d-115">**name**</span><span class="sxs-lookup"><span data-stu-id="8ee7d-115">**name**</span></span> | <span data-ttu-id="8ee7d-116">string</span><span class="sxs-lookup"><span data-stu-id="8ee7d-116">string</span></span> |  <span data-ttu-id="8ee7d-117">ユーザー アカウントのドメインを表します。</span><span class="sxs-lookup"><span data-stu-id="8ee7d-117">Represents the domain for the user account.</span></span>         |

## <a name="json-representation"></a><span data-ttu-id="8ee7d-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8ee7d-118">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationIdentityDomain"
}-->

```json
{
    "appliesTo": {"@odata.type": "microsoft.graph.educationUserRole"},
    "name": "String"
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationidentitydomain.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
