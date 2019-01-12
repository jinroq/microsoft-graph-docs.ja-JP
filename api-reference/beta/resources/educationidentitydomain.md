---
title: educationIdentityDomain リソースの種類
description: '教育のユーザーの種類とユーザーのアカウントが属するドメインとの間のマッピングを表します。 ドメインのリソースは、ユーザー作成の構成の一部です。 '
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 280ae1a65e0c14e7960d316cc21154e405f2ee0d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27982030"
---
# <a name="educationidentitydomain-resource-type"></a><span data-ttu-id="84cb3-104">educationIdentityDomain リソースの種類</span><span class="sxs-lookup"><span data-stu-id="84cb3-104">educationIdentityDomain resource type</span></span>

> <span data-ttu-id="84cb3-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="84cb3-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="84cb3-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="84cb3-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="84cb3-107">教育のユーザーの種類とユーザーのアカウントが属するドメインとの間のマッピングを表します。</span><span class="sxs-lookup"><span data-stu-id="84cb3-107">Represents the mapping between an education user type and the domain the user's account belongs to.</span></span> <span data-ttu-id="84cb3-108">ドメインのリソースは、[作成時の id の構成](educationidentitycreationconfiguration.md)の一部です。</span><span class="sxs-lookup"><span data-stu-id="84cb3-108">The domain resource is part of the [identity creation configuration](educationidentitycreationconfiguration.md).</span></span> 

## <a name="properties"></a><span data-ttu-id="84cb3-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="84cb3-109">Properties</span></span>

| <span data-ttu-id="84cb3-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="84cb3-110">Property</span></span> | <span data-ttu-id="84cb3-111">種類</span><span class="sxs-lookup"><span data-stu-id="84cb3-111">Type</span></span> | <span data-ttu-id="84cb3-112">説明</span><span class="sxs-lookup"><span data-stu-id="84cb3-112">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="84cb3-113">**appliesTo**</span><span class="sxs-lookup"><span data-stu-id="84cb3-113">**appliesTo**</span></span> | <span data-ttu-id="84cb3-114">文字列</span><span class="sxs-lookup"><span data-stu-id="84cb3-114">string</span></span> |  <span data-ttu-id="84cb3-115">ライセンスを割り当てるにはユーザーのロールの種類です。</span><span class="sxs-lookup"><span data-stu-id="84cb3-115">The user role type to assign to license.</span></span> <span data-ttu-id="84cb3-116">使用可能な値は、`student`、`teacher` です。</span><span class="sxs-lookup"><span data-stu-id="84cb3-116">Possible values are: `student`, `teacher`.</span></span>      |
| <span data-ttu-id="84cb3-117">**name**</span><span class="sxs-lookup"><span data-stu-id="84cb3-117">**name**</span></span> | <span data-ttu-id="84cb3-118">文字列</span><span class="sxs-lookup"><span data-stu-id="84cb3-118">string</span></span> |  <span data-ttu-id="84cb3-119">ユーザー アカウントのドメインを表します。</span><span class="sxs-lookup"><span data-stu-id="84cb3-119">Represents the domain for the user account.</span></span>         |

## <a name="json-representation"></a><span data-ttu-id="84cb3-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="84cb3-120">JSON representation</span></span>
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
