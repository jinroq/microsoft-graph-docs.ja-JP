---
title: groupAssignmentTarget リソースの種類
description: グループへの割り当てを表します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 24ac3c4519cc074c3cce423ca5d0745c8a78d865
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32571920"
---
# <a name="groupassignmenttarget-resource-type"></a><span data-ttu-id="aee23-103">groupAssignmentTarget リソースの種類</span><span class="sxs-lookup"><span data-stu-id="aee23-103">groupAssignmentTarget resource type</span></span>

> <span data-ttu-id="aee23-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="aee23-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aee23-105">グループへの割り当てを表します。</span><span class="sxs-lookup"><span data-stu-id="aee23-105">Represents an assignment to a group.</span></span>


<span data-ttu-id="aee23-106">[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="aee23-106">Inherits from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="aee23-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="aee23-107">Properties</span></span>
|<span data-ttu-id="aee23-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="aee23-108">Property</span></span>|<span data-ttu-id="aee23-109">型</span><span class="sxs-lookup"><span data-stu-id="aee23-109">Type</span></span>|<span data-ttu-id="aee23-110">説明</span><span class="sxs-lookup"><span data-stu-id="aee23-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aee23-111">groupId</span><span class="sxs-lookup"><span data-stu-id="aee23-111">groupId</span></span>|<span data-ttu-id="aee23-112">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="aee23-112">String</span></span>|<span data-ttu-id="aee23-113">割り当てのターゲットとなるグループ ID です。</span><span class="sxs-lookup"><span data-stu-id="aee23-113">The group Id that is the target of the assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="aee23-114">関係</span><span class="sxs-lookup"><span data-stu-id="aee23-114">Relationships</span></span>
<span data-ttu-id="aee23-115">なし</span><span class="sxs-lookup"><span data-stu-id="aee23-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="aee23-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="aee23-116">JSON Representation</span></span>
<span data-ttu-id="aee23-117">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="aee23-117">Here is a JSON representation of the resource.</span></span>
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



