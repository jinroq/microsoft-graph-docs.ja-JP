---
title: リスト restrictedAppsViolations
description: restrictedAppsViolation オブジェクトのプロパティとリレーションシップをリストします。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f23831ad389d4e803f3821c1a7ce8f8a5d02ac5a
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31777964"
---
# <a name="list-restrictedappsviolations"></a><span data-ttu-id="ad6e8-103">リスト restrictedAppsViolations</span><span class="sxs-lookup"><span data-stu-id="ad6e8-103">List restrictedAppsViolations</span></span>

> <span data-ttu-id="ad6e8-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ad6e8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ad6e8-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ad6e8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ad6e8-106">[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="ad6e8-106">List properties and relationships of the [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ad6e8-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="ad6e8-107">Prerequisites</span></span>
<span data-ttu-id="ad6e8-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ad6e8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ad6e8-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ad6e8-110">Permission type</span></span>|<span data-ttu-id="ad6e8-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="ad6e8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ad6e8-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ad6e8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ad6e8-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ad6e8-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="ad6e8-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ad6e8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ad6e8-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ad6e8-115">Not supported.</span></span>|
|<span data-ttu-id="ad6e8-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ad6e8-116">Application</span></span>|<span data-ttu-id="ad6e8-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ad6e8-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ad6e8-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ad6e8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurationRestrictedAppsViolations
```

## <a name="request-headers"></a><span data-ttu-id="ad6e8-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ad6e8-119">Request headers</span></span>
|<span data-ttu-id="ad6e8-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ad6e8-120">Header</span></span>|<span data-ttu-id="ad6e8-121">値</span><span class="sxs-lookup"><span data-stu-id="ad6e8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ad6e8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ad6e8-122">Authorization</span></span>|<span data-ttu-id="ad6e8-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="ad6e8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ad6e8-124">承諾</span><span class="sxs-lookup"><span data-stu-id="ad6e8-124">Accept</span></span>|<span data-ttu-id="ad6e8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ad6e8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ad6e8-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="ad6e8-126">Request body</span></span>
<span data-ttu-id="ad6e8-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="ad6e8-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ad6e8-128">応答</span><span class="sxs-lookup"><span data-stu-id="ad6e8-128">Response</span></span>
<span data-ttu-id="ad6e8-129">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="ad6e8-129">If successful, this method returns a `200 OK` response code and a collection of [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ad6e8-130">例</span><span class="sxs-lookup"><span data-stu-id="ad6e8-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="ad6e8-131">要求</span><span class="sxs-lookup"><span data-stu-id="ad6e8-131">Request</span></span>
<span data-ttu-id="ad6e8-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ad6e8-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationRestrictedAppsViolations
```

### <a name="response"></a><span data-ttu-id="ad6e8-133">応答</span><span class="sxs-lookup"><span data-stu-id="ad6e8-133">Response</span></span>
<span data-ttu-id="ad6e8-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ad6e8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 710

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.restrictedAppsViolation",
      "id": "53f99903-9903-53f9-0399-f9530399f953",
      "userId": "User Id value",
      "userName": "User Name value",
      "managedDeviceId": "Managed Device Id value",
      "deviceName": "Device Name value",
      "deviceConfigurationId": "Device Configuration Id value",
      "deviceConfigurationName": "Device Configuration Name value",
      "platformType": "androidForWork",
      "restrictedAppsState": "notApprovedApps",
      "restrictedApps": [
        {
          "@odata.type": "microsoft.graph.managedDeviceReportedApp",
          "appId": "App Id value"
        }
      ]
    }
  ]
}
```





