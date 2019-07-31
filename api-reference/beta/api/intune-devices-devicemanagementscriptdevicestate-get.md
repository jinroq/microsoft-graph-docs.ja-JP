---
title: DeviceManagementScriptDeviceState の取得
description: DeviceManagementScriptDeviceState オブジェクトのプロパティとリレーションシップを読み取ります。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2fe601798119e767824331d4c2975cf58c55cca4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35986009"
---
# <a name="get-devicemanagementscriptdevicestate"></a><span data-ttu-id="ae6fd-103">DeviceManagementScriptDeviceState の取得</span><span class="sxs-lookup"><span data-stu-id="ae6fd-103">Get deviceManagementScriptDeviceState</span></span>

> <span data-ttu-id="ae6fd-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ae6fd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ae6fd-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ae6fd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ae6fd-106">[Devicemanagementscriptdevicestate](../resources/intune-devices-devicemanagementscriptdevicestate.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="ae6fd-106">Read properties and relationships of the [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ae6fd-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="ae6fd-107">Prerequisites</span></span>
<span data-ttu-id="ae6fd-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ae6fd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ae6fd-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ae6fd-110">Permission type</span></span>|<span data-ttu-id="ae6fd-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="ae6fd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ae6fd-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ae6fd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ae6fd-113">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="ae6fd-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="ae6fd-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ae6fd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ae6fd-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ae6fd-115">Not supported.</span></span>|
|<span data-ttu-id="ae6fd-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ae6fd-116">Application</span></span>|<span data-ttu-id="ae6fd-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ae6fd-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ae6fd-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ae6fd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates/{deviceManagementScriptUserStateId}/deviceRunStates/{deviceManagementScriptDeviceStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ae6fd-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="ae6fd-119">Optional query parameters</span></span>
<span data-ttu-id="ae6fd-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="ae6fd-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ae6fd-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ae6fd-121">Request headers</span></span>
|<span data-ttu-id="ae6fd-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ae6fd-122">Header</span></span>|<span data-ttu-id="ae6fd-123">値</span><span class="sxs-lookup"><span data-stu-id="ae6fd-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ae6fd-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="ae6fd-124">Authorization</span></span>|<span data-ttu-id="ae6fd-125">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="ae6fd-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ae6fd-126">承諾</span><span class="sxs-lookup"><span data-stu-id="ae6fd-126">Accept</span></span>|<span data-ttu-id="ae6fd-127">application/json</span><span class="sxs-lookup"><span data-stu-id="ae6fd-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ae6fd-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="ae6fd-128">Request body</span></span>
<span data-ttu-id="ae6fd-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="ae6fd-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ae6fd-130">応答</span><span class="sxs-lookup"><span data-stu-id="ae6fd-130">Response</span></span>
<span data-ttu-id="ae6fd-131">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[Devicemanagementscriptdevicestate](../resources/intune-devices-devicemanagementscriptdevicestate.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ae6fd-131">If successful, this method returns a `200 OK` response code and [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ae6fd-132">例</span><span class="sxs-lookup"><span data-stu-id="ae6fd-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="ae6fd-133">要求</span><span class="sxs-lookup"><span data-stu-id="ae6fd-133">Request</span></span>
<span data-ttu-id="ae6fd-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ae6fd-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}
```

### <a name="response"></a><span data-ttu-id="ae6fd-135">応答</span><span class="sxs-lookup"><span data-stu-id="ae6fd-135">Response</span></span>
<span data-ttu-id="ae6fd-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ae6fd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





