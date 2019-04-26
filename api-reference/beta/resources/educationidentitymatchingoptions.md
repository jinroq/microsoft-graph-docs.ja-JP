---
title: educationIdentityMatchingOptions リソースの種類
description: ソースプロパティと、一致するユーザーアカウントのターゲットプロパティとの間のマッピングを提供します。 source プロパティはソースデータに存在する必要があります。 target プロパティは、azure Active Directory (azure AD) の有効なプロパティである必要があります。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 7ce68460e8dfd0ff3e58b51d0007278aa6c9426e
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33334243"
---
# <a name="educationidentitymatchingoptions-resource-type"></a><span data-ttu-id="2d46c-105">educationIdentityMatchingOptions リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2d46c-105">educationIdentityMatchingOptions resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2d46c-106">ソースプロパティと、一致するユーザーアカウントのターゲットプロパティとの間のマッピングを提供します。</span><span class="sxs-lookup"><span data-stu-id="2d46c-106">Provides a mapping between a source property and a target property for matching user accounts.</span></span> <span data-ttu-id="2d46c-107">source プロパティはソースデータに存在する必要があります。</span><span class="sxs-lookup"><span data-stu-id="2d46c-107">The source property should exist in the source data.</span></span> <span data-ttu-id="2d46c-108">target プロパティは、azure Active Directory (azure AD) の有効なプロパティである必要があります。</span><span class="sxs-lookup"><span data-stu-id="2d46c-108">The target property should be a valid property in Azure Active Directory (Azure AD).</span></span>

## <a name="properties"></a><span data-ttu-id="2d46c-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2d46c-109">Properties</span></span>

| <span data-ttu-id="2d46c-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2d46c-110">Property</span></span> | <span data-ttu-id="2d46c-111">型</span><span class="sxs-lookup"><span data-stu-id="2d46c-111">Type</span></span> | <span data-ttu-id="2d46c-112">説明</span><span class="sxs-lookup"><span data-stu-id="2d46c-112">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="2d46c-113">**appliesTo**</span><span class="sxs-lookup"><span data-stu-id="2d46c-113">**appliesTo**</span></span> | <span data-ttu-id="2d46c-114">string</span><span class="sxs-lookup"><span data-stu-id="2d46c-114">string</span></span> |  <span data-ttu-id="2d46c-115">ライセンスに割り当てるユーザーロールの種類。</span><span class="sxs-lookup"><span data-stu-id="2d46c-115">The user role type to assign to the license.</span></span> <span data-ttu-id="2d46c-116">可能な値は、`student`、`teacher` です。</span><span class="sxs-lookup"><span data-stu-id="2d46c-116">Possible values are: `student`, `teacher`.</span></span>      |
| <span data-ttu-id="2d46c-117">**sourcepropertyname**</span><span class="sxs-lookup"><span data-stu-id="2d46c-117">**sourcePropertyName**</span></span> | <span data-ttu-id="2d46c-118">string</span><span class="sxs-lookup"><span data-stu-id="2d46c-118">string</span></span> |  <span data-ttu-id="2d46c-119">source プロパティの名前です。ソースデータのフィールド名を指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="2d46c-119">The name of the source property, which should be a field name in the source data.</span></span> <span data-ttu-id="2d46c-120">このプロパティは大文字と小文字を区別します。</span><span class="sxs-lookup"><span data-stu-id="2d46c-120">This property is case-sensitive.</span></span>        |
| <span data-ttu-id="2d46c-121">**targetpropertyname**</span><span class="sxs-lookup"><span data-stu-id="2d46c-121">**targetPropertyName**</span></span> | <span data-ttu-id="2d46c-122">string</span><span class="sxs-lookup"><span data-stu-id="2d46c-122">string</span></span> |  <span data-ttu-id="2d46c-123">ターゲットプロパティの名前。これは、Azure AD の有効なプロパティである必要があります。</span><span class="sxs-lookup"><span data-stu-id="2d46c-123">The name of the target property, which should be a valid property in Azure AD.</span></span> <span data-ttu-id="2d46c-124">このプロパティは大文字と小文字を区別します。</span><span class="sxs-lookup"><span data-stu-id="2d46c-124">This property is case-sensitive.</span></span>     |
| <span data-ttu-id="2d46c-125">**targetdomain**</span><span class="sxs-lookup"><span data-stu-id="2d46c-125">**targetDomain**</span></span> | <span data-ttu-id="2d46c-126">string</span><span class="sxs-lookup"><span data-stu-id="2d46c-126">string</span></span> |  <span data-ttu-id="2d46c-127">ターゲットに一致する source プロパティを持つ、ドメインのサフィックス。</span><span class="sxs-lookup"><span data-stu-id="2d46c-127">The domain to suffix with the source property to match on the target.</span></span> <span data-ttu-id="2d46c-128">null として指定された場合、source プロパティを使用してターゲットプロパティと照合します。</span><span class="sxs-lookup"><span data-stu-id="2d46c-128">If provided as null,  the source property will be used to match with the target property.</span></span>        |

## <a name="json-representation"></a><span data-ttu-id="2d46c-129">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2d46c-129">JSON representation</span></span>
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
