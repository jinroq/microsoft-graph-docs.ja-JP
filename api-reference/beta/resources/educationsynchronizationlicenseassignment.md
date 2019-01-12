---
title: educationSynchronizationLicenseAssignment リソースの種類
description: ユーザー アカウントに割り当てるにはライセンス情報を表します。 新しいユーザー アカウントを作成するときに、ライセンスの割り当てを設定するのには、リソースが使用されます。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 757e080a8b2c6f3f01fa1663f10c9b0b98eaf4d3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27948276"
---
# <a name="educationsynchronizationlicenseassignment-resource-type"></a><span data-ttu-id="71963-104">educationSynchronizationLicenseAssignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="71963-104">educationSynchronizationLicenseAssignment resource type</span></span>

> <span data-ttu-id="71963-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="71963-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="71963-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="71963-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="71963-107">ユーザー アカウントに割り当てるにはライセンス情報を表します。</span><span class="sxs-lookup"><span data-stu-id="71963-107">Represents the license information to assign to user accounts.</span></span> <span data-ttu-id="71963-108">新しいユーザー アカウントを作成するときに、ライセンスの割り当てを設定するのには、リソースが使用されます。</span><span class="sxs-lookup"><span data-stu-id="71963-108">The resource will be used to set up license assignments when creating new user accounts.</span></span>

## <a name="properties"></a><span data-ttu-id="71963-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="71963-109">Properties</span></span>

| <span data-ttu-id="71963-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="71963-110">Property</span></span> | <span data-ttu-id="71963-111">種類</span><span class="sxs-lookup"><span data-stu-id="71963-111">Type</span></span> | <span data-ttu-id="71963-112">説明</span><span class="sxs-lookup"><span data-stu-id="71963-112">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="71963-113">**appliesTo**</span><span class="sxs-lookup"><span data-stu-id="71963-113">**appliesTo**</span></span> | <span data-ttu-id="71963-114">文字列</span><span class="sxs-lookup"><span data-stu-id="71963-114">string</span></span> | <span data-ttu-id="71963-115">ライセンスを割り当てるにはユーザーのロールの種類です。</span><span class="sxs-lookup"><span data-stu-id="71963-115">The user role type to assign to license.</span></span> <span data-ttu-id="71963-116">使用可能な値は、`student`、`teacher` です。</span><span class="sxs-lookup"><span data-stu-id="71963-116">Possible values are: `student`, `teacher`.</span></span>         |
| <span data-ttu-id="71963-117">**skuIds**</span><span class="sxs-lookup"><span data-stu-id="71963-117">**skuIds**</span></span> | <span data-ttu-id="71963-118">文字列のコレクション</span><span class="sxs-lookup"><span data-stu-id="71963-118">collection of strings</span></span> |  <span data-ttu-id="71963-119">割り当てるライセンスの SKU 識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="71963-119">Represents the SKU identifiers of the licenses to assign.</span></span>        |

## <a name="json-representation"></a><span data-ttu-id="71963-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="71963-120">JSON representation</span></span>
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
