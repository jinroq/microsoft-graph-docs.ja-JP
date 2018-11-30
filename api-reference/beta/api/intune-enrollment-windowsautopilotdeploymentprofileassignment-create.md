---
title: WindowsAutopilotDeploymentProfileAssignment を作成します。
description: 新しい windowsAutopilotDeploymentProfileAssignment オブジェクトを作成します。
ms.openlocfilehash: 7c6e6e41711a89f5e9690f16a569b5a4afbe91c3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072521"
---
# <a name="create-windowsautopilotdeploymentprofileassignment"></a><span data-ttu-id="5c2b1-103">WindowsAutopilotDeploymentProfileAssignment を作成します。</span><span class="sxs-lookup"><span data-stu-id="5c2b1-103">Create windowsAutopilotDeploymentProfileAssignment</span></span>

> <span data-ttu-id="5c2b1-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="5c2b1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5c2b1-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5c2b1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5c2b1-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="5c2b1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5c2b1-107">新しい[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="5c2b1-107">Create a new [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5c2b1-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="5c2b1-108">Prerequisites</span></span>
<span data-ttu-id="5c2b1-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5c2b1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5c2b1-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5c2b1-111">Permission type</span></span>|<span data-ttu-id="5c2b1-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="5c2b1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5c2b1-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5c2b1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5c2b1-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c2b1-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="5c2b1-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5c2b1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5c2b1-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5c2b1-116">Not supported.</span></span>|
|<span data-ttu-id="5c2b1-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5c2b1-117">Application</span></span>|<span data-ttu-id="5c2b1-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5c2b1-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5c2b1-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5c2b1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignments
```

## <a name="request-headers"></a><span data-ttu-id="5c2b1-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5c2b1-120">Request headers</span></span>
|<span data-ttu-id="5c2b1-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5c2b1-121">Header</span></span>|<span data-ttu-id="5c2b1-122">値</span><span class="sxs-lookup"><span data-stu-id="5c2b1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5c2b1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5c2b1-123">Authorization</span></span>|<span data-ttu-id="5c2b1-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="5c2b1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5c2b1-125">Accept</span><span class="sxs-lookup"><span data-stu-id="5c2b1-125">Accept</span></span>|<span data-ttu-id="5c2b1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5c2b1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5c2b1-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="5c2b1-127">Request body</span></span>
<span data-ttu-id="5c2b1-128">要求の本文に windowsAutopilotDeploymentProfileAssignment オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="5c2b1-128">In the request body, supply a JSON representation for the windowsAutopilotDeploymentProfileAssignment object.</span></span>

<span data-ttu-id="5c2b1-129">次の表は、windowsAutopilotDeploymentProfileAssignment を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="5c2b1-129">The following table shows the properties that are required when you create the windowsAutopilotDeploymentProfileAssignment.</span></span>

|<span data-ttu-id="5c2b1-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5c2b1-130">Property</span></span>|<span data-ttu-id="5c2b1-131">型</span><span class="sxs-lookup"><span data-stu-id="5c2b1-131">Type</span></span>|<span data-ttu-id="5c2b1-132">説明</span><span class="sxs-lookup"><span data-stu-id="5c2b1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5c2b1-133">id</span><span class="sxs-lookup"><span data-stu-id="5c2b1-133">id</span></span>|<span data-ttu-id="5c2b1-134">String</span><span class="sxs-lookup"><span data-stu-id="5c2b1-134">String</span></span>|<span data-ttu-id="5c2b1-135">割り当てのキー。</span><span class="sxs-lookup"><span data-stu-id="5c2b1-135">The key of the assignment.</span></span>|
|<span data-ttu-id="5c2b1-136">target</span><span class="sxs-lookup"><span data-stu-id="5c2b1-136">target</span></span>|[<span data-ttu-id="5c2b1-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="5c2b1-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="5c2b1-138">Windows の自動操縦装置の配置のプロファイルの割り当てのターゲットです。</span><span class="sxs-lookup"><span data-stu-id="5c2b1-138">The assignment target for the Windows Autopilot deployment profile.</span></span>|



## <a name="response"></a><span data-ttu-id="5c2b1-139">応答</span><span class="sxs-lookup"><span data-stu-id="5c2b1-139">Response</span></span>
<span data-ttu-id="5c2b1-140">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="5c2b1-140">If successful, this method returns a `201 Created` response code and a [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5c2b1-141">例</span><span class="sxs-lookup"><span data-stu-id="5c2b1-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="5c2b1-142">要求</span><span class="sxs-lookup"><span data-stu-id="5c2b1-142">Request</span></span>
<span data-ttu-id="5c2b1-143">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="5c2b1-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignments
Content-type: application/json
Content-length: 183

{
  "@odata.type": "#microsoft.graph.windowsAutopilotDeploymentProfileAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="5c2b1-144">応答</span><span class="sxs-lookup"><span data-stu-id="5c2b1-144">Response</span></span>
<span data-ttu-id="5c2b1-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="5c2b1-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





