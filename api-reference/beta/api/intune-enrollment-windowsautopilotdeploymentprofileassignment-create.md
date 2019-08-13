---
title: WindowsAutopilotDeploymentProfileAssignment を作成する
description: 新しい windowsAutopilotDeploymentProfileAssignment オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d8e9e48d577f68647973abe77c7a2628b8fc29d5
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36356152"
---
# <a name="create-windowsautopilotdeploymentprofileassignment"></a><span data-ttu-id="82d77-103">WindowsAutopilotDeploymentProfileAssignment を作成する</span><span class="sxs-lookup"><span data-stu-id="82d77-103">Create windowsAutopilotDeploymentProfileAssignment</span></span>

> <span data-ttu-id="82d77-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="82d77-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="82d77-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="82d77-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="82d77-106">新しい[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="82d77-106">Create a new [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="82d77-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="82d77-107">Prerequisites</span></span>
<span data-ttu-id="82d77-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="82d77-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="82d77-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="82d77-110">Permission type</span></span>|<span data-ttu-id="82d77-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="82d77-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="82d77-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="82d77-112">Delegated (work or school account)</span></span>|<span data-ttu-id="82d77-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82d77-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="82d77-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="82d77-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="82d77-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="82d77-115">Not supported.</span></span>|
|<span data-ttu-id="82d77-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="82d77-116">Application</span></span>|<span data-ttu-id="82d77-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82d77-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="82d77-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="82d77-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignments
```

## <a name="request-headers"></a><span data-ttu-id="82d77-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="82d77-119">Request headers</span></span>
|<span data-ttu-id="82d77-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="82d77-120">Header</span></span>|<span data-ttu-id="82d77-121">値</span><span class="sxs-lookup"><span data-stu-id="82d77-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="82d77-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="82d77-122">Authorization</span></span>|<span data-ttu-id="82d77-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="82d77-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="82d77-124">承諾</span><span class="sxs-lookup"><span data-stu-id="82d77-124">Accept</span></span>|<span data-ttu-id="82d77-125">application/json</span><span class="sxs-lookup"><span data-stu-id="82d77-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="82d77-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="82d77-126">Request body</span></span>
<span data-ttu-id="82d77-127">要求本文で、windowsAutopilotDeploymentProfileAssignment オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="82d77-127">In the request body, supply a JSON representation for the windowsAutopilotDeploymentProfileAssignment object.</span></span>

<span data-ttu-id="82d77-128">次の表に、windowsAutopilotDeploymentProfileAssignment の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="82d77-128">The following table shows the properties that are required when you create the windowsAutopilotDeploymentProfileAssignment.</span></span>

|<span data-ttu-id="82d77-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="82d77-129">Property</span></span>|<span data-ttu-id="82d77-130">型</span><span class="sxs-lookup"><span data-stu-id="82d77-130">Type</span></span>|<span data-ttu-id="82d77-131">説明</span><span class="sxs-lookup"><span data-stu-id="82d77-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="82d77-132">id</span><span class="sxs-lookup"><span data-stu-id="82d77-132">id</span></span>|<span data-ttu-id="82d77-133">String</span><span class="sxs-lookup"><span data-stu-id="82d77-133">String</span></span>|<span data-ttu-id="82d77-134">割り当てのキー。</span><span class="sxs-lookup"><span data-stu-id="82d77-134">The key of the assignment.</span></span>|
|<span data-ttu-id="82d77-135">target</span><span class="sxs-lookup"><span data-stu-id="82d77-135">target</span></span>|[<span data-ttu-id="82d77-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="82d77-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="82d77-137">Windows 自動操縦展開プロファイルの割り当て先。</span><span class="sxs-lookup"><span data-stu-id="82d77-137">The assignment target for the Windows Autopilot deployment profile.</span></span>|



## <a name="response"></a><span data-ttu-id="82d77-138">応答</span><span class="sxs-lookup"><span data-stu-id="82d77-138">Response</span></span>
<span data-ttu-id="82d77-139">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="82d77-139">If successful, this method returns a `201 Created` response code and a [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="82d77-140">例</span><span class="sxs-lookup"><span data-stu-id="82d77-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="82d77-141">要求</span><span class="sxs-lookup"><span data-stu-id="82d77-141">Request</span></span>
<span data-ttu-id="82d77-142">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="82d77-142">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="82d77-143">応答</span><span class="sxs-lookup"><span data-stu-id="82d77-143">Response</span></span>
<span data-ttu-id="82d77-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="82d77-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






