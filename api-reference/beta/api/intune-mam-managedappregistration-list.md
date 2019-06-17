---
title: managedAppRegistrations のリスト
description: managedAppRegistration オブジェクトのプロパティとリレーションシップをリストします。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cfb036a0fad602d06a7f0a201b9339aa45ec560e
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34987209"
---
# <a name="list-managedappregistrations"></a><span data-ttu-id="67856-103">managedAppRegistrations のリスト</span><span class="sxs-lookup"><span data-stu-id="67856-103">List managedAppRegistrations</span></span>

> <span data-ttu-id="67856-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="67856-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="67856-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="67856-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="67856-106">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="67856-106">List properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="67856-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="67856-107">Prerequisites</span></span>
<span data-ttu-id="67856-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="67856-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="67856-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="67856-110">Permission type</span></span>|<span data-ttu-id="67856-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="67856-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="67856-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="67856-112">Delegated (work or school account)</span></span>|<span data-ttu-id="67856-113">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="67856-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="67856-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="67856-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="67856-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="67856-115">Not supported.</span></span>|
|<span data-ttu-id="67856-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="67856-116">Application</span></span>|<span data-ttu-id="67856-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="67856-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="67856-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="67856-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppRegistrations
```

## <a name="request-headers"></a><span data-ttu-id="67856-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="67856-119">Request headers</span></span>
|<span data-ttu-id="67856-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="67856-120">Header</span></span>|<span data-ttu-id="67856-121">値</span><span class="sxs-lookup"><span data-stu-id="67856-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="67856-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="67856-122">Authorization</span></span>|<span data-ttu-id="67856-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="67856-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="67856-124">承諾</span><span class="sxs-lookup"><span data-stu-id="67856-124">Accept</span></span>|<span data-ttu-id="67856-125">application/json</span><span class="sxs-lookup"><span data-stu-id="67856-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="67856-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="67856-126">Request body</span></span>
<span data-ttu-id="67856-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="67856-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="67856-128">応答</span><span class="sxs-lookup"><span data-stu-id="67856-128">Response</span></span>
<span data-ttu-id="67856-129">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [managedAppRegistration](../resources/intune-mam-managedappregistration.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="67856-129">If successful, this method returns a `200 OK` response code and a collection of [managedAppRegistration](../resources/intune-mam-managedappregistration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="67856-130">例</span><span class="sxs-lookup"><span data-stu-id="67856-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="67856-131">要求</span><span class="sxs-lookup"><span data-stu-id="67856-131">Request</span></span>
<span data-ttu-id="67856-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="67856-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppRegistrations
```

### <a name="response"></a><span data-ttu-id="67856-133">応答</span><span class="sxs-lookup"><span data-stu-id="67856-133">Response</span></span>
<span data-ttu-id="67856-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="67856-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1014

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedAppRegistration",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
      "applicationVersion": "Application Version value",
      "managementSdkVersion": "Management Sdk Version value",
      "platformVersion": "Platform Version value",
      "deviceType": "Device Type value",
      "deviceTag": "Device Tag value",
      "deviceName": "Device Name value",
      "managedDeviceId": "Managed Device Id value",
      "azureADDeviceId": "Azure ADDevice Id value",
      "deviceModel": "Device Model value",
      "deviceManufacturer": "Device Manufacturer value",
      "flaggedReasons": [
        "rootedDevice"
      ],
      "userId": "User Id value",
      "appIdentifier": {
        "@odata.type": "microsoft.graph.mobileAppIdentifier"
      },
      "id": "5496aa60-aa60-5496-60aa-965460aa9654",
      "version": "Version value"
    }
  ]
}
```





