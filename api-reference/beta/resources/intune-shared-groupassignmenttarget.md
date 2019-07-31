---
title: groupAssignmentTarget リソースの種類
description: グループへの割り当てを表します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 62de6a0a085fda974d9f8140aa2961e6a3610cb4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35967428"
---
# <a name="groupassignmenttarget-resource-type"></a><span data-ttu-id="32e83-103">groupAssignmentTarget リソースの種類</span><span class="sxs-lookup"><span data-stu-id="32e83-103">groupAssignmentTarget resource type</span></span>

> <span data-ttu-id="32e83-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="32e83-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="32e83-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="32e83-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="32e83-106">グループへの割り当てを表します。</span><span class="sxs-lookup"><span data-stu-id="32e83-106">Represents an assignment to a group.</span></span>


<span data-ttu-id="32e83-107">[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="32e83-107">Inherits from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="32e83-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="32e83-108">Properties</span></span>
|<span data-ttu-id="32e83-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="32e83-109">Property</span></span>|<span data-ttu-id="32e83-110">型</span><span class="sxs-lookup"><span data-stu-id="32e83-110">Type</span></span>|<span data-ttu-id="32e83-111">説明</span><span class="sxs-lookup"><span data-stu-id="32e83-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="32e83-112">groupId</span><span class="sxs-lookup"><span data-stu-id="32e83-112">groupId</span></span>|<span data-ttu-id="32e83-113">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="32e83-113">String</span></span>|<span data-ttu-id="32e83-114">割り当てのターゲットとなるグループ ID です。</span><span class="sxs-lookup"><span data-stu-id="32e83-114">The group Id that is the target of the assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="32e83-115">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="32e83-115">Relationships</span></span>
<span data-ttu-id="32e83-116">なし</span><span class="sxs-lookup"><span data-stu-id="32e83-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="32e83-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="32e83-117">JSON Representation</span></span>
<span data-ttu-id="32e83-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="32e83-118">Here is a JSON representation of the resource.</span></span>
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





