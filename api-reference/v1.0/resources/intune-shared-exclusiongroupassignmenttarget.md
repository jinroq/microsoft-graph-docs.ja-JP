---
title: exclusionGroupAssignmentTarget リソースの種類
description: 割り当てから除外するグループを表します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 2d2d6b004b6dbd78b43d4cab1c06e960d43f30d7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27917224"
---
# <a name="exclusiongroupassignmenttarget-resource-type"></a><span data-ttu-id="95ae9-103">exclusionGroupAssignmentTarget リソースの種類</span><span class="sxs-lookup"><span data-stu-id="95ae9-103">exclusionGroupAssignmentTarget resource type</span></span>

> <span data-ttu-id="95ae9-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="95ae9-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="95ae9-105">割り当てから除外するグループを表します。</span><span class="sxs-lookup"><span data-stu-id="95ae9-105">Represents a group that should be excluded from an assignment.</span></span>

<span data-ttu-id="95ae9-106">[groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="95ae9-106">Inherits from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="95ae9-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="95ae9-107">Properties</span></span>
|<span data-ttu-id="95ae9-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="95ae9-108">Property</span></span>|<span data-ttu-id="95ae9-109">種類</span><span class="sxs-lookup"><span data-stu-id="95ae9-109">Type</span></span>|<span data-ttu-id="95ae9-110">説明</span><span class="sxs-lookup"><span data-stu-id="95ae9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="95ae9-111">groupId</span><span class="sxs-lookup"><span data-stu-id="95ae9-111">groupId</span></span>|<span data-ttu-id="95ae9-112">文字列</span><span class="sxs-lookup"><span data-stu-id="95ae9-112">String</span></span>|<span data-ttu-id="95ae9-113">割り当てのターゲットとなるグループ ID です。</span><span class="sxs-lookup"><span data-stu-id="95ae9-113">The group Id that is the target of the assignment.</span></span> <span data-ttu-id="95ae9-114">[groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="95ae9-114">Inherited from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="95ae9-115">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="95ae9-115">Relationships</span></span>
<span data-ttu-id="95ae9-116">なし</span><span class="sxs-lookup"><span data-stu-id="95ae9-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="95ae9-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="95ae9-117">JSON Representation</span></span>
<span data-ttu-id="95ae9-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="95ae9-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.exclusionGroupAssignmentTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.exclusionGroupAssignmentTarget",
  "groupId": "String"
}
```



