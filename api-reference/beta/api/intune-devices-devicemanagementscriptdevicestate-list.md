---
title: リスト deviceManagementScriptDeviceStates
description: DeviceManagementScriptDeviceState オブジェクトのプロパティとリレーションシップをリストします。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: fe14c5b2a866c36e50f097dd4c290823f56bf8ad
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36310368"
---
# <a name="list-devicemanagementscriptdevicestates"></a><span data-ttu-id="af625-103">リスト deviceManagementScriptDeviceStates</span><span class="sxs-lookup"><span data-stu-id="af625-103">List deviceManagementScriptDeviceStates</span></span>

> <span data-ttu-id="af625-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="af625-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="af625-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="af625-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="af625-106">[Devicemanagementscriptdevicestate](../resources/intune-devices-devicemanagementscriptdevicestate.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="af625-106">List properties and relationships of the [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="af625-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="af625-107">Prerequisites</span></span>
<span data-ttu-id="af625-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="af625-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="af625-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="af625-110">Permission type</span></span>|<span data-ttu-id="af625-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="af625-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="af625-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="af625-112">Delegated (work or school account)</span></span>|<span data-ttu-id="af625-113">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="af625-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="af625-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="af625-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="af625-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="af625-115">Not supported.</span></span>|
|<span data-ttu-id="af625-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="af625-116">Application</span></span>|<span data-ttu-id="af625-117">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="af625-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="af625-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="af625-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates/{deviceManagementScriptUserStateId}/deviceRunStates
```

## <a name="request-headers"></a><span data-ttu-id="af625-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="af625-119">Request headers</span></span>
|<span data-ttu-id="af625-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="af625-120">Header</span></span>|<span data-ttu-id="af625-121">値</span><span class="sxs-lookup"><span data-stu-id="af625-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="af625-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="af625-122">Authorization</span></span>|<span data-ttu-id="af625-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="af625-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="af625-124">承諾</span><span class="sxs-lookup"><span data-stu-id="af625-124">Accept</span></span>|<span data-ttu-id="af625-125">application/json</span><span class="sxs-lookup"><span data-stu-id="af625-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="af625-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="af625-126">Request body</span></span>
<span data-ttu-id="af625-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="af625-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="af625-128">応答</span><span class="sxs-lookup"><span data-stu-id="af625-128">Response</span></span>
<span data-ttu-id="af625-129">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[Devicemanagementscriptdevicestate](../resources/intune-devices-devicemanagementscriptdevicestate.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="af625-129">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="af625-130">例</span><span class="sxs-lookup"><span data-stu-id="af625-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="af625-131">要求</span><span class="sxs-lookup"><span data-stu-id="af625-131">Request</span></span>
<span data-ttu-id="af625-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="af625-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates
```

### <a name="response"></a><span data-ttu-id="af625-133">応答</span><span class="sxs-lookup"><span data-stu-id="af625-133">Response</span></span>
<span data-ttu-id="af625-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="af625-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 714

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementScriptDeviceState",
      "id": "39440cba-0cba-3944-ba0c-4439ba0c4439",
      "runState": "success",
      "resultMessage": "Result Message value",
      "lastStateUpdateDateTime": "2017-01-01T00:02:58.4418045-08:00",
      "errorCode": 9,
      "errorDescription": "Error Description value",
      "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
      "preRemediationDetectionScriptOutput": "Pre Remediation Detection Script Output value",
      "remediationScriptError": "Remediation Script Error value",
      "postRemediationDetectionScriptOutput": "Post Remediation Detection Script Output value"
    }
  ]
}
```






