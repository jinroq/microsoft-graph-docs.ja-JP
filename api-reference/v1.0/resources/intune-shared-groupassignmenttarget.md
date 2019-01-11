---
title: groupAssignmentTarget リソースの種類
description: グループへの割り当てを表します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 7218fc69564ea08a7302cfb0af7856360cd9a330
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27809045"
---
# <a name="groupassignmenttarget-resource-type"></a><span data-ttu-id="425fb-103">groupAssignmentTarget リソースの種類</span><span class="sxs-lookup"><span data-stu-id="425fb-103">groupAssignmentTarget resource type</span></span>

> <span data-ttu-id="425fb-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="425fb-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="425fb-105">グループへの割り当てを表します。</span><span class="sxs-lookup"><span data-stu-id="425fb-105">Represents an assignment to a group.</span></span>

<span data-ttu-id="425fb-106">[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="425fb-106">Inherits from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="425fb-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="425fb-107">Properties</span></span>
|<span data-ttu-id="425fb-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="425fb-108">Property</span></span>|<span data-ttu-id="425fb-109">種類</span><span class="sxs-lookup"><span data-stu-id="425fb-109">Type</span></span>|<span data-ttu-id="425fb-110">説明</span><span class="sxs-lookup"><span data-stu-id="425fb-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="425fb-111">groupId</span><span class="sxs-lookup"><span data-stu-id="425fb-111">groupId</span></span>|<span data-ttu-id="425fb-112">文字列</span><span class="sxs-lookup"><span data-stu-id="425fb-112">String</span></span>|<span data-ttu-id="425fb-113">割り当てのターゲットとなるグループ ID です。</span><span class="sxs-lookup"><span data-stu-id="425fb-113">The group Id that is the target of the assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="425fb-114">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="425fb-114">Relationships</span></span>
<span data-ttu-id="425fb-115">なし</span><span class="sxs-lookup"><span data-stu-id="425fb-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="425fb-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="425fb-116">JSON Representation</span></span>
<span data-ttu-id="425fb-117">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="425fb-117">Here is a JSON representation of the resource.</span></span>
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



