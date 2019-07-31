---
title: educationSynchronizationLicenseAssignment リソースの種類
description: ユーザーアカウントに割り当てるライセンス情報を表します。 リソースは、新しいユーザーアカウントの作成時にライセンスの割り当てを設定するために使用されます。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: b00550c1a4d2d02efc983ab345fbc429b443a5bf
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972398"
---
# <a name="educationsynchronizationlicenseassignment-resource-type"></a><span data-ttu-id="51fd7-104">educationSynchronizationLicenseAssignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="51fd7-104">educationSynchronizationLicenseAssignment resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="51fd7-105">ユーザーアカウントに割り当てるライセンス情報を表します。</span><span class="sxs-lookup"><span data-stu-id="51fd7-105">Represents the license information to assign to user accounts.</span></span> <span data-ttu-id="51fd7-106">リソースは、新しいユーザーアカウントの作成時にライセンスの割り当てを設定するために使用されます。</span><span class="sxs-lookup"><span data-stu-id="51fd7-106">The resource will be used to set up license assignments when creating new user accounts.</span></span>

## <a name="properties"></a><span data-ttu-id="51fd7-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="51fd7-107">Properties</span></span>

| <span data-ttu-id="51fd7-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="51fd7-108">Property</span></span> | <span data-ttu-id="51fd7-109">型</span><span class="sxs-lookup"><span data-stu-id="51fd7-109">Type</span></span> | <span data-ttu-id="51fd7-110">説明</span><span class="sxs-lookup"><span data-stu-id="51fd7-110">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="51fd7-111">**appliesTo**</span><span class="sxs-lookup"><span data-stu-id="51fd7-111">**appliesTo**</span></span> | <span data-ttu-id="51fd7-112">string</span><span class="sxs-lookup"><span data-stu-id="51fd7-112">string</span></span> | <span data-ttu-id="51fd7-113">ライセンスに割り当てるユーザーの役割の種類。</span><span class="sxs-lookup"><span data-stu-id="51fd7-113">The user role type to assign to license.</span></span> <span data-ttu-id="51fd7-114">可能な値は、`student`、`teacher`、`faculty` です。</span><span class="sxs-lookup"><span data-stu-id="51fd7-114">Possible values are: `student`, `teacher`, `faculty`.</span></span>         |
| <span data-ttu-id="51fd7-115">**skuIds**</span><span class="sxs-lookup"><span data-stu-id="51fd7-115">**skuIds**</span></span> | <span data-ttu-id="51fd7-116">文字列のコレクション</span><span class="sxs-lookup"><span data-stu-id="51fd7-116">collection of strings</span></span> |  <span data-ttu-id="51fd7-117">割り当てるライセンスの SKU 識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="51fd7-117">Represents the SKU identifiers of the licenses to assign.</span></span>        |

## <a name="json-representation"></a><span data-ttu-id="51fd7-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="51fd7-118">JSON representation</span></span>
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
