---
title: windowsAutopilotDeploymentProfileAssignment リソースの種類
description: AAD グループに Windows の自動操縦装置の展開のプロファイルの割り当て。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: ec24363dbf245ce261cdbd534ef00f501af1d8ad
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29406011"
---
# <a name="windowsautopilotdeploymentprofileassignment-resource-type"></a><span data-ttu-id="af7fe-103">windowsAutopilotDeploymentProfileAssignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="af7fe-103">windowsAutopilotDeploymentProfileAssignment resource type</span></span>

> <span data-ttu-id="af7fe-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="af7fe-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="af7fe-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="af7fe-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="af7fe-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="af7fe-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="af7fe-107">AAD グループに Windows の自動操縦装置の展開のプロファイルの割り当て。</span><span class="sxs-lookup"><span data-stu-id="af7fe-107">An assignment of a Windows Autopilot deployment profile to an AAD group.</span></span>

## <a name="methods"></a><span data-ttu-id="af7fe-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="af7fe-108">Methods</span></span>
|<span data-ttu-id="af7fe-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="af7fe-109">Method</span></span>|<span data-ttu-id="af7fe-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="af7fe-110">Return Type</span></span>|<span data-ttu-id="af7fe-111">説明</span><span class="sxs-lookup"><span data-stu-id="af7fe-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="af7fe-112">リスト windowsAutopilotDeploymentProfileAssignments</span><span class="sxs-lookup"><span data-stu-id="af7fe-112">List windowsAutopilotDeploymentProfileAssignments</span></span>](../api/intune-enrollment-windowsautopilotdeploymentprofileassignment-list.md)|<span data-ttu-id="af7fe-113">[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="af7fe-113">[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) collection</span></span>|<span data-ttu-id="af7fe-114">[WindowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="af7fe-114">List properties and relationships of the [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) objects.</span></span>|
|[<span data-ttu-id="af7fe-115">WindowsAutopilotDeploymentProfileAssignment を取得します。</span><span class="sxs-lookup"><span data-stu-id="af7fe-115">Get windowsAutopilotDeploymentProfileAssignment</span></span>](../api/intune-enrollment-windowsautopilotdeploymentprofileassignment-get.md)|[<span data-ttu-id="af7fe-116">windowsAutopilotDeploymentProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="af7fe-116">windowsAutopilotDeploymentProfileAssignment</span></span>](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)|<span data-ttu-id="af7fe-117">[WindowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="af7fe-117">Read properties and relationships of the [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object.</span></span>|
|[<span data-ttu-id="af7fe-118">WindowsAutopilotDeploymentProfileAssignment を作成します。</span><span class="sxs-lookup"><span data-stu-id="af7fe-118">Create windowsAutopilotDeploymentProfileAssignment</span></span>](../api/intune-enrollment-windowsautopilotdeploymentprofileassignment-create.md)|[<span data-ttu-id="af7fe-119">windowsAutopilotDeploymentProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="af7fe-119">windowsAutopilotDeploymentProfileAssignment</span></span>](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)|<span data-ttu-id="af7fe-120">新しい[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="af7fe-120">Create a new [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object.</span></span>|
|[<span data-ttu-id="af7fe-121">WindowsAutopilotDeploymentProfileAssignment を削除します。</span><span class="sxs-lookup"><span data-stu-id="af7fe-121">Delete windowsAutopilotDeploymentProfileAssignment</span></span>](../api/intune-enrollment-windowsautopilotdeploymentprofileassignment-delete.md)|<span data-ttu-id="af7fe-122">なし</span><span class="sxs-lookup"><span data-stu-id="af7fe-122">None</span></span>|<span data-ttu-id="af7fe-123">の[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="af7fe-123">Deletes a [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md).</span></span>|
|[<span data-ttu-id="af7fe-124">WindowsAutopilotDeploymentProfileAssignment を更新します。</span><span class="sxs-lookup"><span data-stu-id="af7fe-124">Update windowsAutopilotDeploymentProfileAssignment</span></span>](../api/intune-enrollment-windowsautopilotdeploymentprofileassignment-update.md)|[<span data-ttu-id="af7fe-125">windowsAutopilotDeploymentProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="af7fe-125">windowsAutopilotDeploymentProfileAssignment</span></span>](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)|<span data-ttu-id="af7fe-126">[WindowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="af7fe-126">Update the properties of a [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="af7fe-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="af7fe-127">Properties</span></span>
|<span data-ttu-id="af7fe-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="af7fe-128">Property</span></span>|<span data-ttu-id="af7fe-129">型</span><span class="sxs-lookup"><span data-stu-id="af7fe-129">Type</span></span>|<span data-ttu-id="af7fe-130">説明</span><span class="sxs-lookup"><span data-stu-id="af7fe-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="af7fe-131">id</span><span class="sxs-lookup"><span data-stu-id="af7fe-131">id</span></span>|<span data-ttu-id="af7fe-132">String</span><span class="sxs-lookup"><span data-stu-id="af7fe-132">String</span></span>|<span data-ttu-id="af7fe-133">割り当てのキー。</span><span class="sxs-lookup"><span data-stu-id="af7fe-133">The key of the assignment.</span></span>|
|<span data-ttu-id="af7fe-134">target</span><span class="sxs-lookup"><span data-stu-id="af7fe-134">target</span></span>|[<span data-ttu-id="af7fe-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="af7fe-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="af7fe-136">Windows の自動操縦装置の配置のプロファイルの割り当てのターゲットです。</span><span class="sxs-lookup"><span data-stu-id="af7fe-136">The assignment target for the Windows Autopilot deployment profile.</span></span>|

## <a name="relationships"></a><span data-ttu-id="af7fe-137">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="af7fe-137">Relationships</span></span>
<span data-ttu-id="af7fe-138">なし</span><span class="sxs-lookup"><span data-stu-id="af7fe-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="af7fe-139">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="af7fe-139">JSON Representation</span></span>
<span data-ttu-id="af7fe-140">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="af7fe-140">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsAutopilotDeploymentProfileAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsAutopilotDeploymentProfileAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```




