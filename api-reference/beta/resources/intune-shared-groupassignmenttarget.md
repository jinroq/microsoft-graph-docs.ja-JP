---
title: groupAssignmentTarget リソースの種類
description: グループへの割り当てを表します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 2039f5917aa5d69b74ccb6c1732496dc567ab673
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399424"
---
# <a name="groupassignmenttarget-resource-type"></a><span data-ttu-id="2c64d-103">groupAssignmentTarget リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2c64d-103">groupAssignmentTarget resource type</span></span>

> <span data-ttu-id="2c64d-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="2c64d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="2c64d-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2c64d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2c64d-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="2c64d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2c64d-107">グループへの割り当てを表します。</span><span class="sxs-lookup"><span data-stu-id="2c64d-107">Represents an assignment to a group.</span></span>


<span data-ttu-id="2c64d-108">[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="2c64d-108">Inherits from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="2c64d-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2c64d-109">Properties</span></span>
|<span data-ttu-id="2c64d-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2c64d-110">Property</span></span>|<span data-ttu-id="2c64d-111">型</span><span class="sxs-lookup"><span data-stu-id="2c64d-111">Type</span></span>|<span data-ttu-id="2c64d-112">説明</span><span class="sxs-lookup"><span data-stu-id="2c64d-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2c64d-113">groupId</span><span class="sxs-lookup"><span data-stu-id="2c64d-113">groupId</span></span>|<span data-ttu-id="2c64d-114">文字列</span><span class="sxs-lookup"><span data-stu-id="2c64d-114">String</span></span>|<span data-ttu-id="2c64d-115">割り当てのターゲットとなるグループ ID です。</span><span class="sxs-lookup"><span data-stu-id="2c64d-115">The group Id that is the target of the assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2c64d-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="2c64d-116">Relationships</span></span>
<span data-ttu-id="2c64d-117">なし</span><span class="sxs-lookup"><span data-stu-id="2c64d-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2c64d-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2c64d-118">JSON Representation</span></span>
<span data-ttu-id="2c64d-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="2c64d-119">Here is a JSON representation of the resource.</span></span>
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




