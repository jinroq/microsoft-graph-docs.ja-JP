---
title: educationIdentityMatchingOptions リソースの種類
description: ユーザー アカウントを一致させるためには、ソース プロパティとターゲット プロパティの間のマッピングを提供します。 元データ ソース プロパティが存在する必要があります。 ターゲット プロパティには、Azure Active Directory (AD の Azure) の有効なプロパティをする必要があります。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 624e2717387c5cc8994596fd83d5a6856ac6082b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27978257"
---
# <a name="educationidentitymatchingoptions-resource-type"></a><span data-ttu-id="bf076-105">educationIdentityMatchingOptions リソースの種類</span><span class="sxs-lookup"><span data-stu-id="bf076-105">educationIdentityMatchingOptions resource type</span></span>

> <span data-ttu-id="bf076-106">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="bf076-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bf076-107">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bf076-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bf076-108">ユーザー アカウントを一致させるためには、ソース プロパティとターゲット プロパティの間のマッピングを提供します。</span><span class="sxs-lookup"><span data-stu-id="bf076-108">Provides a mapping between a source property and a target property for matching user accounts.</span></span> <span data-ttu-id="bf076-109">元データ ソース プロパティが存在する必要があります。</span><span class="sxs-lookup"><span data-stu-id="bf076-109">The source property should exist in the source data.</span></span> <span data-ttu-id="bf076-110">ターゲット プロパティには、Azure Active Directory (AD の Azure) の有効なプロパティをする必要があります。</span><span class="sxs-lookup"><span data-stu-id="bf076-110">The target property should be a valid property in Azure Active Directory (Azure AD).</span></span>

## <a name="properties"></a><span data-ttu-id="bf076-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bf076-111">Properties</span></span>

| <span data-ttu-id="bf076-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bf076-112">Property</span></span> | <span data-ttu-id="bf076-113">種類</span><span class="sxs-lookup"><span data-stu-id="bf076-113">Type</span></span> | <span data-ttu-id="bf076-114">説明</span><span class="sxs-lookup"><span data-stu-id="bf076-114">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="bf076-115">**appliesTo**</span><span class="sxs-lookup"><span data-stu-id="bf076-115">**appliesTo**</span></span> | <span data-ttu-id="bf076-116">文字列</span><span class="sxs-lookup"><span data-stu-id="bf076-116">string</span></span> |  <span data-ttu-id="bf076-117">ライセンスを割り当てるにはユーザーのロールの種類です。</span><span class="sxs-lookup"><span data-stu-id="bf076-117">The user role type to assign to the license.</span></span> <span data-ttu-id="bf076-118">使用可能な値は、`student`、`teacher` です。</span><span class="sxs-lookup"><span data-stu-id="bf076-118">Possible values are: `student`, `teacher`.</span></span>      |
| <span data-ttu-id="bf076-119">**sourcePropertyName**</span><span class="sxs-lookup"><span data-stu-id="bf076-119">**sourcePropertyName**</span></span> | <span data-ttu-id="bf076-120">文字列</span><span class="sxs-lookup"><span data-stu-id="bf076-120">string</span></span> |  <span data-ttu-id="bf076-121">ソース データ内のフィールド名をする必要があります、ソース プロパティの名前。</span><span class="sxs-lookup"><span data-stu-id="bf076-121">The name of the source property, which should be a field name in the source data.</span></span> <span data-ttu-id="bf076-122">このプロパティは、大文字小文字を区別します。</span><span class="sxs-lookup"><span data-stu-id="bf076-122">This property is case-sensitive.</span></span>        |
| <span data-ttu-id="bf076-123">**targetPropertyName**</span><span class="sxs-lookup"><span data-stu-id="bf076-123">**targetPropertyName**</span></span> | <span data-ttu-id="bf076-124">文字列</span><span class="sxs-lookup"><span data-stu-id="bf076-124">string</span></span> |  <span data-ttu-id="bf076-125">Azure AD に有効なプロパティである必要がありますターゲット プロパティの名前です。</span><span class="sxs-lookup"><span data-stu-id="bf076-125">The name of the target property, which should be a valid property in Azure AD.</span></span> <span data-ttu-id="bf076-126">このプロパティは、大文字小文字を区別します。</span><span class="sxs-lookup"><span data-stu-id="bf076-126">This property is case-sensitive.</span></span>     |
| <span data-ttu-id="bf076-127">**targetDomain**</span><span class="sxs-lookup"><span data-stu-id="bf076-127">**targetDomain**</span></span> | <span data-ttu-id="bf076-128">文字列</span><span class="sxs-lookup"><span data-stu-id="bf076-128">string</span></span> |  <span data-ttu-id="bf076-129">ターゲット条件に一致するソース プロパティを使用して、サフィックスをドメイン。</span><span class="sxs-lookup"><span data-stu-id="bf076-129">The domain to suffix with the source property to match on the target.</span></span> <span data-ttu-id="bf076-130">として null を指定した場合、source プロパティを使用してターゲット プロパティと一致します。</span><span class="sxs-lookup"><span data-stu-id="bf076-130">If provided as null,  the source property will be used to match with the target property.</span></span>        |

## <a name="json-representation"></a><span data-ttu-id="bf076-131">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="bf076-131">JSON representation</span></span>
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
