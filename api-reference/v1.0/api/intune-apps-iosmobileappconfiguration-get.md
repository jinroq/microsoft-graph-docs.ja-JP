---
title: iosMobileAppConfiguration の取得
description: iosMobileAppConfiguration オブジェクトのプロパティとリレーションシップを読み取ります。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5392333d009652fdb9f0ab07b6ce3ad31b6f84a4
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30966895"
---
# <a name="get-iosmobileappconfiguration"></a><span data-ttu-id="f2268-103">iosMobileAppConfiguration の取得</span><span class="sxs-lookup"><span data-stu-id="f2268-103">Get iosMobileAppConfiguration</span></span>

> <span data-ttu-id="f2268-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f2268-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f2268-105">[iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="f2268-105">Read properties and relationships of the [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f2268-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="f2268-106">Prerequisites</span></span>
<span data-ttu-id="f2268-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f2268-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f2268-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f2268-109">Permission type</span></span>|<span data-ttu-id="f2268-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="f2268-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f2268-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f2268-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f2268-112">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f2268-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="f2268-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f2268-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f2268-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f2268-114">Not supported.</span></span>|
|<span data-ttu-id="f2268-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f2268-115">Application</span></span>|<span data-ttu-id="f2268-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f2268-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f2268-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f2268-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f2268-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="f2268-118">Optional query parameters</span></span>
<span data-ttu-id="f2268-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="f2268-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f2268-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f2268-120">Request headers</span></span>
|<span data-ttu-id="f2268-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f2268-121">Header</span></span>|<span data-ttu-id="f2268-122">値</span><span class="sxs-lookup"><span data-stu-id="f2268-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f2268-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f2268-123">Authorization</span></span>|<span data-ttu-id="f2268-124">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="f2268-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f2268-125">承諾</span><span class="sxs-lookup"><span data-stu-id="f2268-125">Accept</span></span>|<span data-ttu-id="f2268-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f2268-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f2268-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="f2268-127">Request body</span></span>
<span data-ttu-id="f2268-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="f2268-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f2268-129">応答</span><span class="sxs-lookup"><span data-stu-id="f2268-129">Response</span></span>
<span data-ttu-id="f2268-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文での [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f2268-130">If successful, this method returns a `200 OK` response code and [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f2268-131">例</span><span class="sxs-lookup"><span data-stu-id="f2268-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="f2268-132">要求</span><span class="sxs-lookup"><span data-stu-id="f2268-132">Request</span></span>
<span data-ttu-id="f2268-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f2268-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

### <a name="response"></a><span data-ttu-id="f2268-134">応答</span><span class="sxs-lookup"><span data-stu-id="f2268-134">Response</span></span>
<span data-ttu-id="f2268-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f2268-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 763

{
  "value": {
    "@odata.type": "#microsoft.graph.iosMobileAppConfiguration",
    "id": "b2c33191-3191-b2c3-9131-c3b29131c3b2",
    "targetedMobileApps": [
      "Targeted Mobile Apps value"
    ],
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "displayName": "Display Name value",
    "version": 7,
    "encodedSettingXml": "ZW5jb2RlZFNldHRpbmdYbWw=",
    "settings": [
      {
        "@odata.type": "microsoft.graph.appConfigurationSettingItem",
        "appConfigKey": "App Config Key value",
        "appConfigKeyType": "integerType",
        "appConfigKeyValue": "App Config Key Value value"
      }
    ]
  }
}
```



