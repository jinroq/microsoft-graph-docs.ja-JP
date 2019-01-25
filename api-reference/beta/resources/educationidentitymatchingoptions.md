---
title: educationIdentityMatchingOptions リソースの種類
description: ユーザー アカウントを一致させるためには、ソース プロパティとターゲット プロパティの間のマッピングを提供します。 元データ ソース プロパティが存在する必要があります。 ターゲット プロパティには、Azure Active Directory (AD の Azure) の有効なプロパティをする必要があります。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 723a74cff1d5a660272d3456e9f54de8a54e21bc
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513705"
---
# <a name="educationidentitymatchingoptions-resource-type"></a><span data-ttu-id="ee102-105">educationIdentityMatchingOptions リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ee102-105">educationIdentityMatchingOptions resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ee102-106">ユーザー アカウントを一致させるためには、ソース プロパティとターゲット プロパティの間のマッピングを提供します。</span><span class="sxs-lookup"><span data-stu-id="ee102-106">Provides a mapping between a source property and a target property for matching user accounts.</span></span> <span data-ttu-id="ee102-107">元データ ソース プロパティが存在する必要があります。</span><span class="sxs-lookup"><span data-stu-id="ee102-107">The source property should exist in the source data.</span></span> <span data-ttu-id="ee102-108">ターゲット プロパティには、Azure Active Directory (AD の Azure) の有効なプロパティをする必要があります。</span><span class="sxs-lookup"><span data-stu-id="ee102-108">The target property should be a valid property in Azure Active Directory (Azure AD).</span></span>

## <a name="properties"></a><span data-ttu-id="ee102-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ee102-109">Properties</span></span>

| <span data-ttu-id="ee102-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ee102-110">Property</span></span> | <span data-ttu-id="ee102-111">型</span><span class="sxs-lookup"><span data-stu-id="ee102-111">Type</span></span> | <span data-ttu-id="ee102-112">説明</span><span class="sxs-lookup"><span data-stu-id="ee102-112">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="ee102-113">appliesTo</span><span class="sxs-lookup"><span data-stu-id="ee102-113">**appliesTo**</span></span> | <span data-ttu-id="ee102-114">string</span><span class="sxs-lookup"><span data-stu-id="ee102-114">string</span></span> |  <span data-ttu-id="ee102-115">ライセンスを割り当てるにはユーザーのロールの種類です。</span><span class="sxs-lookup"><span data-stu-id="ee102-115">The user role type to assign to the license.</span></span> <span data-ttu-id="ee102-116">使用可能な値は、`student`、`teacher` です。</span><span class="sxs-lookup"><span data-stu-id="ee102-116">Possible values are: `student`, `teacher`.</span></span>      |
| <span data-ttu-id="ee102-117">**sourcePropertyName**</span><span class="sxs-lookup"><span data-stu-id="ee102-117">**sourcePropertyName**</span></span> | <span data-ttu-id="ee102-118">string</span><span class="sxs-lookup"><span data-stu-id="ee102-118">string</span></span> |  <span data-ttu-id="ee102-119">ソース データ内のフィールド名をする必要があります、ソース プロパティの名前。</span><span class="sxs-lookup"><span data-stu-id="ee102-119">The name of the source property, which should be a field name in the source data.</span></span> <span data-ttu-id="ee102-120">このプロパティは、大文字小文字を区別します。</span><span class="sxs-lookup"><span data-stu-id="ee102-120">This property is case-sensitive.</span></span>        |
| <span data-ttu-id="ee102-121">**targetPropertyName**</span><span class="sxs-lookup"><span data-stu-id="ee102-121">**targetPropertyName**</span></span> | <span data-ttu-id="ee102-122">string</span><span class="sxs-lookup"><span data-stu-id="ee102-122">string</span></span> |  <span data-ttu-id="ee102-123">Azure AD に有効なプロパティである必要がありますターゲット プロパティの名前です。</span><span class="sxs-lookup"><span data-stu-id="ee102-123">The name of the target property, which should be a valid property in Azure AD.</span></span> <span data-ttu-id="ee102-124">このプロパティは、大文字小文字を区別します。</span><span class="sxs-lookup"><span data-stu-id="ee102-124">This property is case-sensitive.</span></span>     |
| <span data-ttu-id="ee102-125">**targetDomain**</span><span class="sxs-lookup"><span data-stu-id="ee102-125">**targetDomain**</span></span> | <span data-ttu-id="ee102-126">string</span><span class="sxs-lookup"><span data-stu-id="ee102-126">string</span></span> |  <span data-ttu-id="ee102-127">ターゲット条件に一致するソース プロパティを使用して、サフィックスをドメイン。</span><span class="sxs-lookup"><span data-stu-id="ee102-127">The domain to suffix with the source property to match on the target.</span></span> <span data-ttu-id="ee102-128">として null を指定した場合、source プロパティを使用してターゲット プロパティと一致します。</span><span class="sxs-lookup"><span data-stu-id="ee102-128">If provided as null,  the source property will be used to match with the target property.</span></span>        |

## <a name="json-representation"></a><span data-ttu-id="ee102-129">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ee102-129">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationIdentityMatchingOptions"
}-->

```json
{
    "appliesTo": {"@odata.type": "microsoft.graph.educationUserRole"},
    "sourcePropertyName": "String",
    "targetPropertyName": "String",
    "targetDomain": "String"
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationidentitymatchingoptions.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
