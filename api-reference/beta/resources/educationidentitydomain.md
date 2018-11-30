---
title: educationIdentityDomain リソースの種類
description: '教育のユーザーの種類とユーザーのアカウントが属するドメインとの間のマッピングを表します。 ドメインのリソースは、ユーザー作成の構成の一部です。 '
ms.openlocfilehash: 8298e1eb38ae70f982719ee3a7d6588cd181bdd8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071683"
---
# <a name="educationidentitydomain-resource-type"></a><span data-ttu-id="b35b7-104">educationIdentityDomain リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b35b7-104">educationIdentityDomain resource type</span></span>

> <span data-ttu-id="b35b7-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b35b7-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b35b7-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b35b7-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b35b7-107">教育のユーザーの種類とユーザーのアカウントが属するドメインとの間のマッピングを表します。</span><span class="sxs-lookup"><span data-stu-id="b35b7-107">Represents the mapping between an education user type and the domain the user's account belongs to.</span></span> <span data-ttu-id="b35b7-108">ドメインのリソースは、[作成時の id の構成](educationidentitycreationconfiguration.md)の一部です。</span><span class="sxs-lookup"><span data-stu-id="b35b7-108">The domain resource is part of the [identity creation configuration](educationidentitycreationconfiguration.md).</span></span> 

## <a name="properties"></a><span data-ttu-id="b35b7-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b35b7-109">Properties</span></span>

| <span data-ttu-id="b35b7-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b35b7-110">Property</span></span> | <span data-ttu-id="b35b7-111">型</span><span class="sxs-lookup"><span data-stu-id="b35b7-111">Type</span></span> | <span data-ttu-id="b35b7-112">説明</span><span class="sxs-lookup"><span data-stu-id="b35b7-112">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="b35b7-113">**appliesTo**</span><span class="sxs-lookup"><span data-stu-id="b35b7-113">**appliesTo**</span></span> | <span data-ttu-id="b35b7-114">文字列</span><span class="sxs-lookup"><span data-stu-id="b35b7-114">string</span></span> |  <span data-ttu-id="b35b7-115">ライセンスを割り当てるにはユーザーのロールの種類です。</span><span class="sxs-lookup"><span data-stu-id="b35b7-115">The user role type to assign to license.</span></span> <span data-ttu-id="b35b7-116">使用可能な値は、`student`、`teacher` です。</span><span class="sxs-lookup"><span data-stu-id="b35b7-116">Possible values are: `student`, `teacher`.</span></span>      |
| <span data-ttu-id="b35b7-117">**name**</span><span class="sxs-lookup"><span data-stu-id="b35b7-117">**name**</span></span> | <span data-ttu-id="b35b7-118">文字列</span><span class="sxs-lookup"><span data-stu-id="b35b7-118">string</span></span> |  <span data-ttu-id="b35b7-119">ユーザー アカウントのドメインを表します。</span><span class="sxs-lookup"><span data-stu-id="b35b7-119">Represents the domain for the user account.</span></span>         |

## <a name="json-representation"></a><span data-ttu-id="b35b7-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b35b7-120">JSON representation</span></span>
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
