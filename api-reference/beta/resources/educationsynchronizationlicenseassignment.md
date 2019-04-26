---
title: educationSynchronizationLicenseAssignment リソースの種類
description: ユーザーアカウントに割り当てるライセンス情報を表します。 リソースは、新しいユーザーアカウントの作成時にライセンスの割り当てを設定するために使用されます。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: ae9b89d9fe921967b50b8e290ce29026dbc35ec1
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33334052"
---
# <a name="educationsynchronizationlicenseassignment-resource-type"></a><span data-ttu-id="22b08-104">educationSynchronizationLicenseAssignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="22b08-104">educationSynchronizationLicenseAssignment resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="22b08-105">ユーザーアカウントに割り当てるライセンス情報を表します。</span><span class="sxs-lookup"><span data-stu-id="22b08-105">Represents the license information to assign to user accounts.</span></span> <span data-ttu-id="22b08-106">リソースは、新しいユーザーアカウントの作成時にライセンスの割り当てを設定するために使用されます。</span><span class="sxs-lookup"><span data-stu-id="22b08-106">The resource will be used to set up license assignments when creating new user accounts.</span></span>

## <a name="properties"></a><span data-ttu-id="22b08-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="22b08-107">Properties</span></span>

| <span data-ttu-id="22b08-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="22b08-108">Property</span></span> | <span data-ttu-id="22b08-109">型</span><span class="sxs-lookup"><span data-stu-id="22b08-109">Type</span></span> | <span data-ttu-id="22b08-110">説明</span><span class="sxs-lookup"><span data-stu-id="22b08-110">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="22b08-111">**appliesTo**</span><span class="sxs-lookup"><span data-stu-id="22b08-111">**appliesTo**</span></span> | <span data-ttu-id="22b08-112">string</span><span class="sxs-lookup"><span data-stu-id="22b08-112">string</span></span> | <span data-ttu-id="22b08-113">ライセンスに割り当てるユーザーの役割の種類。</span><span class="sxs-lookup"><span data-stu-id="22b08-113">The user role type to assign to license.</span></span> <span data-ttu-id="22b08-114">可能な値は、`student`、`teacher` です。</span><span class="sxs-lookup"><span data-stu-id="22b08-114">Possible values are: `student`, `teacher`.</span></span>         |
| <span data-ttu-id="22b08-115">**skuids**</span><span class="sxs-lookup"><span data-stu-id="22b08-115">**skuIds**</span></span> | <span data-ttu-id="22b08-116">文字列のコレクション</span><span class="sxs-lookup"><span data-stu-id="22b08-116">collection of strings</span></span> |  <span data-ttu-id="22b08-117">割り当てるライセンスの SKU 識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="22b08-117">Represents the SKU identifiers of the licenses to assign.</span></span>        |

## <a name="json-representation"></a><span data-ttu-id="22b08-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="22b08-118">JSON representation</span></span>
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
