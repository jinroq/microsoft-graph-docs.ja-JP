---
title: windowsAutopilotDeploymentProfileAssignment リソースの種類
description: AAD グループへの Windows 自動操縦展開プロファイルの割り当て。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 884f233908f1757fc775cd302fcdd95a8ed38f32
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34993895"
---
# <a name="windowsautopilotdeploymentprofileassignment-resource-type"></a><span data-ttu-id="eca98-103">windowsAutopilotDeploymentProfileAssignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="eca98-103">windowsAutopilotDeploymentProfileAssignment resource type</span></span>

> <span data-ttu-id="eca98-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="eca98-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eca98-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="eca98-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eca98-106">AAD グループへの Windows 自動操縦展開プロファイルの割り当て。</span><span class="sxs-lookup"><span data-stu-id="eca98-106">An assignment of a Windows Autopilot deployment profile to an AAD group.</span></span>

## <a name="methods"></a><span data-ttu-id="eca98-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="eca98-107">Methods</span></span>
|<span data-ttu-id="eca98-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="eca98-108">Method</span></span>|<span data-ttu-id="eca98-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="eca98-109">Return Type</span></span>|<span data-ttu-id="eca98-110">説明</span><span class="sxs-lookup"><span data-stu-id="eca98-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="eca98-111">リスト windowsAutopilotDeploymentProfileAssignments</span><span class="sxs-lookup"><span data-stu-id="eca98-111">List windowsAutopilotDeploymentProfileAssignments</span></span>](../api/intune-enrollment-windowsautopilotdeploymentprofileassignment-list.md)|<span data-ttu-id="eca98-112">[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="eca98-112">[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) collection</span></span>|<span data-ttu-id="eca98-113">[WindowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="eca98-113">List properties and relationships of the [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) objects.</span></span>|
|[<span data-ttu-id="eca98-114">WindowsAutopilotDeploymentProfileAssignment を取得する</span><span class="sxs-lookup"><span data-stu-id="eca98-114">Get windowsAutopilotDeploymentProfileAssignment</span></span>](../api/intune-enrollment-windowsautopilotdeploymentprofileassignment-get.md)|[<span data-ttu-id="eca98-115">windowsAutopilotDeploymentProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="eca98-115">windowsAutopilotDeploymentProfileAssignment</span></span>](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)|<span data-ttu-id="eca98-116">[WindowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="eca98-116">Read properties and relationships of the [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object.</span></span>|
|[<span data-ttu-id="eca98-117">WindowsAutopilotDeploymentProfileAssignment を作成する</span><span class="sxs-lookup"><span data-stu-id="eca98-117">Create windowsAutopilotDeploymentProfileAssignment</span></span>](../api/intune-enrollment-windowsautopilotdeploymentprofileassignment-create.md)|[<span data-ttu-id="eca98-118">windowsAutopilotDeploymentProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="eca98-118">windowsAutopilotDeploymentProfileAssignment</span></span>](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)|<span data-ttu-id="eca98-119">新しい[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="eca98-119">Create a new [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object.</span></span>|
|[<span data-ttu-id="eca98-120">WindowsAutopilotDeploymentProfileAssignment の削除</span><span class="sxs-lookup"><span data-stu-id="eca98-120">Delete windowsAutopilotDeploymentProfileAssignment</span></span>](../api/intune-enrollment-windowsautopilotdeploymentprofileassignment-delete.md)|<span data-ttu-id="eca98-121">None</span><span class="sxs-lookup"><span data-stu-id="eca98-121">None</span></span>|<span data-ttu-id="eca98-122">[WindowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="eca98-122">Deletes a [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md).</span></span>|
|[<span data-ttu-id="eca98-123">WindowsAutopilotDeploymentProfileAssignment の更新</span><span class="sxs-lookup"><span data-stu-id="eca98-123">Update windowsAutopilotDeploymentProfileAssignment</span></span>](../api/intune-enrollment-windowsautopilotdeploymentprofileassignment-update.md)|[<span data-ttu-id="eca98-124">windowsAutopilotDeploymentProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="eca98-124">windowsAutopilotDeploymentProfileAssignment</span></span>](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)|<span data-ttu-id="eca98-125">[WindowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="eca98-125">Update the properties of a [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="eca98-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="eca98-126">Properties</span></span>
|<span data-ttu-id="eca98-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="eca98-127">Property</span></span>|<span data-ttu-id="eca98-128">型</span><span class="sxs-lookup"><span data-stu-id="eca98-128">Type</span></span>|<span data-ttu-id="eca98-129">説明</span><span class="sxs-lookup"><span data-stu-id="eca98-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eca98-130">id</span><span class="sxs-lookup"><span data-stu-id="eca98-130">id</span></span>|<span data-ttu-id="eca98-131">String</span><span class="sxs-lookup"><span data-stu-id="eca98-131">String</span></span>|<span data-ttu-id="eca98-132">割り当てのキー。</span><span class="sxs-lookup"><span data-stu-id="eca98-132">The key of the assignment.</span></span>|
|<span data-ttu-id="eca98-133">target</span><span class="sxs-lookup"><span data-stu-id="eca98-133">target</span></span>|[<span data-ttu-id="eca98-134">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="eca98-134">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="eca98-135">Windows 自動操縦展開プロファイルの割り当て先。</span><span class="sxs-lookup"><span data-stu-id="eca98-135">The assignment target for the Windows Autopilot deployment profile.</span></span>|

## <a name="relationships"></a><span data-ttu-id="eca98-136">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="eca98-136">Relationships</span></span>
<span data-ttu-id="eca98-137">なし</span><span class="sxs-lookup"><span data-stu-id="eca98-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="eca98-138">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="eca98-138">JSON Representation</span></span>
<span data-ttu-id="eca98-139">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="eca98-139">Here is a JSON representation of the resource.</span></span>
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





