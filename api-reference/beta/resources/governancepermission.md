---
title: governancePermission リソースの種類
description: 'governanceSubject が特定の governanceResource に対して持つアクセス許可を表します。  '
localization_priority: Normal
ms.openlocfilehash: 255cd4c25a957a40e5e5ac765ed446f516c51607
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32547509"
---
# <a name="governancepermission-resource-type"></a><span data-ttu-id="cbf59-103">governancePermission リソースの種類</span><span class="sxs-lookup"><span data-stu-id="cbf59-103">governancePermission resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cbf59-104">[governanceSubject](../resources/governancesubject.md)が特定の[governanceResource](../resources/governanceresource.md)に対して持つアクセス許可を表します。</span><span class="sxs-lookup"><span data-stu-id="cbf59-104">Represents the access permission that a [governanceSubject](../resources/governancesubject.md) has to a specific [governanceResource](../resources/governanceresource.md).</span></span>  


## <a name="properties"></a><span data-ttu-id="cbf59-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cbf59-105">Properties</span></span>
| <span data-ttu-id="cbf59-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cbf59-106">Property</span></span>     | <span data-ttu-id="cbf59-107">型</span><span class="sxs-lookup"><span data-stu-id="cbf59-107">Type</span></span>   |<span data-ttu-id="cbf59-108">説明</span><span class="sxs-lookup"><span data-stu-id="cbf59-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cbf59-109">accessLevel</span><span class="sxs-lookup"><span data-stu-id="cbf59-109">accessLevel</span></span>|<span data-ttu-id="cbf59-110">String</span><span class="sxs-lookup"><span data-stu-id="cbf59-110">String</span></span>|<span data-ttu-id="cbf59-111">アクセスレベル。</span><span class="sxs-lookup"><span data-stu-id="cbf59-111">The access level.</span></span> <span data-ttu-id="cbf59-112">有効な値``None``は``UserRead``、 ``AdminRead``、、 ``AdminReadWrite``、です。</span><span class="sxs-lookup"><span data-stu-id="cbf59-112">Valid values: ``None``, ``UserRead``, ``AdminRead``, and ``AdminReadWrite``.</span></span>|
|<span data-ttu-id="cbf59-113">isActive</span><span class="sxs-lookup"><span data-stu-id="cbf59-113">isActive</span></span>|<span data-ttu-id="cbf59-114">ブール値</span><span class="sxs-lookup"><span data-stu-id="cbf59-114">Boolean</span></span>|<span data-ttu-id="cbf59-115">要求者がアクセスレベルに対してアクティブなロール割り当てを持っているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="cbf59-115">Indicate if the the requestor has any active role assignment for the access level.</span></span>|
|<span data-ttu-id="cbf59-116">isEligible</span><span class="sxs-lookup"><span data-stu-id="cbf59-116">isEligible</span></span>|<span data-ttu-id="cbf59-117">ブール値</span><span class="sxs-lookup"><span data-stu-id="cbf59-117">Boolean</span></span>|<span data-ttu-id="cbf59-118">要求者がアクセスレベルに対して適格な役割の割り当てを持っているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="cbf59-118">Indicate if the requestor has any eligible role assignment for the access level.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cbf59-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="cbf59-119">JSON representation</span></span>

<span data-ttu-id="cbf59-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="cbf59-120">Here is a JSON representation of the resource.</span></span>

```json
{
  "accessLevel": "String",
  "isActive": true,
  "isEligible": true
}

```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/governancepermission.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
