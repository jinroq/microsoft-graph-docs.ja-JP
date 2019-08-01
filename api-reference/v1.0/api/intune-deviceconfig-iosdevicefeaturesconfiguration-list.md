---
title: iosDeviceFeaturesConfigurations のリスト
description: iosDeviceFeaturesConfiguration オブジェクトのプロパティとリレーションシップをリストします。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f941fca80c6ccf39f806bf1eb4b4407a8ef97966
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36018919"
---
# <a name="list-iosdevicefeaturesconfigurations"></a><span data-ttu-id="47245-103">iosDeviceFeaturesConfigurations のリスト</span><span class="sxs-lookup"><span data-stu-id="47245-103">List iosDeviceFeaturesConfigurations</span></span>

> <span data-ttu-id="47245-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="47245-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="47245-105">[iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="47245-105">List properties and relationships of the [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="47245-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="47245-106">Prerequisites</span></span>
<span data-ttu-id="47245-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="47245-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="47245-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="47245-109">Permission type</span></span>|<span data-ttu-id="47245-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="47245-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="47245-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="47245-111">Delegated (work or school account)</span></span>|<span data-ttu-id="47245-112">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="47245-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="47245-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="47245-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="47245-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="47245-114">Not supported.</span></span>|
|<span data-ttu-id="47245-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="47245-115">Application</span></span>|<span data-ttu-id="47245-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="47245-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="47245-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="47245-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="47245-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="47245-118">Request headers</span></span>
|<span data-ttu-id="47245-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="47245-119">Header</span></span>|<span data-ttu-id="47245-120">値</span><span class="sxs-lookup"><span data-stu-id="47245-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="47245-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="47245-121">Authorization</span></span>|<span data-ttu-id="47245-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="47245-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="47245-123">承諾</span><span class="sxs-lookup"><span data-stu-id="47245-123">Accept</span></span>|<span data-ttu-id="47245-124">application/json</span><span class="sxs-lookup"><span data-stu-id="47245-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="47245-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="47245-125">Request body</span></span>
<span data-ttu-id="47245-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="47245-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="47245-127">応答</span><span class="sxs-lookup"><span data-stu-id="47245-127">Response</span></span>
<span data-ttu-id="47245-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="47245-128">If successful, this method returns a `200 OK` response code and a collection of [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="47245-129">例</span><span class="sxs-lookup"><span data-stu-id="47245-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="47245-130">要求</span><span class="sxs-lookup"><span data-stu-id="47245-130">Request</span></span>
<span data-ttu-id="47245-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="47245-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="47245-132">応答</span><span class="sxs-lookup"><span data-stu-id="47245-132">Response</span></span>
<span data-ttu-id="47245-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="47245-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2461

{
  "value": [
    {
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
  ]
}
```



