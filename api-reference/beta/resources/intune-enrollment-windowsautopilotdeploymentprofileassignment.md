---
title: windowsAutopilotDeploymentProfileAssignment リソースの種類
description: AAD グループへの Windows 自動操縦展開プロファイルの割り当て。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5147a3a7414c44d8b17345b97b54fdfc6a7f81c8
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30151458"
---
# <a name="windowsautopilotdeploymentprofileassignment-resource-type"></a><span data-ttu-id="0cc8c-103">windowsAutopilotDeploymentProfileAssignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0cc8c-103">windowsAutopilotDeploymentProfileAssignment resource type</span></span>

> <span data-ttu-id="0cc8c-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0cc8c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0cc8c-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0cc8c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0cc8c-106">AAD グループへの Windows 自動操縦展開プロファイルの割り当て。</span><span class="sxs-lookup"><span data-stu-id="0cc8c-106">An assignment of a Windows Autopilot deployment profile to an AAD group.</span></span>

## <a name="methods"></a><span data-ttu-id="0cc8c-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="0cc8c-107">Methods</span></span>
|<span data-ttu-id="0cc8c-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="0cc8c-108">Method</span></span>|<span data-ttu-id="0cc8c-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="0cc8c-109">Return Type</span></span>|<span data-ttu-id="0cc8c-110">説明</span><span class="sxs-lookup"><span data-stu-id="0cc8c-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0cc8c-111">リスト windowsAutopilotDeploymentProfileAssignments</span><span class="sxs-lookup"><span data-stu-id="0cc8c-111">List windowsAutopilotDeploymentProfileAssignments</span></span>](../api/intune-enrollment-windowsautopilotdeploymentprofileassignment-list.md)|<span data-ttu-id="0cc8c-112">[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="0cc8c-112">[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) collection</span></span>|<span data-ttu-id="0cc8c-113">[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="0cc8c-113">List properties and relationships of the [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) objects.</span></span>|
|[<span data-ttu-id="0cc8c-114">windowsAutopilotDeploymentProfileAssignment を取得する</span><span class="sxs-lookup"><span data-stu-id="0cc8c-114">Get windowsAutopilotDeploymentProfileAssignment</span></span>](../api/intune-enrollment-windowsautopilotdeploymentprofileassignment-get.md)|[<span data-ttu-id="0cc8c-115">windowsAutopilotDeploymentProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="0cc8c-115">windowsAutopilotDeploymentProfileAssignment</span></span>](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)|<span data-ttu-id="0cc8c-116">[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="0cc8c-116">Read properties and relationships of the [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object.</span></span>|
|[<span data-ttu-id="0cc8c-117">windowsAutopilotDeploymentProfileAssignment を作成する</span><span class="sxs-lookup"><span data-stu-id="0cc8c-117">Create windowsAutopilotDeploymentProfileAssignment</span></span>](../api/intune-enrollment-windowsautopilotdeploymentprofileassignment-create.md)|[<span data-ttu-id="0cc8c-118">windowsAutopilotDeploymentProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="0cc8c-118">windowsAutopilotDeploymentProfileAssignment</span></span>](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)|<span data-ttu-id="0cc8c-119">新しい[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="0cc8c-119">Create a new [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object.</span></span>|
|[<span data-ttu-id="0cc8c-120">windowsAutopilotDeploymentProfileAssignment の削除</span><span class="sxs-lookup"><span data-stu-id="0cc8c-120">Delete windowsAutopilotDeploymentProfileAssignment</span></span>](../api/intune-enrollment-windowsautopilotdeploymentprofileassignment-delete.md)|<span data-ttu-id="0cc8c-121">なし</span><span class="sxs-lookup"><span data-stu-id="0cc8c-121">None</span></span>|<span data-ttu-id="0cc8c-122">[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="0cc8c-122">Deletes a [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md).</span></span>|
|[<span data-ttu-id="0cc8c-123">windowsAutopilotDeploymentProfileAssignment の更新</span><span class="sxs-lookup"><span data-stu-id="0cc8c-123">Update windowsAutopilotDeploymentProfileAssignment</span></span>](../api/intune-enrollment-windowsautopilotdeploymentprofileassignment-update.md)|[<span data-ttu-id="0cc8c-124">windowsAutopilotDeploymentProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="0cc8c-124">windowsAutopilotDeploymentProfileAssignment</span></span>](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)|<span data-ttu-id="0cc8c-125">[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="0cc8c-125">Update the properties of a [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="0cc8c-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0cc8c-126">Properties</span></span>
|<span data-ttu-id="0cc8c-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0cc8c-127">Property</span></span>|<span data-ttu-id="0cc8c-128">型</span><span class="sxs-lookup"><span data-stu-id="0cc8c-128">Type</span></span>|<span data-ttu-id="0cc8c-129">説明</span><span class="sxs-lookup"><span data-stu-id="0cc8c-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0cc8c-130">id</span><span class="sxs-lookup"><span data-stu-id="0cc8c-130">id</span></span>|<span data-ttu-id="0cc8c-131">String</span><span class="sxs-lookup"><span data-stu-id="0cc8c-131">String</span></span>|<span data-ttu-id="0cc8c-132">割り当てのキー。</span><span class="sxs-lookup"><span data-stu-id="0cc8c-132">The key of the assignment.</span></span>|
|<span data-ttu-id="0cc8c-133">target</span><span class="sxs-lookup"><span data-stu-id="0cc8c-133">target</span></span>|[<span data-ttu-id="0cc8c-134">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="0cc8c-134">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="0cc8c-135">Windows 自動操縦展開プロファイルの割り当て先。</span><span class="sxs-lookup"><span data-stu-id="0cc8c-135">The assignment target for the Windows Autopilot deployment profile.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0cc8c-136">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0cc8c-136">Relationships</span></span>
<span data-ttu-id="0cc8c-137">なし</span><span class="sxs-lookup"><span data-stu-id="0cc8c-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0cc8c-138">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0cc8c-138">JSON Representation</span></span>
<span data-ttu-id="0cc8c-139">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0cc8c-139">Here is a JSON representation of the resource.</span></span>
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




