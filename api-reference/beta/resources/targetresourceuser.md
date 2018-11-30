---
title: targetResourceUser リソースの種類
description: 追加、更新または監査活動の一環として、管理者によって削除されたユーザー オブジェクトを示します。 TargetResource リソースから派生します。
ms.openlocfilehash: 632d0551b3aba434c3309c8c874947708eb9a9f5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069763"
---
# <a name="targetresourceuser-resource-type"></a><span data-ttu-id="5667f-104">targetResourceUser リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5667f-104">targetResourceUser resource type</span></span>
<span data-ttu-id="5667f-105">追加、更新または監査活動の一環として、管理者によって削除されたユーザー オブジェクトを示します。</span><span class="sxs-lookup"><span data-stu-id="5667f-105">Indicates the user object that was added, updated or deleted by admins as part of audit activity.</span></span> <span data-ttu-id="5667f-106">[TargetResource](targetresource.md)リソースから派生します。</span><span class="sxs-lookup"><span data-stu-id="5667f-106">Derived from the [targetResource](targetresource.md) resource.</span></span>


## <a name="properties"></a><span data-ttu-id="5667f-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5667f-107">Properties</span></span>
| <span data-ttu-id="5667f-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5667f-108">Property</span></span>     | <span data-ttu-id="5667f-109">型</span><span class="sxs-lookup"><span data-stu-id="5667f-109">Type</span></span>   |<span data-ttu-id="5667f-110">説明</span><span class="sxs-lookup"><span data-stu-id="5667f-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5667f-111">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="5667f-111">userPrincipalName</span></span>|<span data-ttu-id="5667f-112">String</span><span class="sxs-lookup"><span data-stu-id="5667f-112">String</span></span>|<span data-ttu-id="5667f-113">ユーザーの一意の Id を示します。</span><span class="sxs-lookup"><span data-stu-id="5667f-113">Indicates the Unique Id of the User.</span></span> <span data-ttu-id="5667f-114">特定のユーザーのユーザー Id を参照します。</span><span class="sxs-lookup"><span data-stu-id="5667f-114">Refers to User Id for a specific user.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5667f-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5667f-115">JSON representation</span></span>

<span data-ttu-id="5667f-116">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="5667f-116">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.targetResourceUser"
}-->

```json
{
  "userPrincipalName": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "targetResourceUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->