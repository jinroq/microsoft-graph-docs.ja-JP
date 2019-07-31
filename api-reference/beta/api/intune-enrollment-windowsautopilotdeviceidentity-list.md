---
title: リスト windowsAutopilotDeviceIdentities
description: WindowsAutopilotDeviceIdentity オブジェクトのプロパティとリレーションシップをリストします。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a24edb14de36858360ee3318b713b29c85b23978
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35995476"
---
# <a name="list-windowsautopilotdeviceidentities"></a><span data-ttu-id="dcf3b-103">リスト windowsAutopilotDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="dcf3b-103">List windowsAutopilotDeviceIdentities</span></span>

> <span data-ttu-id="dcf3b-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dcf3b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dcf3b-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="dcf3b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dcf3b-106">[WindowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="dcf3b-106">List properties and relationships of the [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dcf3b-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="dcf3b-107">Prerequisites</span></span>
<span data-ttu-id="dcf3b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="dcf3b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dcf3b-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="dcf3b-110">Permission type</span></span>|<span data-ttu-id="dcf3b-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="dcf3b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dcf3b-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="dcf3b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="dcf3b-113">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="dcf3b-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="dcf3b-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="dcf3b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dcf3b-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dcf3b-115">Not supported.</span></span>|
|<span data-ttu-id="dcf3b-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="dcf3b-116">Application</span></span>|<span data-ttu-id="dcf3b-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dcf3b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dcf3b-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="dcf3b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsAutopilotDeviceIdentities
GET /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignedDevices
```

## <a name="request-headers"></a><span data-ttu-id="dcf3b-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="dcf3b-119">Request headers</span></span>
|<span data-ttu-id="dcf3b-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="dcf3b-120">Header</span></span>|<span data-ttu-id="dcf3b-121">値</span><span class="sxs-lookup"><span data-stu-id="dcf3b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dcf3b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="dcf3b-122">Authorization</span></span>|<span data-ttu-id="dcf3b-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="dcf3b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dcf3b-124">承諾</span><span class="sxs-lookup"><span data-stu-id="dcf3b-124">Accept</span></span>|<span data-ttu-id="dcf3b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="dcf3b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dcf3b-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="dcf3b-126">Request body</span></span>
<span data-ttu-id="dcf3b-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="dcf3b-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dcf3b-128">応答</span><span class="sxs-lookup"><span data-stu-id="dcf3b-128">Response</span></span>
<span data-ttu-id="dcf3b-129">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="dcf3b-129">If successful, this method returns a `200 OK` response code and a collection of [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dcf3b-130">例</span><span class="sxs-lookup"><span data-stu-id="dcf3b-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="dcf3b-131">要求</span><span class="sxs-lookup"><span data-stu-id="dcf3b-131">Request</span></span>
<span data-ttu-id="dcf3b-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="dcf3b-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities
```

### <a name="response"></a><span data-ttu-id="dcf3b-133">応答</span><span class="sxs-lookup"><span data-stu-id="dcf3b-133">Response</span></span>
<span data-ttu-id="dcf3b-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="dcf3b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1201

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsAutopilotDeviceIdentity",
      "id": "fac6f0b1-f0b1-fac6-b1f0-c6fab1f0c6fa",
      "deploymentProfileAssignmentStatus": "assignedInSync",
      "deploymentProfileAssignmentDetailedStatus": "hardwareRequirementsNotMet",
      "deploymentProfileAssignedDateTime": "2016-12-31T23:58:26.2447023-08:00",
      "orderIdentifier": "Order Identifier value",
      "groupTag": "Group Tag value",
      "purchaseOrderIdentifier": "Purchase Order Identifier value",
      "serialNumber": "Serial Number value",
      "productKey": "Product Key value",
      "manufacturer": "Manufacturer value",
      "model": "Model value",
      "enrollmentState": "enrolled",
      "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
      "addressableUserName": "Addressable User Name value",
      "userPrincipalName": "User Principal Name value",
      "resourceName": "Resource Name value",
      "skuNumber": "Sku Number value",
      "systemFamily": "System Family value",
      "azureActiveDirectoryDeviceId": "Azure Active Directory Device Id value",
      "managedDeviceId": "Managed Device Id value"
    }
  ]
}
```





