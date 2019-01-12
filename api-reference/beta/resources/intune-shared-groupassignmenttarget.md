---
title: groupAssignmentTarget リソースの種類
description: グループへの割り当てを表します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 96aec1b72233cfe7d553b8f17feb9af382d89cde
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27971677"
---
# <a name="groupassignmenttarget-resource-type"></a><span data-ttu-id="7d5e3-103">groupAssignmentTarget リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7d5e3-103">groupAssignmentTarget resource type</span></span>

> <span data-ttu-id="7d5e3-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="7d5e3-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7d5e3-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7d5e3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7d5e3-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="7d5e3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7d5e3-107">グループへの割り当てを表します。</span><span class="sxs-lookup"><span data-stu-id="7d5e3-107">Represents an assignment to a group.</span></span>

<span data-ttu-id="7d5e3-108">[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="7d5e3-108">Inherits from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="7d5e3-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7d5e3-109">Properties</span></span>
|<span data-ttu-id="7d5e3-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7d5e3-110">Property</span></span>|<span data-ttu-id="7d5e3-111">種類</span><span class="sxs-lookup"><span data-stu-id="7d5e3-111">Type</span></span>|<span data-ttu-id="7d5e3-112">説明</span><span class="sxs-lookup"><span data-stu-id="7d5e3-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7d5e3-113">groupId</span><span class="sxs-lookup"><span data-stu-id="7d5e3-113">groupId</span></span>|<span data-ttu-id="7d5e3-114">文字列</span><span class="sxs-lookup"><span data-stu-id="7d5e3-114">String</span></span>|<span data-ttu-id="7d5e3-115">割り当てのターゲットとなるグループ ID です。</span><span class="sxs-lookup"><span data-stu-id="7d5e3-115">The group Id that is the target of the assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7d5e3-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="7d5e3-116">Relationships</span></span>
<span data-ttu-id="7d5e3-117">なし</span><span class="sxs-lookup"><span data-stu-id="7d5e3-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="7d5e3-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7d5e3-118">JSON Representation</span></span>
<span data-ttu-id="7d5e3-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="7d5e3-119">Here is a JSON representation of the resource.</span></span>
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





