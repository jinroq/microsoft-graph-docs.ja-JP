---
title: androidManagedAppRegistrations のリスト
description: androidManagedAppRegistration オブジェクトのプロパティとリレーションシップをリストします。
author: tfitzmac
ms.openlocfilehash: e6fb7364e9b3dbef0fff3ca0e779d2740316f6f3
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27343373"
---
# <a name="list-androidmanagedappregistrations"></a><span data-ttu-id="a3bb9-103">androidManagedAppRegistrations のリスト</span><span class="sxs-lookup"><span data-stu-id="a3bb9-103">List androidManagedAppRegistrations</span></span>

> <span data-ttu-id="a3bb9-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="a3bb9-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a3bb9-105">[androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="a3bb9-105">List properties and relationships of the [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a3bb9-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="a3bb9-106">Prerequisites</span></span>
<span data-ttu-id="a3bb9-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a3bb9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a3bb9-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a3bb9-109">Permission type</span></span>|<span data-ttu-id="a3bb9-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="a3bb9-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a3bb9-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a3bb9-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a3bb9-112">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="a3bb9-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="a3bb9-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a3bb9-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a3bb9-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a3bb9-114">Not supported.</span></span>|
|<span data-ttu-id="a3bb9-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a3bb9-115">Application</span></span>|<span data-ttu-id="a3bb9-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a3bb9-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a3bb9-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a3bb9-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppRegistrations
```

## <a name="request-headers"></a><span data-ttu-id="a3bb9-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a3bb9-118">Request headers</span></span>
|<span data-ttu-id="a3bb9-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a3bb9-119">Header</span></span>|<span data-ttu-id="a3bb9-120">値</span><span class="sxs-lookup"><span data-stu-id="a3bb9-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a3bb9-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a3bb9-121">Authorization</span></span>|<span data-ttu-id="a3bb9-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="a3bb9-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a3bb9-123">Accept</span><span class="sxs-lookup"><span data-stu-id="a3bb9-123">Accept</span></span>|<span data-ttu-id="a3bb9-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a3bb9-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a3bb9-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="a3bb9-125">Request body</span></span>
<span data-ttu-id="a3bb9-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="a3bb9-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a3bb9-127">応答</span><span class="sxs-lookup"><span data-stu-id="a3bb9-127">Response</span></span>
<span data-ttu-id="a3bb9-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="a3bb9-128">If successful, this method returns a `200 OK` response code and a collection of [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a3bb9-129">例</span><span class="sxs-lookup"><span data-stu-id="a3bb9-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="a3bb9-130">要求</span><span class="sxs-lookup"><span data-stu-id="a3bb9-130">Request</span></span>
<span data-ttu-id="a3bb9-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a3bb9-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppRegistrations
```

### <a name="response"></a><span data-ttu-id="a3bb9-132">応答</span><span class="sxs-lookup"><span data-stu-id="a3bb9-132">Response</span></span>
<span data-ttu-id="a3bb9-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a3bb9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 862

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidManagedAppRegistration",
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
        "@odata.type": "microsoft.graph.androidMobileAppIdentifier",
        "packageId": "Package Id value"
      },
      "id": "0e064997-4997-0e06-9749-060e9749060e",
      "version": "Version value"
    }
  ]
}
```


