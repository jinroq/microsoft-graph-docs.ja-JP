---
title: Get iosDeviceFeaturesConfiguration
description: iosDeviceFeaturesConfiguration オブジェクトのプロパティとリレーションシップを読み取ります。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a05faa3c6c9fe91797e52a69c63231cff5c9958a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27985866"
---
# <a name="get-iosdevicefeaturesconfiguration"></a><span data-ttu-id="89392-103">Get iosDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="89392-103">Get iosDeviceFeaturesConfiguration</span></span>

> <span data-ttu-id="89392-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="89392-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="89392-105">[iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="89392-105">Read properties and relationships of the [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="89392-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="89392-106">Prerequisites</span></span>
<span data-ttu-id="89392-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="89392-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="89392-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="89392-109">Permission type</span></span>|<span data-ttu-id="89392-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="89392-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="89392-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="89392-111">Delegated (work or school account)</span></span>|<span data-ttu-id="89392-112">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="89392-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="89392-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="89392-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="89392-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="89392-114">Not supported.</span></span>|
|<span data-ttu-id="89392-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="89392-115">Application</span></span>|<span data-ttu-id="89392-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="89392-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="89392-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="89392-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="89392-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="89392-118">Optional query parameters</span></span>
<span data-ttu-id="89392-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="89392-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="89392-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="89392-120">Request headers</span></span>
|<span data-ttu-id="89392-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="89392-121">Header</span></span>|<span data-ttu-id="89392-122">値</span><span class="sxs-lookup"><span data-stu-id="89392-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="89392-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="89392-123">Authorization</span></span>|<span data-ttu-id="89392-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="89392-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="89392-125">Accept</span><span class="sxs-lookup"><span data-stu-id="89392-125">Accept</span></span>|<span data-ttu-id="89392-126">application/json</span><span class="sxs-lookup"><span data-stu-id="89392-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="89392-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="89392-127">Request body</span></span>
<span data-ttu-id="89392-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="89392-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="89392-129">応答</span><span class="sxs-lookup"><span data-stu-id="89392-129">Response</span></span>
<span data-ttu-id="89392-130">このメソッドが成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="89392-130">If successful, this method returns a `200 OK` response code and [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="89392-131">例</span><span class="sxs-lookup"><span data-stu-id="89392-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="89392-132">要求</span><span class="sxs-lookup"><span data-stu-id="89392-132">Request</span></span>
<span data-ttu-id="89392-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="89392-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="89392-134">応答</span><span class="sxs-lookup"><span data-stu-id="89392-134">Response</span></span>
<span data-ttu-id="89392-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="89392-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2313

{
  "value": {
    "@odata.type": "#microsoft.graph.iosDeviceFeaturesConfiguration",
    "id": "651e0ab3-0ab3-651e-b30a-1e65b30a1e65",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "assetTagTemplate": "Asset Tag Template value",
    "lockScreenFootnote": "Lock Screen Footnote value",
    "homeScreenDockIcons": [
      {
        "@odata.type": "microsoft.graph.iosHomeScreenFolder",
        "displayName": "Display Name value",
        "pages": [
          {
            "@odata.type": "microsoft.graph.iosHomeScreenFolderPage",
            "displayName": "Display Name value",
            "apps": [
              {
                "@odata.type": "microsoft.graph.iosHomeScreenApp",
                "displayName": "Display Name value",
                "bundleID": "Bundle ID value"
              }
            ]
          }
        ]
      }
    ],
    "homeScreenPages": [
      {
        "@odata.type": "microsoft.graph.iosHomeScreenPage",
        "displayName": "Display Name value",
        "icons": [
          {
            "@odata.type": "microsoft.graph.iosHomeScreenFolder",
            "displayName": "Display Name value",
            "pages": [
              {
                "@odata.type": "microsoft.graph.iosHomeScreenFolderPage",
                "displayName": "Display Name value",
                "apps": [
                  {
                    "@odata.type": "microsoft.graph.iosHomeScreenApp",
                    "displayName": "Display Name value",
                    "bundleID": "Bundle ID value"
                  }
                ]
              }
            ]
          }
        ]
      }
    ],
    "notificationSettings": [
      {
        "@odata.type": "microsoft.graph.iosNotificationSettings",
        "bundleID": "Bundle ID value",
        "appName": "App Name value",
        "publisher": "Publisher value",
        "enabled": true,
        "showInNotificationCenter": true,
        "showOnLockScreen": true,
        "alertType": "banner",
        "badgesEnabled": true,
        "soundsEnabled": true
      }
    ]
  }
}
```



