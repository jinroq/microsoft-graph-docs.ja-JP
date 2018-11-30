---
title: exclusionGroupAssignmentTarget リソースの種類
description: 割り当てから除外するグループを表します。
ms.openlocfilehash: fdbb463687d75791965db2ef05abfea1a269d1a1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27022839"
---
# <a name="exclusiongroupassignmenttarget-resource-type"></a><span data-ttu-id="37225-103">exclusionGroupAssignmentTarget リソースの種類</span><span class="sxs-lookup"><span data-stu-id="37225-103">exclusionGroupAssignmentTarget resource type</span></span>

> <span data-ttu-id="37225-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="37225-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="37225-105">割り当てから除外するグループを表します。</span><span class="sxs-lookup"><span data-stu-id="37225-105">Represents a group that should be excluded from an assignment.</span></span>

<span data-ttu-id="37225-106">[groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="37225-106">Inherits from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="37225-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="37225-107">Properties</span></span>
|<span data-ttu-id="37225-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="37225-108">Property</span></span>|<span data-ttu-id="37225-109">型</span><span class="sxs-lookup"><span data-stu-id="37225-109">Type</span></span>|<span data-ttu-id="37225-110">説明</span><span class="sxs-lookup"><span data-stu-id="37225-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="37225-111">groupId</span><span class="sxs-lookup"><span data-stu-id="37225-111">groupId</span></span>|<span data-ttu-id="37225-112">文字列</span><span class="sxs-lookup"><span data-stu-id="37225-112">String</span></span>|<span data-ttu-id="37225-113">割り当てのターゲットとなるグループ ID です。</span><span class="sxs-lookup"><span data-stu-id="37225-113">The group Id that is the target of the assignment.</span></span> <span data-ttu-id="37225-114">[groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="37225-114">Inherited from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="37225-115">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="37225-115">Relationships</span></span>
<span data-ttu-id="37225-116">なし</span><span class="sxs-lookup"><span data-stu-id="37225-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="37225-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="37225-117">JSON Representation</span></span>
<span data-ttu-id="37225-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="37225-118">Here is a JSON representation of the resource.</span></span>
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



