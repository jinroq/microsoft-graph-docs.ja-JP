---
title: deviceConfigurationDeviceStatuses のリスト
description: deviceConfigurationDeviceStatus オブジェクトのプロパティとリレーションシップをリストします。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: aed784995eaa99f59e614536a70726a600bb912c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36017504"
---
# <a name="list-deviceconfigurationdevicestatuses"></a><span data-ttu-id="f4f46-103">deviceConfigurationDeviceStatuses のリスト</span><span class="sxs-lookup"><span data-stu-id="f4f46-103">List deviceConfigurationDeviceStatuses</span></span>

> <span data-ttu-id="f4f46-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f4f46-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f4f46-105">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="f4f46-105">List properties and relationships of the [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f4f46-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="f4f46-106">Prerequisites</span></span>
<span data-ttu-id="f4f46-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f4f46-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f4f46-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f4f46-109">Permission type</span></span>|<span data-ttu-id="f4f46-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="f4f46-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f4f46-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f4f46-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f4f46-112">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f4f46-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="f4f46-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f4f46-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f4f46-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f4f46-114">Not supported.</span></span>|
|<span data-ttu-id="f4f46-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f4f46-115">Application</span></span>|<span data-ttu-id="f4f46-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f4f46-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f4f46-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f4f46-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="f4f46-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f4f46-118">Request headers</span></span>
|<span data-ttu-id="f4f46-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f4f46-119">Header</span></span>|<span data-ttu-id="f4f46-120">値</span><span class="sxs-lookup"><span data-stu-id="f4f46-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f4f46-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f4f46-121">Authorization</span></span>|<span data-ttu-id="f4f46-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="f4f46-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f4f46-123">承諾</span><span class="sxs-lookup"><span data-stu-id="f4f46-123">Accept</span></span>|<span data-ttu-id="f4f46-124">application/json</span><span class="sxs-lookup"><span data-stu-id="f4f46-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f4f46-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="f4f46-125">Request body</span></span>
<span data-ttu-id="f4f46-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="f4f46-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f4f46-127">応答</span><span class="sxs-lookup"><span data-stu-id="f4f46-127">Response</span></span>
<span data-ttu-id="f4f46-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="f4f46-128">If successful, this method returns a `200 OK` response code and a collection of [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f4f46-129">例</span><span class="sxs-lookup"><span data-stu-id="f4f46-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="f4f46-130">要求</span><span class="sxs-lookup"><span data-stu-id="f4f46-130">Request</span></span>
<span data-ttu-id="f4f46-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f4f46-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses
```

### <a name="response"></a><span data-ttu-id="f4f46-132">応答</span><span class="sxs-lookup"><span data-stu-id="f4f46-132">Response</span></span>
<span data-ttu-id="f4f46-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f4f46-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 547

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceConfigurationDeviceStatus",
      "id": "674e98e5-98e5-674e-e598-4e67e5984e67",
      "deviceDisplayName": "Device Display Name value",
      "userName": "User Name value",
      "deviceModel": "Device Model value",
      "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
      "status": "notApplicable",
      "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
      "userPrincipalName": "User Principal Name value"
    }
  ]
}
```



