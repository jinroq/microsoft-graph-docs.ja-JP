---
title: educationIdentityMatchingOptions リソースの種類
description: ソースプロパティと、一致するユーザーアカウントのターゲットプロパティとの間のマッピングを提供します。 Source プロパティはソースデータに存在する必要があります。 Target プロパティは、Azure Active Directory (Azure AD) の有効なプロパティである必要があります。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 88a22ff446aaa4fd1e7093ec507372c03afcc42b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972692"
---
# <a name="educationidentitymatchingoptions-resource-type"></a><span data-ttu-id="d24a5-105">educationIdentityMatchingOptions リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d24a5-105">educationIdentityMatchingOptions resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d24a5-106">ソースプロパティと、一致するユーザーアカウントのターゲットプロパティとの間のマッピングを提供します。</span><span class="sxs-lookup"><span data-stu-id="d24a5-106">Provides a mapping between a source property and a target property for matching user accounts.</span></span> <span data-ttu-id="d24a5-107">Source プロパティはソースデータに存在する必要があります。</span><span class="sxs-lookup"><span data-stu-id="d24a5-107">The source property should exist in the source data.</span></span> <span data-ttu-id="d24a5-108">Target プロパティは、Azure Active Directory (Azure AD) の有効なプロパティである必要があります。</span><span class="sxs-lookup"><span data-stu-id="d24a5-108">The target property should be a valid property in Azure Active Directory (Azure AD).</span></span>

## <a name="properties"></a><span data-ttu-id="d24a5-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d24a5-109">Properties</span></span>

| <span data-ttu-id="d24a5-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d24a5-110">Property</span></span> | <span data-ttu-id="d24a5-111">型</span><span class="sxs-lookup"><span data-stu-id="d24a5-111">Type</span></span> | <span data-ttu-id="d24a5-112">説明</span><span class="sxs-lookup"><span data-stu-id="d24a5-112">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="d24a5-113">**appliesTo**</span><span class="sxs-lookup"><span data-stu-id="d24a5-113">**appliesTo**</span></span> | <span data-ttu-id="d24a5-114">string</span><span class="sxs-lookup"><span data-stu-id="d24a5-114">string</span></span> |  <span data-ttu-id="d24a5-115">ライセンスに割り当てるユーザーロールの種類。</span><span class="sxs-lookup"><span data-stu-id="d24a5-115">The user role type to assign to the license.</span></span> <span data-ttu-id="d24a5-116">可能な値は、`student`、`teacher`、`faculty` です。</span><span class="sxs-lookup"><span data-stu-id="d24a5-116">Possible values are: `student`, `teacher`, `faculty`.</span></span>      |
| <span data-ttu-id="d24a5-117">**sourcePropertyName**</span><span class="sxs-lookup"><span data-stu-id="d24a5-117">**sourcePropertyName**</span></span> | <span data-ttu-id="d24a5-118">string</span><span class="sxs-lookup"><span data-stu-id="d24a5-118">string</span></span> |  <span data-ttu-id="d24a5-119">Source プロパティの名前です。ソースデータのフィールド名を指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="d24a5-119">The name of the source property, which should be a field name in the source data.</span></span> <span data-ttu-id="d24a5-120">このプロパティは大文字と小文字を区別します。</span><span class="sxs-lookup"><span data-stu-id="d24a5-120">This property is case-sensitive.</span></span>        |
| <span data-ttu-id="d24a5-121">**targetPropertyName**</span><span class="sxs-lookup"><span data-stu-id="d24a5-121">**targetPropertyName**</span></span> | <span data-ttu-id="d24a5-122">string</span><span class="sxs-lookup"><span data-stu-id="d24a5-122">string</span></span> |  <span data-ttu-id="d24a5-123">ターゲットプロパティの名前。これは、Azure AD の有効なプロパティである必要があります。</span><span class="sxs-lookup"><span data-stu-id="d24a5-123">The name of the target property, which should be a valid property in Azure AD.</span></span> <span data-ttu-id="d24a5-124">このプロパティは大文字と小文字を区別します。</span><span class="sxs-lookup"><span data-stu-id="d24a5-124">This property is case-sensitive.</span></span>     |
| <span data-ttu-id="d24a5-125">**targetDomain**</span><span class="sxs-lookup"><span data-stu-id="d24a5-125">**targetDomain**</span></span> | <span data-ttu-id="d24a5-126">string</span><span class="sxs-lookup"><span data-stu-id="d24a5-126">string</span></span> |  <span data-ttu-id="d24a5-127">ターゲットに一致する source プロパティを持つ、ドメインのサフィックス。</span><span class="sxs-lookup"><span data-stu-id="d24a5-127">The domain to suffix with the source property to match on the target.</span></span> <span data-ttu-id="d24a5-128">Null として指定された場合、source プロパティを使用してターゲットプロパティと照合します。</span><span class="sxs-lookup"><span data-stu-id="d24a5-128">If provided as null,  the source property will be used to match with the target property.</span></span>        |

## <a name="json-representation"></a><span data-ttu-id="d24a5-129">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d24a5-129">JSON representation</span></span>
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
