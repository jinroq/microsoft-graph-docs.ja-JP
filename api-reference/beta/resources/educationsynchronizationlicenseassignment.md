---
title: educationSynchronizationLicenseAssignment リソースの種類
description: ユーザー アカウントに割り当てるにはライセンス情報を表します。 新しいユーザー アカウントを作成するときに、ライセンスの割り当てを設定するのには、リソースが使用されます。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: ce1ae196ba4f014a039e81713119b01fa69e6170
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525823"
---
# <a name="educationsynchronizationlicenseassignment-resource-type"></a><span data-ttu-id="78c32-104">educationSynchronizationLicenseAssignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="78c32-104">educationSynchronizationLicenseAssignment resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="78c32-105">ユーザー アカウントに割り当てるにはライセンス情報を表します。</span><span class="sxs-lookup"><span data-stu-id="78c32-105">Represents the license information to assign to user accounts.</span></span> <span data-ttu-id="78c32-106">新しいユーザー アカウントを作成するときに、ライセンスの割り当てを設定するのには、リソースが使用されます。</span><span class="sxs-lookup"><span data-stu-id="78c32-106">The resource will be used to set up license assignments when creating new user accounts.</span></span>

## <a name="properties"></a><span data-ttu-id="78c32-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="78c32-107">Properties</span></span>

| <span data-ttu-id="78c32-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="78c32-108">Property</span></span> | <span data-ttu-id="78c32-109">型</span><span class="sxs-lookup"><span data-stu-id="78c32-109">Type</span></span> | <span data-ttu-id="78c32-110">説明</span><span class="sxs-lookup"><span data-stu-id="78c32-110">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="78c32-111">appliesTo</span><span class="sxs-lookup"><span data-stu-id="78c32-111">**appliesTo**</span></span> | <span data-ttu-id="78c32-112">string</span><span class="sxs-lookup"><span data-stu-id="78c32-112">string</span></span> | <span data-ttu-id="78c32-113">ライセンスを割り当てるにはユーザーのロールの種類です。</span><span class="sxs-lookup"><span data-stu-id="78c32-113">The user role type to assign to license.</span></span> <span data-ttu-id="78c32-114">使用可能な値は、`student`、`teacher` です。</span><span class="sxs-lookup"><span data-stu-id="78c32-114">Possible values are: `student`, `teacher`.</span></span>         |
| <span data-ttu-id="78c32-115">**skuIds**</span><span class="sxs-lookup"><span data-stu-id="78c32-115">**skuIds**</span></span> | <span data-ttu-id="78c32-116">文字列のコレクション</span><span class="sxs-lookup"><span data-stu-id="78c32-116">collection of strings</span></span> |  <span data-ttu-id="78c32-117">割り当てるライセンスの SKU 識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="78c32-117">Represents the SKU identifiers of the licenses to assign.</span></span>        |

## <a name="json-representation"></a><span data-ttu-id="78c32-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="78c32-118">JSON representation</span></span>
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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationsynchronizationlicenseassignment.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
