---
title: リスト deviceManagementIntentDeviceStates
description: devicemanagementintentdevicestate オブジェクトのプロパティとリレーションシップをリストします。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3e9f1f38dc75b0d7e5488382a26ecd3100fbc6da
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/08/2019
ms.locfileid: "31523764"
---
# <a name="list-devicemanagementintentdevicestates"></a><span data-ttu-id="540ed-103">リスト deviceManagementIntentDeviceStates</span><span class="sxs-lookup"><span data-stu-id="540ed-103">List deviceManagementIntentDeviceStates</span></span>

> <span data-ttu-id="540ed-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="540ed-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="540ed-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="540ed-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="540ed-106">[devicemanagementintentdevicestate](../resources/intune-deviceintent-devicemanagementintentdevicestate.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="540ed-106">List properties and relationships of the [deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="540ed-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="540ed-107">Prerequisites</span></span>
<span data-ttu-id="540ed-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="540ed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="540ed-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="540ed-110">Permission type</span></span>|<span data-ttu-id="540ed-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="540ed-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="540ed-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="540ed-112">Delegated (work or school account)</span></span>|<span data-ttu-id="540ed-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="540ed-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="540ed-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="540ed-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="540ed-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="540ed-115">Not supported.</span></span>|
|<span data-ttu-id="540ed-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="540ed-116">Application</span></span>|<span data-ttu-id="540ed-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="540ed-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="540ed-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="540ed-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/intents/{deviceManagementIntentId}/deviceStates
```

## <a name="request-headers"></a><span data-ttu-id="540ed-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="540ed-119">Request headers</span></span>
|<span data-ttu-id="540ed-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="540ed-120">Header</span></span>|<span data-ttu-id="540ed-121">値</span><span class="sxs-lookup"><span data-stu-id="540ed-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="540ed-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="540ed-122">Authorization</span></span>|<span data-ttu-id="540ed-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="540ed-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="540ed-124">承諾</span><span class="sxs-lookup"><span data-stu-id="540ed-124">Accept</span></span>|<span data-ttu-id="540ed-125">application/json</span><span class="sxs-lookup"><span data-stu-id="540ed-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="540ed-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="540ed-126">Request body</span></span>
<span data-ttu-id="540ed-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="540ed-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="540ed-128">応答</span><span class="sxs-lookup"><span data-stu-id="540ed-128">Response</span></span>
<span data-ttu-id="540ed-129">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[devicemanagementintentdevicestate](../resources/intune-deviceintent-devicemanagementintentdevicestate.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="540ed-129">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="540ed-130">例</span><span class="sxs-lookup"><span data-stu-id="540ed-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="540ed-131">要求</span><span class="sxs-lookup"><span data-stu-id="540ed-131">Request</span></span>
<span data-ttu-id="540ed-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="540ed-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/deviceStates
```

### <a name="response"></a><span data-ttu-id="540ed-133">応答</span><span class="sxs-lookup"><span data-stu-id="540ed-133">Response</span></span>
<span data-ttu-id="540ed-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="540ed-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 456

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementIntentDeviceState",
      "id": "8db75881-5881-8db7-8158-b78d8158b78d",
      "userPrincipalName": "User Principal Name value",
      "userName": "User Name value",
      "deviceDisplayName": "Device Display Name value",
      "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
      "state": "notApplicable",
      "deviceId": "Device Id value"
    }
  ]
}
```







