---
title: windowsAutopilotDeploymentProfileAssignment リソースの種類
description: AAD グループに Windows の自動操縦装置の展開のプロファイルの割り当て。
author: tfitzmac
ms.openlocfilehash: b9141d9a3126d25dd6de5e342ebb463304e1ae02
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27337122"
---
# <a name="windowsautopilotdeploymentprofileassignment-resource-type"></a><span data-ttu-id="28afe-103">windowsAutopilotDeploymentProfileAssignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="28afe-103">windowsAutopilotDeploymentProfileAssignment resource type</span></span>

> <span data-ttu-id="28afe-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="28afe-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="28afe-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="28afe-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="28afe-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="28afe-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="28afe-107">AAD グループに Windows の自動操縦装置の展開のプロファイルの割り当て。</span><span class="sxs-lookup"><span data-stu-id="28afe-107">An assignment of a Windows Autopilot deployment profile to an AAD group.</span></span>
## <a name="methods"></a><span data-ttu-id="28afe-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="28afe-108">Methods</span></span>
|<span data-ttu-id="28afe-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="28afe-109">Method</span></span>|<span data-ttu-id="28afe-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="28afe-110">Return Type</span></span>|<span data-ttu-id="28afe-111">説明</span><span class="sxs-lookup"><span data-stu-id="28afe-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="28afe-112">リスト windowsAutopilotDeploymentProfileAssignments</span><span class="sxs-lookup"><span data-stu-id="28afe-112">List windowsAutopilotDeploymentProfileAssignments</span></span>](../api/intune-enrollment-windowsautopilotdeploymentprofileassignment-list.md)|<span data-ttu-id="28afe-113">[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="28afe-113">[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) collection</span></span>|<span data-ttu-id="28afe-114">[WindowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="28afe-114">List properties and relationships of the [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) objects.</span></span>|
|[<span data-ttu-id="28afe-115">WindowsAutopilotDeploymentProfileAssignment を取得します。</span><span class="sxs-lookup"><span data-stu-id="28afe-115">Get windowsAutopilotDeploymentProfileAssignment</span></span>](../api/intune-enrollment-windowsautopilotdeploymentprofileassignment-get.md)|[<span data-ttu-id="28afe-116">windowsAutopilotDeploymentProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="28afe-116">windowsAutopilotDeploymentProfileAssignment</span></span>](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)|<span data-ttu-id="28afe-117">[WindowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="28afe-117">Read properties and relationships of the [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object.</span></span>|
|[<span data-ttu-id="28afe-118">WindowsAutopilotDeploymentProfileAssignment を作成します。</span><span class="sxs-lookup"><span data-stu-id="28afe-118">Create windowsAutopilotDeploymentProfileAssignment</span></span>](../api/intune-enrollment-windowsautopilotdeploymentprofileassignment-create.md)|[<span data-ttu-id="28afe-119">windowsAutopilotDeploymentProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="28afe-119">windowsAutopilotDeploymentProfileAssignment</span></span>](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)|<span data-ttu-id="28afe-120">新しい[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="28afe-120">Create a new [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object.</span></span>|
|[<span data-ttu-id="28afe-121">WindowsAutopilotDeploymentProfileAssignment を削除します。</span><span class="sxs-lookup"><span data-stu-id="28afe-121">Delete windowsAutopilotDeploymentProfileAssignment</span></span>](../api/intune-enrollment-windowsautopilotdeploymentprofileassignment-delete.md)|<span data-ttu-id="28afe-122">なし</span><span class="sxs-lookup"><span data-stu-id="28afe-122">None</span></span>|<span data-ttu-id="28afe-123">の[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="28afe-123">Deletes a [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md).</span></span>|
|[<span data-ttu-id="28afe-124">WindowsAutopilotDeploymentProfileAssignment を更新します。</span><span class="sxs-lookup"><span data-stu-id="28afe-124">Update windowsAutopilotDeploymentProfileAssignment</span></span>](../api/intune-enrollment-windowsautopilotdeploymentprofileassignment-update.md)|[<span data-ttu-id="28afe-125">windowsAutopilotDeploymentProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="28afe-125">windowsAutopilotDeploymentProfileAssignment</span></span>](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)|<span data-ttu-id="28afe-126">[WindowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="28afe-126">Update the properties of a [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="28afe-127">Properties</span><span class="sxs-lookup"><span data-stu-id="28afe-127">Properties</span></span>
|<span data-ttu-id="28afe-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="28afe-128">Property</span></span>|<span data-ttu-id="28afe-129">種類</span><span class="sxs-lookup"><span data-stu-id="28afe-129">Type</span></span>|<span data-ttu-id="28afe-130">説明</span><span class="sxs-lookup"><span data-stu-id="28afe-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="28afe-131">ID</span><span class="sxs-lookup"><span data-stu-id="28afe-131">id</span></span>|<span data-ttu-id="28afe-132">String</span><span class="sxs-lookup"><span data-stu-id="28afe-132">String</span></span>|<span data-ttu-id="28afe-133">割り当てのキー。</span><span class="sxs-lookup"><span data-stu-id="28afe-133">The key of the assignment.</span></span>|
|<span data-ttu-id="28afe-134">target</span><span class="sxs-lookup"><span data-stu-id="28afe-134">target</span></span>|[<span data-ttu-id="28afe-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="28afe-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="28afe-136">Windows の自動操縦装置の配置のプロファイルの割り当てのターゲットです。</span><span class="sxs-lookup"><span data-stu-id="28afe-136">The assignment target for the Windows Autopilot deployment profile.</span></span>|

## <a name="relationships"></a><span data-ttu-id="28afe-137">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="28afe-137">Relationships</span></span>
<span data-ttu-id="28afe-138">なし</span><span class="sxs-lookup"><span data-stu-id="28afe-138">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="28afe-139">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="28afe-139">JSON Representation</span></span>
<span data-ttu-id="28afe-140">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="28afe-140">Here is a JSON representation of the resource.</span></span>
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





