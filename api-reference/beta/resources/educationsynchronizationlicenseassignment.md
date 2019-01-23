---
title: educationSynchronizationLicenseAssignment リソースの種類
description: ユーザー アカウントに割り当てるにはライセンス情報を表します。 新しいユーザー アカウントを作成するときに、ライセンスの割り当てを設定するのには、リソースが使用されます。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 5c60b868ab8d973f6249d7e9ea2b30415d4b8a1b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29409679"
---
# <a name="educationsynchronizationlicenseassignment-resource-type"></a><span data-ttu-id="43eb9-104">educationSynchronizationLicenseAssignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="43eb9-104">educationSynchronizationLicenseAssignment resource type</span></span>

> <span data-ttu-id="43eb9-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="43eb9-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="43eb9-106">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="43eb9-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="43eb9-107">ユーザー アカウントに割り当てるにはライセンス情報を表します。</span><span class="sxs-lookup"><span data-stu-id="43eb9-107">Represents the license information to assign to user accounts.</span></span> <span data-ttu-id="43eb9-108">新しいユーザー アカウントを作成するときに、ライセンスの割り当てを設定するのには、リソースが使用されます。</span><span class="sxs-lookup"><span data-stu-id="43eb9-108">The resource will be used to set up license assignments when creating new user accounts.</span></span>

## <a name="properties"></a><span data-ttu-id="43eb9-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="43eb9-109">Properties</span></span>

| <span data-ttu-id="43eb9-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="43eb9-110">Property</span></span> | <span data-ttu-id="43eb9-111">型</span><span class="sxs-lookup"><span data-stu-id="43eb9-111">Type</span></span> | <span data-ttu-id="43eb9-112">説明</span><span class="sxs-lookup"><span data-stu-id="43eb9-112">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="43eb9-113">**appliesTo**</span><span class="sxs-lookup"><span data-stu-id="43eb9-113">**appliesTo**</span></span> | <span data-ttu-id="43eb9-114">string</span><span class="sxs-lookup"><span data-stu-id="43eb9-114">string</span></span> | <span data-ttu-id="43eb9-115">ライセンスを割り当てるにはユーザーのロールの種類です。</span><span class="sxs-lookup"><span data-stu-id="43eb9-115">The user role type to assign to license.</span></span> <span data-ttu-id="43eb9-116">使用可能な値は、`student`、`teacher` です。</span><span class="sxs-lookup"><span data-stu-id="43eb9-116">Possible values are: `student`, `teacher`.</span></span>         |
| <span data-ttu-id="43eb9-117">**skuIds**</span><span class="sxs-lookup"><span data-stu-id="43eb9-117">**skuIds**</span></span> | <span data-ttu-id="43eb9-118">文字列のコレクション</span><span class="sxs-lookup"><span data-stu-id="43eb9-118">collection of strings</span></span> |  <span data-ttu-id="43eb9-119">割り当てるライセンスの SKU 識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="43eb9-119">Represents the SKU identifiers of the licenses to assign.</span></span>        |

## <a name="json-representation"></a><span data-ttu-id="43eb9-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="43eb9-120">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSynchronizationLicenseAssignment"
}-->

```json
{
    "appliesTo": {"@odata.type": "microsoft.graph.educationUserRole"},
    "skuIds": ["String"]
}
```
