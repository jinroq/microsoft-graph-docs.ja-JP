---
title: educationIdentityDomain リソースの種類
description: '教育ユーザーの種類とユーザーのアカウントが属するドメインとの間のマッピングを表します。 ドメインリソースは、id 作成構成の一部です。 '
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 86e65d46c8037ebcbb2c98f9f9e93f94f34bbdef
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972706"
---
# <a name="educationidentitydomain-resource-type"></a><span data-ttu-id="2ec74-104">educationIdentityDomain リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2ec74-104">educationIdentityDomain resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2ec74-105">教育ユーザーの種類とユーザーのアカウントが属するドメインとの間のマッピングを表します。</span><span class="sxs-lookup"><span data-stu-id="2ec74-105">Represents the mapping between an education user type and the domain the user's account belongs to.</span></span> <span data-ttu-id="2ec74-106">ドメインリソースは、 [id 作成構成](educationidentitycreationconfiguration.md)の一部です。</span><span class="sxs-lookup"><span data-stu-id="2ec74-106">The domain resource is part of the [identity creation configuration](educationidentitycreationconfiguration.md).</span></span> 

## <a name="properties"></a><span data-ttu-id="2ec74-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2ec74-107">Properties</span></span>

| <span data-ttu-id="2ec74-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2ec74-108">Property</span></span> | <span data-ttu-id="2ec74-109">型</span><span class="sxs-lookup"><span data-stu-id="2ec74-109">Type</span></span> | <span data-ttu-id="2ec74-110">説明</span><span class="sxs-lookup"><span data-stu-id="2ec74-110">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="2ec74-111">**appliesTo**</span><span class="sxs-lookup"><span data-stu-id="2ec74-111">**appliesTo**</span></span> | <span data-ttu-id="2ec74-112">string</span><span class="sxs-lookup"><span data-stu-id="2ec74-112">string</span></span> |  <span data-ttu-id="2ec74-113">ライセンスに割り当てるユーザーロールの種類。</span><span class="sxs-lookup"><span data-stu-id="2ec74-113">The user role type to assign to the license.</span></span> <span data-ttu-id="2ec74-114">可能な値は、`student`、`teacher`、`faculty` です。</span><span class="sxs-lookup"><span data-stu-id="2ec74-114">Possible values are: `student`, `teacher`, `faculty`.</span></span>      |
| <span data-ttu-id="2ec74-115">**name**</span><span class="sxs-lookup"><span data-stu-id="2ec74-115">**name**</span></span> | <span data-ttu-id="2ec74-116">string</span><span class="sxs-lookup"><span data-stu-id="2ec74-116">string</span></span> |  <span data-ttu-id="2ec74-117">ユーザーアカウントのドメインを表します。</span><span class="sxs-lookup"><span data-stu-id="2ec74-117">Represents the domain for the user account.</span></span>         |

## <a name="json-representation"></a><span data-ttu-id="2ec74-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2ec74-118">JSON representation</span></span>
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
