---
title: educationSynchronizationLicenseAssignment リソースの種類
description: ユーザーアカウントに割り当てるライセンス情報を表します。 リソースは、新しいユーザーアカウントの作成時にライセンスの割り当てを設定するために使用されます。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: ce1ae196ba4f014a039e81713119b01fa69e6170
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507099"
---
# <a name="educationsynchronizationlicenseassignment-resource-type"></a><span data-ttu-id="f045c-104">educationSynchronizationLicenseAssignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f045c-104">educationSynchronizationLicenseAssignment resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f045c-105">ユーザーアカウントに割り当てるライセンス情報を表します。</span><span class="sxs-lookup"><span data-stu-id="f045c-105">Represents the license information to assign to user accounts.</span></span> <span data-ttu-id="f045c-106">リソースは、新しいユーザーアカウントの作成時にライセンスの割り当てを設定するために使用されます。</span><span class="sxs-lookup"><span data-stu-id="f045c-106">The resource will be used to set up license assignments when creating new user accounts.</span></span>

## <a name="properties"></a><span data-ttu-id="f045c-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f045c-107">Properties</span></span>

| <span data-ttu-id="f045c-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f045c-108">Property</span></span> | <span data-ttu-id="f045c-109">型</span><span class="sxs-lookup"><span data-stu-id="f045c-109">Type</span></span> | <span data-ttu-id="f045c-110">説明</span><span class="sxs-lookup"><span data-stu-id="f045c-110">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="f045c-111">**appliesTo**</span><span class="sxs-lookup"><span data-stu-id="f045c-111">**appliesTo**</span></span> | <span data-ttu-id="f045c-112">string</span><span class="sxs-lookup"><span data-stu-id="f045c-112">string</span></span> | <span data-ttu-id="f045c-113">ライセンスに割り当てるユーザーの役割の種類。</span><span class="sxs-lookup"><span data-stu-id="f045c-113">The user role type to assign to license.</span></span> <span data-ttu-id="f045c-114">可能な値は、`student`、`teacher` です。</span><span class="sxs-lookup"><span data-stu-id="f045c-114">Possible values are: `student`, `teacher`.</span></span>         |
| <span data-ttu-id="f045c-115">**skuids**</span><span class="sxs-lookup"><span data-stu-id="f045c-115">**skuIds**</span></span> | <span data-ttu-id="f045c-116">文字列のコレクション</span><span class="sxs-lookup"><span data-stu-id="f045c-116">collection of strings</span></span> |  <span data-ttu-id="f045c-117">割り当てるライセンスの SKU 識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="f045c-117">Represents the SKU identifiers of the licenses to assign.</span></span>        |

## <a name="json-representation"></a><span data-ttu-id="f045c-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f045c-118">JSON representation</span></span>
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
