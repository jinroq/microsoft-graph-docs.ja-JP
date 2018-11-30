---
title: groupAssignmentTarget リソースの種類
description: グループへの割り当てを表します。
ms.openlocfilehash: 76ea8c56b8022dc832335c575ad52632894f1d60
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067178"
---
# <a name="groupassignmenttarget-resource-type"></a><span data-ttu-id="b7a28-103">groupAssignmentTarget リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b7a28-103">groupAssignmentTarget resource type</span></span>

> <span data-ttu-id="b7a28-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b7a28-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b7a28-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b7a28-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b7a28-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b7a28-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b7a28-107">グループへの割り当てを表します。</span><span class="sxs-lookup"><span data-stu-id="b7a28-107">Represents an assignment to a group.</span></span>

<span data-ttu-id="b7a28-108">[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="b7a28-108">Inherits from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b7a28-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b7a28-109">Properties</span></span>
|<span data-ttu-id="b7a28-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b7a28-110">Property</span></span>|<span data-ttu-id="b7a28-111">型</span><span class="sxs-lookup"><span data-stu-id="b7a28-111">Type</span></span>|<span data-ttu-id="b7a28-112">説明</span><span class="sxs-lookup"><span data-stu-id="b7a28-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b7a28-113">groupId</span><span class="sxs-lookup"><span data-stu-id="b7a28-113">groupId</span></span>|<span data-ttu-id="b7a28-114">文字列</span><span class="sxs-lookup"><span data-stu-id="b7a28-114">String</span></span>|<span data-ttu-id="b7a28-115">割り当てのターゲットとなるグループ ID です。</span><span class="sxs-lookup"><span data-stu-id="b7a28-115">The group Id that is the target of the assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b7a28-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b7a28-116">Relationships</span></span>
<span data-ttu-id="b7a28-117">なし</span><span class="sxs-lookup"><span data-stu-id="b7a28-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b7a28-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b7a28-118">JSON Representation</span></span>
<span data-ttu-id="b7a28-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b7a28-119">Here is a JSON representation of the resource.</span></span>
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





