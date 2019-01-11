---
title: educationIdentityDomain リソースの種類
description: '教育のユーザーの種類とユーザーのアカウントが属するドメインとの間のマッピングを表します。 ドメインのリソースは、ユーザー作成の構成の一部です。 '
localization_priority: Normal
ms.openlocfilehash: 5675499aca010f90deeb517210065ac4802d66b5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27807750"
---
# <a name="educationidentitydomain-resource-type"></a><span data-ttu-id="1e852-104">educationIdentityDomain リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1e852-104">educationIdentityDomain resource type</span></span>

> <span data-ttu-id="1e852-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="1e852-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1e852-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1e852-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1e852-107">教育のユーザーの種類とユーザーのアカウントが属するドメインとの間のマッピングを表します。</span><span class="sxs-lookup"><span data-stu-id="1e852-107">Represents the mapping between an education user type and the domain the user's account belongs to.</span></span> <span data-ttu-id="1e852-108">ドメインのリソースは、[作成時の id の構成](educationidentitycreationconfiguration.md)の一部です。</span><span class="sxs-lookup"><span data-stu-id="1e852-108">The domain resource is part of the [identity creation configuration](educationidentitycreationconfiguration.md).</span></span> 

## <a name="properties"></a><span data-ttu-id="1e852-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1e852-109">Properties</span></span>

| <span data-ttu-id="1e852-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1e852-110">Property</span></span> | <span data-ttu-id="1e852-111">種類</span><span class="sxs-lookup"><span data-stu-id="1e852-111">Type</span></span> | <span data-ttu-id="1e852-112">説明</span><span class="sxs-lookup"><span data-stu-id="1e852-112">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="1e852-113">**appliesTo**</span><span class="sxs-lookup"><span data-stu-id="1e852-113">**appliesTo**</span></span> | <span data-ttu-id="1e852-114">文字列</span><span class="sxs-lookup"><span data-stu-id="1e852-114">string</span></span> |  <span data-ttu-id="1e852-115">ライセンスを割り当てるにはユーザーのロールの種類です。</span><span class="sxs-lookup"><span data-stu-id="1e852-115">The user role type to assign to license.</span></span> <span data-ttu-id="1e852-116">使用可能な値は、`student`、`teacher` です。</span><span class="sxs-lookup"><span data-stu-id="1e852-116">Possible values are: `student`, `teacher`.</span></span>      |
| <span data-ttu-id="1e852-117">**name**</span><span class="sxs-lookup"><span data-stu-id="1e852-117">**name**</span></span> | <span data-ttu-id="1e852-118">文字列</span><span class="sxs-lookup"><span data-stu-id="1e852-118">string</span></span> |  <span data-ttu-id="1e852-119">ユーザー アカウントのドメインを表します。</span><span class="sxs-lookup"><span data-stu-id="1e852-119">Represents the domain for the user account.</span></span>         |

## <a name="json-representation"></a><span data-ttu-id="1e852-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1e852-120">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationIdentityDomain"
}-->

```json
{
    "appliesTo": {"@odata.type": "#microsoft.graph.educationUserRole"},
    "name": "String"
}
```
