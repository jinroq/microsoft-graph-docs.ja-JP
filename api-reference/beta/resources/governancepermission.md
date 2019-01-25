---
title: governancePermission リソースの種類
description: '特定の governanceResource に、governanceSubject を持つアクセス許可を表します。  '
localization_priority: Normal
ms.openlocfilehash: 255cd4c25a957a40e5e5ac765ed446f516c51607
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529839"
---
# <a name="governancepermission-resource-type"></a><span data-ttu-id="44e41-103">governancePermission リソースの種類</span><span class="sxs-lookup"><span data-stu-id="44e41-103">governancePermission resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="44e41-104">特定の[governanceResource](../resources/governanceresource.md)に、 [governanceSubject](../resources/governancesubject.md)を持つアクセス許可を表します。</span><span class="sxs-lookup"><span data-stu-id="44e41-104">Represents the access permission that a [governanceSubject](../resources/governancesubject.md) has to a specific [governanceResource](../resources/governanceresource.md).</span></span>  


## <a name="properties"></a><span data-ttu-id="44e41-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="44e41-105">Properties</span></span>
| <span data-ttu-id="44e41-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="44e41-106">Property</span></span>     | <span data-ttu-id="44e41-107">型</span><span class="sxs-lookup"><span data-stu-id="44e41-107">Type</span></span>   |<span data-ttu-id="44e41-108">説明</span><span class="sxs-lookup"><span data-stu-id="44e41-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="44e41-109">AccessLevel</span><span class="sxs-lookup"><span data-stu-id="44e41-109">accessLevel</span></span>|<span data-ttu-id="44e41-110">String</span><span class="sxs-lookup"><span data-stu-id="44e41-110">String</span></span>|<span data-ttu-id="44e41-111">アクセス レベルです。</span><span class="sxs-lookup"><span data-stu-id="44e41-111">The access level.</span></span> <span data-ttu-id="44e41-112">有効な値: ``None``、 ``UserRead``、``AdminRead``と``AdminReadWrite``。</span><span class="sxs-lookup"><span data-stu-id="44e41-112">Valid values: ``None``, ``UserRead``, ``AdminRead``, and ``AdminReadWrite``.</span></span>|
|<span data-ttu-id="44e41-113">isActive</span><span class="sxs-lookup"><span data-stu-id="44e41-113">isActive</span></span>|<span data-ttu-id="44e41-114">ブール値</span><span class="sxs-lookup"><span data-stu-id="44e41-114">Boolean</span></span>|<span data-ttu-id="44e41-115">指定する場合、リクエスターが、アクティブなロールの割り当てのアクセス レベルを持ちます。</span><span class="sxs-lookup"><span data-stu-id="44e41-115">Indicate if the the requestor has any active role assignment for the access level.</span></span>|
|<span data-ttu-id="44e41-116">isEligible</span><span class="sxs-lookup"><span data-stu-id="44e41-116">isEligible</span></span>|<span data-ttu-id="44e41-117">ブール値</span><span class="sxs-lookup"><span data-stu-id="44e41-117">Boolean</span></span>|<span data-ttu-id="44e41-118">リクエスターは、対象となるロールの割り当てのアクセス レベルを指定します。</span><span class="sxs-lookup"><span data-stu-id="44e41-118">Indicate if the requestor has any eligible role assignment for the access level.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="44e41-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="44e41-119">JSON representation</span></span>

<span data-ttu-id="44e41-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="44e41-120">Here is a JSON representation of the resource.</span></span>

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
