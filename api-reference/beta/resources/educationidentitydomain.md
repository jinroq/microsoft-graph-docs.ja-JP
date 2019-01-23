---
title: educationIdentityDomain リソースの種類
description: '教育のユーザーの種類とユーザーのアカウントが属するドメインとの間のマッピングを表します。 ドメインのリソースは、ユーザー作成の構成の一部です。 '
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 4eb9e5b58f62a23dbe1b450c2ec6b9d2f94970ac
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395651"
---
# <a name="educationidentitydomain-resource-type"></a><span data-ttu-id="892e8-104">educationIdentityDomain リソースの種類</span><span class="sxs-lookup"><span data-stu-id="892e8-104">educationIdentityDomain resource type</span></span>

> <span data-ttu-id="892e8-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="892e8-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="892e8-106">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="892e8-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="892e8-107">教育のユーザーの種類とユーザーのアカウントが属するドメインとの間のマッピングを表します。</span><span class="sxs-lookup"><span data-stu-id="892e8-107">Represents the mapping between an education user type and the domain the user's account belongs to.</span></span> <span data-ttu-id="892e8-108">ドメインのリソースは、[作成時の id の構成](educationidentitycreationconfiguration.md)の一部です。</span><span class="sxs-lookup"><span data-stu-id="892e8-108">The domain resource is part of the [identity creation configuration](educationidentitycreationconfiguration.md).</span></span> 

## <a name="properties"></a><span data-ttu-id="892e8-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="892e8-109">Properties</span></span>

| <span data-ttu-id="892e8-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="892e8-110">Property</span></span> | <span data-ttu-id="892e8-111">型</span><span class="sxs-lookup"><span data-stu-id="892e8-111">Type</span></span> | <span data-ttu-id="892e8-112">説明</span><span class="sxs-lookup"><span data-stu-id="892e8-112">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="892e8-113">**appliesTo**</span><span class="sxs-lookup"><span data-stu-id="892e8-113">**appliesTo**</span></span> | <span data-ttu-id="892e8-114">string</span><span class="sxs-lookup"><span data-stu-id="892e8-114">string</span></span> |  <span data-ttu-id="892e8-115">ライセンスを割り当てるにはユーザーのロールの種類です。</span><span class="sxs-lookup"><span data-stu-id="892e8-115">The user role type to assign to license.</span></span> <span data-ttu-id="892e8-116">使用可能な値は、`student`、`teacher` です。</span><span class="sxs-lookup"><span data-stu-id="892e8-116">Possible values are: `student`, `teacher`.</span></span>      |
| <span data-ttu-id="892e8-117">**name**</span><span class="sxs-lookup"><span data-stu-id="892e8-117">**name**</span></span> | <span data-ttu-id="892e8-118">string</span><span class="sxs-lookup"><span data-stu-id="892e8-118">string</span></span> |  <span data-ttu-id="892e8-119">ユーザー アカウントのドメインを表します。</span><span class="sxs-lookup"><span data-stu-id="892e8-119">Represents the domain for the user account.</span></span>         |

## <a name="json-representation"></a><span data-ttu-id="892e8-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="892e8-120">JSON representation</span></span>
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
