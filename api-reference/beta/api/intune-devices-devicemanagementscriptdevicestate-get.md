---
title: DeviceManagementScriptDeviceState を取得します。
description: DeviceManagementScriptDeviceState オブジェクトのプロパティと関係を参照してください。
ms.openlocfilehash: 2f29f1bfa657afe96e40d8e43b8a62a8f2fbc0d2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070335"
---
# <a name="get-devicemanagementscriptdevicestate"></a><span data-ttu-id="87966-103">DeviceManagementScriptDeviceState を取得します。</span><span class="sxs-lookup"><span data-stu-id="87966-103">Get deviceManagementScriptDeviceState</span></span>

> <span data-ttu-id="87966-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="87966-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="87966-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="87966-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="87966-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="87966-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="87966-107">[DeviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="87966-107">Read properties and relationships of the [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="87966-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="87966-108">Prerequisites</span></span>
<span data-ttu-id="87966-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="87966-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="87966-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="87966-111">Permission type</span></span>|<span data-ttu-id="87966-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="87966-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="87966-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="87966-113">Delegated (work or school account)</span></span>|<span data-ttu-id="87966-114">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="87966-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="87966-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="87966-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="87966-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="87966-116">Not supported.</span></span>|
|<span data-ttu-id="87966-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="87966-117">Application</span></span>|<span data-ttu-id="87966-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="87966-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="87966-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="87966-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates/{deviceManagementScriptUserStateId}/deviceRunStates/{deviceManagementScriptDeviceStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="87966-120">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="87966-120">Optional query parameters</span></span>
<span data-ttu-id="87966-121">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="87966-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="87966-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="87966-122">Request headers</span></span>
|<span data-ttu-id="87966-123">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="87966-123">Header</span></span>|<span data-ttu-id="87966-124">値</span><span class="sxs-lookup"><span data-stu-id="87966-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="87966-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="87966-125">Authorization</span></span>|<span data-ttu-id="87966-126">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="87966-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="87966-127">Accept</span><span class="sxs-lookup"><span data-stu-id="87966-127">Accept</span></span>|<span data-ttu-id="87966-128">application/json</span><span class="sxs-lookup"><span data-stu-id="87966-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="87966-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="87966-129">Request body</span></span>
<span data-ttu-id="87966-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="87966-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="87966-131">応答</span><span class="sxs-lookup"><span data-stu-id="87966-131">Response</span></span>
<span data-ttu-id="87966-132">かどうかは成功すると、このメソッドが返されます、 `200 OK` 、応答の本体で応答コードと[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="87966-132">If successful, this method returns a `200 OK` response code and [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="87966-133">例</span><span class="sxs-lookup"><span data-stu-id="87966-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="87966-134">要求</span><span class="sxs-lookup"><span data-stu-id="87966-134">Request</span></span>
<span data-ttu-id="87966-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="87966-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}
```

### <a name="response"></a><span data-ttu-id="87966-136">応答</span><span class="sxs-lookup"><span data-stu-id="87966-136">Response</span></span>
<span data-ttu-id="87966-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="87966-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 363

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementScriptDeviceState",
    "id": "39440cba-0cba-3944-ba0c-4439ba0c4439",
    "runState": "success",
    "resultMessage": "Result Message value",
    "lastStateUpdateDateTime": "2017-01-01T00:02:58.4418045-08:00",
    "errorCode": 9,
    "errorDescription": "Error Description value"
  }
}
```





