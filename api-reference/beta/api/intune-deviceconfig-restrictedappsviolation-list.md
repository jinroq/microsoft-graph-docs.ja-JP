---
title: リスト restrictedAppsViolations
description: RestrictedAppsViolation オブジェクトのプロパティと関係を一覧表示します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 284eeac8ca2220058ac1233540d3d845b55d1bd0
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410183"
---
# <a name="list-restrictedappsviolations"></a><span data-ttu-id="85778-103">リスト restrictedAppsViolations</span><span class="sxs-lookup"><span data-stu-id="85778-103">List restrictedAppsViolations</span></span>

> <span data-ttu-id="85778-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="85778-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="85778-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="85778-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="85778-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="85778-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="85778-107">[RestrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="85778-107">List properties and relationships of the [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="85778-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="85778-108">Prerequisites</span></span>
<span data-ttu-id="85778-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="85778-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="85778-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="85778-111">Permission type</span></span>|<span data-ttu-id="85778-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="85778-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="85778-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="85778-113">Delegated (work or school account)</span></span>|<span data-ttu-id="85778-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="85778-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="85778-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="85778-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="85778-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="85778-116">Not supported.</span></span>|
|<span data-ttu-id="85778-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="85778-117">Application</span></span>|<span data-ttu-id="85778-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="85778-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="85778-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="85778-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurationRestrictedAppsViolations
```

## <a name="request-headers"></a><span data-ttu-id="85778-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="85778-120">Request headers</span></span>
|<span data-ttu-id="85778-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="85778-121">Header</span></span>|<span data-ttu-id="85778-122">値</span><span class="sxs-lookup"><span data-stu-id="85778-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="85778-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="85778-123">Authorization</span></span>|<span data-ttu-id="85778-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="85778-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="85778-125">Accept</span><span class="sxs-lookup"><span data-stu-id="85778-125">Accept</span></span>|<span data-ttu-id="85778-126">application/json</span><span class="sxs-lookup"><span data-stu-id="85778-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="85778-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="85778-127">Request body</span></span>
<span data-ttu-id="85778-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="85778-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="85778-129">応答</span><span class="sxs-lookup"><span data-stu-id="85778-129">Response</span></span>
<span data-ttu-id="85778-130">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="85778-130">If successful, this method returns a `200 OK` response code and a collection of [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="85778-131">例</span><span class="sxs-lookup"><span data-stu-id="85778-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="85778-132">要求</span><span class="sxs-lookup"><span data-stu-id="85778-132">Request</span></span>
<span data-ttu-id="85778-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="85778-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationRestrictedAppsViolations
```

### <a name="response"></a><span data-ttu-id="85778-134">応答</span><span class="sxs-lookup"><span data-stu-id="85778-134">Response</span></span>
<span data-ttu-id="85778-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="85778-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




