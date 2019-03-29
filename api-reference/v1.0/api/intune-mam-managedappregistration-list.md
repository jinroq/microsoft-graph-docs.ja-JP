---
title: managedAppRegistrations のリスト
description: managedAppRegistration オブジェクトのプロパティとリレーションシップをリストします。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 94738c4b0aef555a536ceec2533db241007251a4
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30975309"
---
# <a name="list-managedappregistrations"></a><span data-ttu-id="f792b-103">managedAppRegistrations のリスト</span><span class="sxs-lookup"><span data-stu-id="f792b-103">List managedAppRegistrations</span></span>

> <span data-ttu-id="f792b-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f792b-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f792b-105">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="f792b-105">List properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f792b-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="f792b-106">Prerequisites</span></span>
<span data-ttu-id="f792b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f792b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f792b-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f792b-109">Permission type</span></span>|<span data-ttu-id="f792b-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="f792b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f792b-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f792b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f792b-112">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f792b-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="f792b-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f792b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f792b-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f792b-114">Not supported.</span></span>|
|<span data-ttu-id="f792b-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f792b-115">Application</span></span>|<span data-ttu-id="f792b-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f792b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f792b-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f792b-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppRegistrations
```

## <a name="request-headers"></a><span data-ttu-id="f792b-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f792b-118">Request headers</span></span>
|<span data-ttu-id="f792b-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f792b-119">Header</span></span>|<span data-ttu-id="f792b-120">値</span><span class="sxs-lookup"><span data-stu-id="f792b-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f792b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f792b-121">Authorization</span></span>|<span data-ttu-id="f792b-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="f792b-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f792b-123">承諾</span><span class="sxs-lookup"><span data-stu-id="f792b-123">Accept</span></span>|<span data-ttu-id="f792b-124">application/json</span><span class="sxs-lookup"><span data-stu-id="f792b-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f792b-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="f792b-125">Request body</span></span>
<span data-ttu-id="f792b-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="f792b-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f792b-127">応答</span><span class="sxs-lookup"><span data-stu-id="f792b-127">Response</span></span>
<span data-ttu-id="f792b-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [managedAppRegistration](../resources/intune-mam-managedappregistration.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="f792b-128">If successful, this method returns a `200 OK` response code and a collection of [managedAppRegistration](../resources/intune-mam-managedappregistration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f792b-129">例</span><span class="sxs-lookup"><span data-stu-id="f792b-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="f792b-130">要求</span><span class="sxs-lookup"><span data-stu-id="f792b-130">Request</span></span>
<span data-ttu-id="f792b-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f792b-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppRegistrations
```

### <a name="response"></a><span data-ttu-id="f792b-132">応答</span><span class="sxs-lookup"><span data-stu-id="f792b-132">Response</span></span>
<span data-ttu-id="f792b-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f792b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 806

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



