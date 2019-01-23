---
title: WindowsAutopilotDeploymentProfileAssignment を更新します。
description: WindowsAutopilotDeploymentProfileAssignment オブジェクトのプロパティを更新します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8267019105d42260ec346595680ea8d4805c35dc
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29408090"
---
# <a name="update-windowsautopilotdeploymentprofileassignment"></a><span data-ttu-id="51386-103">WindowsAutopilotDeploymentProfileAssignment を更新します。</span><span class="sxs-lookup"><span data-stu-id="51386-103">Update windowsAutopilotDeploymentProfileAssignment</span></span>

> <span data-ttu-id="51386-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="51386-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="51386-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="51386-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="51386-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="51386-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="51386-107">[WindowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="51386-107">Update the properties of a [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="51386-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="51386-108">Prerequisites</span></span>
<span data-ttu-id="51386-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="51386-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="51386-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="51386-111">Permission type</span></span>|<span data-ttu-id="51386-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="51386-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="51386-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="51386-113">Delegated (work or school account)</span></span>|<span data-ttu-id="51386-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51386-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="51386-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="51386-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="51386-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="51386-116">Not supported.</span></span>|
|<span data-ttu-id="51386-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="51386-117">Application</span></span>|<span data-ttu-id="51386-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="51386-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="51386-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="51386-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignments/{windowsAutopilotDeploymentProfileAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="51386-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="51386-120">Request headers</span></span>
|<span data-ttu-id="51386-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="51386-121">Header</span></span>|<span data-ttu-id="51386-122">値</span><span class="sxs-lookup"><span data-stu-id="51386-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="51386-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="51386-123">Authorization</span></span>|<span data-ttu-id="51386-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="51386-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="51386-125">Accept</span><span class="sxs-lookup"><span data-stu-id="51386-125">Accept</span></span>|<span data-ttu-id="51386-126">application/json</span><span class="sxs-lookup"><span data-stu-id="51386-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="51386-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="51386-127">Request body</span></span>
<span data-ttu-id="51386-128">要求の本文に[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="51386-128">In the request body, supply a JSON representation for the [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object.</span></span>

<span data-ttu-id="51386-129">[WindowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="51386-129">The following table shows the properties that are required when you create the [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md).</span></span>

|<span data-ttu-id="51386-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="51386-130">Property</span></span>|<span data-ttu-id="51386-131">型</span><span class="sxs-lookup"><span data-stu-id="51386-131">Type</span></span>|<span data-ttu-id="51386-132">説明</span><span class="sxs-lookup"><span data-stu-id="51386-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="51386-133">id</span><span class="sxs-lookup"><span data-stu-id="51386-133">id</span></span>|<span data-ttu-id="51386-134">String</span><span class="sxs-lookup"><span data-stu-id="51386-134">String</span></span>|<span data-ttu-id="51386-135">割り当てのキー。</span><span class="sxs-lookup"><span data-stu-id="51386-135">The key of the assignment.</span></span>|
|<span data-ttu-id="51386-136">target</span><span class="sxs-lookup"><span data-stu-id="51386-136">target</span></span>|[<span data-ttu-id="51386-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="51386-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="51386-138">Windows の自動操縦装置の配置のプロファイルの割り当てのターゲットです。</span><span class="sxs-lookup"><span data-stu-id="51386-138">The assignment target for the Windows Autopilot deployment profile.</span></span>|



## <a name="response"></a><span data-ttu-id="51386-139">応答</span><span class="sxs-lookup"><span data-stu-id="51386-139">Response</span></span>
<span data-ttu-id="51386-140">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="51386-140">If successful, this method returns a `200 OK` response code and an updated [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="51386-141">例</span><span class="sxs-lookup"><span data-stu-id="51386-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="51386-142">要求</span><span class="sxs-lookup"><span data-stu-id="51386-142">Request</span></span>
<span data-ttu-id="51386-143">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="51386-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignments/{windowsAutopilotDeploymentProfileAssignmentId}
Content-type: application/json
Content-length: 183

{
  "@odata.type": "#microsoft.graph.windowsAutopilotDeploymentProfileAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="51386-144">応答</span><span class="sxs-lookup"><span data-stu-id="51386-144">Response</span></span>
<span data-ttu-id="51386-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="51386-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 232

{
  "@odata.type": "#microsoft.graph.windowsAutopilotDeploymentProfileAssignment",
  "id": "de7e1e1e-1e1e-de7e-1e1e-7ede1e1e7ede",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```




