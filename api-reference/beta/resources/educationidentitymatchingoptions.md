---
title: educationIdentityMatchingOptions リソースの種類
description: ユーザー アカウントを一致させるためには、ソース プロパティとターゲット プロパティの間のマッピングを提供します。 元データ ソース プロパティが存在する必要があります。 ターゲット プロパティには、Azure Active Directory (AD の Azure) の有効なプロパティをする必要があります。
ms.openlocfilehash: 2cabb255648f4089d437912a97bb7d29ff286779
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071882"
---
# <a name="educationidentitymatchingoptions-resource-type"></a><span data-ttu-id="aa870-105">educationIdentityMatchingOptions リソースの種類</span><span class="sxs-lookup"><span data-stu-id="aa870-105">educationIdentityMatchingOptions resource type</span></span>

> <span data-ttu-id="aa870-106">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="aa870-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="aa870-107">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="aa870-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="aa870-108">ユーザー アカウントを一致させるためには、ソース プロパティとターゲット プロパティの間のマッピングを提供します。</span><span class="sxs-lookup"><span data-stu-id="aa870-108">Provides a mapping between a source property and a target property for matching user accounts.</span></span> <span data-ttu-id="aa870-109">元データ ソース プロパティが存在する必要があります。</span><span class="sxs-lookup"><span data-stu-id="aa870-109">The source property should exist in the source data.</span></span> <span data-ttu-id="aa870-110">ターゲット プロパティには、Azure Active Directory (AD の Azure) の有効なプロパティをする必要があります。</span><span class="sxs-lookup"><span data-stu-id="aa870-110">The target property should be a valid property in Azure Active Directory (Azure AD).</span></span>

## <a name="properties"></a><span data-ttu-id="aa870-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="aa870-111">Properties</span></span>

| <span data-ttu-id="aa870-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="aa870-112">Property</span></span> | <span data-ttu-id="aa870-113">型</span><span class="sxs-lookup"><span data-stu-id="aa870-113">Type</span></span> | <span data-ttu-id="aa870-114">説明</span><span class="sxs-lookup"><span data-stu-id="aa870-114">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="aa870-115">**appliesTo**</span><span class="sxs-lookup"><span data-stu-id="aa870-115">**appliesTo**</span></span> | <span data-ttu-id="aa870-116">文字列</span><span class="sxs-lookup"><span data-stu-id="aa870-116">string</span></span> |  <span data-ttu-id="aa870-117">ライセンスを割り当てるにはユーザーのロールの種類です。</span><span class="sxs-lookup"><span data-stu-id="aa870-117">The user role type to assign to the license.</span></span> <span data-ttu-id="aa870-118">使用可能な値は、`student`、`teacher` です。</span><span class="sxs-lookup"><span data-stu-id="aa870-118">Possible values are: `student`, `teacher`.</span></span>      |
| <span data-ttu-id="aa870-119">**sourcePropertyName**</span><span class="sxs-lookup"><span data-stu-id="aa870-119">**sourcePropertyName**</span></span> | <span data-ttu-id="aa870-120">文字列</span><span class="sxs-lookup"><span data-stu-id="aa870-120">string</span></span> |  <span data-ttu-id="aa870-121">ソース データ内のフィールド名をする必要があります、ソース プロパティの名前。</span><span class="sxs-lookup"><span data-stu-id="aa870-121">The name of the source property, which should be a field name in the source data.</span></span> <span data-ttu-id="aa870-122">このプロパティは、大文字小文字を区別します。</span><span class="sxs-lookup"><span data-stu-id="aa870-122">This property is case-sensitive.</span></span>        |
| <span data-ttu-id="aa870-123">**targetPropertyName**</span><span class="sxs-lookup"><span data-stu-id="aa870-123">**targetPropertyName**</span></span> | <span data-ttu-id="aa870-124">文字列</span><span class="sxs-lookup"><span data-stu-id="aa870-124">string</span></span> |  <span data-ttu-id="aa870-125">Azure AD に有効なプロパティである必要がありますターゲット プロパティの名前です。</span><span class="sxs-lookup"><span data-stu-id="aa870-125">The name of the target property, which should be a valid property in Azure AD.</span></span> <span data-ttu-id="aa870-126">このプロパティは、大文字小文字を区別します。</span><span class="sxs-lookup"><span data-stu-id="aa870-126">This property is case-sensitive.</span></span>     |
| <span data-ttu-id="aa870-127">**targetDomain**</span><span class="sxs-lookup"><span data-stu-id="aa870-127">**targetDomain**</span></span> | <span data-ttu-id="aa870-128">文字列</span><span class="sxs-lookup"><span data-stu-id="aa870-128">string</span></span> |  <span data-ttu-id="aa870-129">ターゲット条件に一致するソース プロパティを使用して、サフィックスをドメイン。</span><span class="sxs-lookup"><span data-stu-id="aa870-129">The domain to suffix with the source property to match on the target.</span></span> <span data-ttu-id="aa870-130">として null を指定した場合、source プロパティを使用してターゲット プロパティと一致します。</span><span class="sxs-lookup"><span data-stu-id="aa870-130">If provided as null,  the source property will be used to match with the target property.</span></span>        |

## <a name="json-representation"></a><span data-ttu-id="aa870-131">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="aa870-131">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationIdentityMatchingOptions"
}-->

```json
{
    "appliesTo": {"@odata.type": "#microsoft.graph.educationUserRole"},
    "sourcePropertyName": "String",
    "targetPropertyName": "String",
    "targetDomain": "String"
}
```
