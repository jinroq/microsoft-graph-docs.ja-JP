---
title: restrictedAppsViolation を取得する
description: restrictedAppsViolation オブジェクトのプロパティとリレーションシップを読み取ります。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4f9e5639293153e308965f22676d3c346b5a65b0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32518311"
---
# <a name="get-restrictedappsviolation"></a><span data-ttu-id="a3a2a-103">restrictedAppsViolation を取得する</span><span class="sxs-lookup"><span data-stu-id="a3a2a-103">Get restrictedAppsViolation</span></span>

> <span data-ttu-id="a3a2a-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a3a2a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a3a2a-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a3a2a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a3a2a-106">[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="a3a2a-106">Read properties and relationships of the [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a3a2a-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="a3a2a-107">Prerequisites</span></span>
<span data-ttu-id="a3a2a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a3a2a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a3a2a-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a3a2a-110">Permission type</span></span>|<span data-ttu-id="a3a2a-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="a3a2a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a3a2a-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a3a2a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a3a2a-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a3a2a-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="a3a2a-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a3a2a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a3a2a-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a3a2a-115">Not supported.</span></span>|
|<span data-ttu-id="a3a2a-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a3a2a-116">Application</span></span>|<span data-ttu-id="a3a2a-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a3a2a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a3a2a-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a3a2a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurationRestrictedAppsViolations/{restrictedAppsViolationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a3a2a-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="a3a2a-119">Optional query parameters</span></span>
<span data-ttu-id="a3a2a-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="a3a2a-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a3a2a-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a3a2a-121">Request headers</span></span>
|<span data-ttu-id="a3a2a-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a3a2a-122">Header</span></span>|<span data-ttu-id="a3a2a-123">値</span><span class="sxs-lookup"><span data-stu-id="a3a2a-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a3a2a-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="a3a2a-124">Authorization</span></span>|<span data-ttu-id="a3a2a-125">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="a3a2a-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a3a2a-126">承諾</span><span class="sxs-lookup"><span data-stu-id="a3a2a-126">Accept</span></span>|<span data-ttu-id="a3a2a-127">application/json</span><span class="sxs-lookup"><span data-stu-id="a3a2a-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a3a2a-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="a3a2a-128">Request body</span></span>
<span data-ttu-id="a3a2a-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="a3a2a-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a3a2a-130">応答</span><span class="sxs-lookup"><span data-stu-id="a3a2a-130">Response</span></span>
<span data-ttu-id="a3a2a-131">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="a3a2a-131">If successful, this method returns a `200 OK` response code and [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a3a2a-132">例</span><span class="sxs-lookup"><span data-stu-id="a3a2a-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="a3a2a-133">要求</span><span class="sxs-lookup"><span data-stu-id="a3a2a-133">Request</span></span>
<span data-ttu-id="a3a2a-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a3a2a-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationRestrictedAppsViolations/{restrictedAppsViolationId}
```

### <a name="response"></a><span data-ttu-id="a3a2a-135">応答</span><span class="sxs-lookup"><span data-stu-id="a3a2a-135">Response</span></span>
<span data-ttu-id="a3a2a-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a3a2a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 664

{
  "value": {
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
}
```





