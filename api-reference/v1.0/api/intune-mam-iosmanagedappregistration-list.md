---
title: iosManagedAppRegistrations のリスト
description: iosManagedAppRegistration オブジェクトのプロパティとリレーションシップをリストします。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 234d2f1f198f5261b6d6f7cc27a63c8464bf1207
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30967245"
---
# <a name="list-iosmanagedappregistrations"></a><span data-ttu-id="9ba56-103">iosManagedAppRegistrations のリスト</span><span class="sxs-lookup"><span data-stu-id="9ba56-103">List iosManagedAppRegistrations</span></span>

> <span data-ttu-id="9ba56-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="9ba56-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9ba56-105">[iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="9ba56-105">List properties and relationships of the [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9ba56-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="9ba56-106">Prerequisites</span></span>
<span data-ttu-id="9ba56-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9ba56-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9ba56-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9ba56-109">Permission type</span></span>|<span data-ttu-id="9ba56-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="9ba56-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9ba56-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9ba56-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9ba56-112">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="9ba56-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="9ba56-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9ba56-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9ba56-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9ba56-114">Not supported.</span></span>|
|<span data-ttu-id="9ba56-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9ba56-115">Application</span></span>|<span data-ttu-id="9ba56-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9ba56-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9ba56-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9ba56-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppRegistrations
```

## <a name="request-headers"></a><span data-ttu-id="9ba56-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9ba56-118">Request headers</span></span>
|<span data-ttu-id="9ba56-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9ba56-119">Header</span></span>|<span data-ttu-id="9ba56-120">値</span><span class="sxs-lookup"><span data-stu-id="9ba56-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9ba56-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="9ba56-121">Authorization</span></span>|<span data-ttu-id="9ba56-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="9ba56-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9ba56-123">承諾</span><span class="sxs-lookup"><span data-stu-id="9ba56-123">Accept</span></span>|<span data-ttu-id="9ba56-124">application/json</span><span class="sxs-lookup"><span data-stu-id="9ba56-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9ba56-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="9ba56-125">Request body</span></span>
<span data-ttu-id="9ba56-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="9ba56-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9ba56-127">応答</span><span class="sxs-lookup"><span data-stu-id="9ba56-127">Response</span></span>
<span data-ttu-id="9ba56-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="9ba56-128">If successful, this method returns a `200 OK` response code and a collection of [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9ba56-129">例</span><span class="sxs-lookup"><span data-stu-id="9ba56-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="9ba56-130">要求</span><span class="sxs-lookup"><span data-stu-id="9ba56-130">Request</span></span>
<span data-ttu-id="9ba56-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="9ba56-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppRegistrations
```

### <a name="response"></a><span data-ttu-id="9ba56-132">応答</span><span class="sxs-lookup"><span data-stu-id="9ba56-132">Response</span></span>
<span data-ttu-id="9ba56-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="9ba56-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 852

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosManagedAppRegistration",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
      "applicationVersion": "Application Version value",
      "managementSdkVersion": "Management Sdk Version value",
      "platformVersion": "Platform Version value",
      "deviceType": "Device Type value",
      "deviceTag": "Device Tag value",
      "deviceName": "Device Name value",
      "flaggedReasons": [
        "rootedDevice"
      ],
      "userId": "User Id value",
      "appIdentifier": {
        "@odata.type": "microsoft.graph.iosMobileAppIdentifier",
        "bundleId": "Bundle Id value"
      },
      "id": "47632c19-2c19-4763-192c-6347192c6347",
      "version": "Version value"
    }
  ]
}
```



