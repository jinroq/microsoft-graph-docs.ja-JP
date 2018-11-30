---
title: groupAssignmentTarget リソースの種類
description: グループへの割り当てを表します。
ms.openlocfilehash: 0ebb41b1f737a20a37d322bac7ab5ae6ab2a248f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27022464"
---
# <a name="groupassignmenttarget-resource-type"></a><span data-ttu-id="0ccee-103">groupAssignmentTarget リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0ccee-103">groupAssignmentTarget resource type</span></span>

> <span data-ttu-id="0ccee-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="0ccee-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0ccee-105">グループへの割り当てを表します。</span><span class="sxs-lookup"><span data-stu-id="0ccee-105">Represents an assignment to a group.</span></span>

<span data-ttu-id="0ccee-106">[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="0ccee-106">Inherits from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0ccee-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0ccee-107">Properties</span></span>
|<span data-ttu-id="0ccee-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0ccee-108">Property</span></span>|<span data-ttu-id="0ccee-109">型</span><span class="sxs-lookup"><span data-stu-id="0ccee-109">Type</span></span>|<span data-ttu-id="0ccee-110">説明</span><span class="sxs-lookup"><span data-stu-id="0ccee-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0ccee-111">groupId</span><span class="sxs-lookup"><span data-stu-id="0ccee-111">groupId</span></span>|<span data-ttu-id="0ccee-112">文字列</span><span class="sxs-lookup"><span data-stu-id="0ccee-112">String</span></span>|<span data-ttu-id="0ccee-113">割り当てのターゲットとなるグループ ID です。</span><span class="sxs-lookup"><span data-stu-id="0ccee-113">The group Id that is the target of the assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0ccee-114">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0ccee-114">Relationships</span></span>
<span data-ttu-id="0ccee-115">なし</span><span class="sxs-lookup"><span data-stu-id="0ccee-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0ccee-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0ccee-116">JSON Representation</span></span>
<span data-ttu-id="0ccee-117">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0ccee-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.groupAssignmentTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupAssignmentTarget",
  "groupId": "String"
}
```



