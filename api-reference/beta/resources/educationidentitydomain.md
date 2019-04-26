---
title: educationIdentityDomain リソースの種類
description: '教育ユーザーの種類とユーザーのアカウントが属するドメインとの間のマッピングを表します。 ドメインリソースは、id 作成構成の一部です。 '
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 5cf7444c51b34ae4a8eacf9c99fdfd085dbec896
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33334269"
---
# <a name="educationidentitydomain-resource-type"></a><span data-ttu-id="9ee3a-104">educationIdentityDomain リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9ee3a-104">educationIdentityDomain resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9ee3a-105">教育ユーザーの種類とユーザーのアカウントが属するドメインとの間のマッピングを表します。</span><span class="sxs-lookup"><span data-stu-id="9ee3a-105">Represents the mapping between an education user type and the domain the user's account belongs to.</span></span> <span data-ttu-id="9ee3a-106">ドメインリソースは、 [id 作成構成](educationidentitycreationconfiguration.md)の一部です。</span><span class="sxs-lookup"><span data-stu-id="9ee3a-106">The domain resource is part of the [identity creation configuration](educationidentitycreationconfiguration.md).</span></span> 

## <a name="properties"></a><span data-ttu-id="9ee3a-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9ee3a-107">Properties</span></span>

| <span data-ttu-id="9ee3a-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9ee3a-108">Property</span></span> | <span data-ttu-id="9ee3a-109">型</span><span class="sxs-lookup"><span data-stu-id="9ee3a-109">Type</span></span> | <span data-ttu-id="9ee3a-110">説明</span><span class="sxs-lookup"><span data-stu-id="9ee3a-110">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="9ee3a-111">**appliesTo**</span><span class="sxs-lookup"><span data-stu-id="9ee3a-111">**appliesTo**</span></span> | <span data-ttu-id="9ee3a-112">string</span><span class="sxs-lookup"><span data-stu-id="9ee3a-112">string</span></span> |  <span data-ttu-id="9ee3a-113">ライセンスに割り当てるユーザーの役割の種類。</span><span class="sxs-lookup"><span data-stu-id="9ee3a-113">The user role type to assign to license.</span></span> <span data-ttu-id="9ee3a-114">可能な値は、`student`、`teacher` です。</span><span class="sxs-lookup"><span data-stu-id="9ee3a-114">Possible values are: `student`, `teacher`.</span></span>      |
| <span data-ttu-id="9ee3a-115">**name**</span><span class="sxs-lookup"><span data-stu-id="9ee3a-115">**name**</span></span> | <span data-ttu-id="9ee3a-116">string</span><span class="sxs-lookup"><span data-stu-id="9ee3a-116">string</span></span> |  <span data-ttu-id="9ee3a-117">ユーザーアカウントのドメインを表します。</span><span class="sxs-lookup"><span data-stu-id="9ee3a-117">Represents the domain for the user account.</span></span>         |

## <a name="json-representation"></a><span data-ttu-id="9ee3a-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9ee3a-118">JSON representation</span></span>
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
