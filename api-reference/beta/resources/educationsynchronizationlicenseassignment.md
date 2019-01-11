---
title: educationSynchronizationLicenseAssignment リソースの種類
description: ユーザー アカウントに割り当てるにはライセンス情報を表します。 新しいユーザー アカウントを作成するときに、ライセンスの割り当てを設定するのには、リソースが使用されます。
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: 9100ba799c8981d5defdd74d6346a66859b2d53e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27804908"
---
# <a name="educationsynchronizationlicenseassignment-resource-type"></a><span data-ttu-id="09d81-104">educationSynchronizationLicenseAssignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="09d81-104">educationSynchronizationLicenseAssignment resource type</span></span>

> <span data-ttu-id="09d81-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="09d81-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="09d81-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="09d81-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="09d81-107">ユーザー アカウントに割り当てるにはライセンス情報を表します。</span><span class="sxs-lookup"><span data-stu-id="09d81-107">Represents the license information to assign to user accounts.</span></span> <span data-ttu-id="09d81-108">新しいユーザー アカウントを作成するときに、ライセンスの割り当てを設定するのには、リソースが使用されます。</span><span class="sxs-lookup"><span data-stu-id="09d81-108">The resource will be used to set up license assignments when creating new user accounts.</span></span>

## <a name="properties"></a><span data-ttu-id="09d81-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="09d81-109">Properties</span></span>

| <span data-ttu-id="09d81-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="09d81-110">Property</span></span> | <span data-ttu-id="09d81-111">種類</span><span class="sxs-lookup"><span data-stu-id="09d81-111">Type</span></span> | <span data-ttu-id="09d81-112">説明</span><span class="sxs-lookup"><span data-stu-id="09d81-112">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="09d81-113">**appliesTo**</span><span class="sxs-lookup"><span data-stu-id="09d81-113">**appliesTo**</span></span> | <span data-ttu-id="09d81-114">文字列</span><span class="sxs-lookup"><span data-stu-id="09d81-114">string</span></span> | <span data-ttu-id="09d81-115">ライセンスを割り当てるにはユーザーのロールの種類です。</span><span class="sxs-lookup"><span data-stu-id="09d81-115">The user role type to assign to license.</span></span> <span data-ttu-id="09d81-116">使用可能な値は、`student`、`teacher` です。</span><span class="sxs-lookup"><span data-stu-id="09d81-116">Possible values are: `student`, `teacher`.</span></span>         |
| <span data-ttu-id="09d81-117">**skuIds**</span><span class="sxs-lookup"><span data-stu-id="09d81-117">**skuIds**</span></span> | <span data-ttu-id="09d81-118">文字列のコレクション</span><span class="sxs-lookup"><span data-stu-id="09d81-118">collection of strings</span></span> |  <span data-ttu-id="09d81-119">割り当てるライセンスの SKU 識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="09d81-119">Represents the SKU identifiers of the licenses to assign.</span></span>        |

## <a name="json-representation"></a><span data-ttu-id="09d81-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="09d81-120">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationSynchronizationLicenseAssignment"
}-->

```json
{
    "appliesTo": {"@odata.type": "#microsoft.graph.educationUserRole"},
    "skuIds": ["String"]
}
```
