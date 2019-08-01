---
title: sharedPCConfigurations のリスト
description: sharedPCConfiguration オブジェクトのプロパティとリレーションシップをリストします。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8c8f120e1f539ee94ef3c42f9b8c8e9191f651a3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36017048"
---
# <a name="list-sharedpcconfigurations"></a><span data-ttu-id="49bfb-103">sharedPCConfigurations のリスト</span><span class="sxs-lookup"><span data-stu-id="49bfb-103">List sharedPCConfigurations</span></span>

> <span data-ttu-id="49bfb-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="49bfb-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="49bfb-105">[sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="49bfb-105">List properties and relationships of the [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="49bfb-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="49bfb-106">Prerequisites</span></span>
<span data-ttu-id="49bfb-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="49bfb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="49bfb-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="49bfb-109">Permission type</span></span>|<span data-ttu-id="49bfb-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="49bfb-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="49bfb-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="49bfb-111">Delegated (work or school account)</span></span>|<span data-ttu-id="49bfb-112">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="49bfb-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="49bfb-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="49bfb-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="49bfb-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="49bfb-114">Not supported.</span></span>|
|<span data-ttu-id="49bfb-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="49bfb-115">Application</span></span>|<span data-ttu-id="49bfb-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="49bfb-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="49bfb-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="49bfb-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="49bfb-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="49bfb-118">Request headers</span></span>
|<span data-ttu-id="49bfb-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="49bfb-119">Header</span></span>|<span data-ttu-id="49bfb-120">値</span><span class="sxs-lookup"><span data-stu-id="49bfb-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="49bfb-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="49bfb-121">Authorization</span></span>|<span data-ttu-id="49bfb-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="49bfb-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="49bfb-123">承諾</span><span class="sxs-lookup"><span data-stu-id="49bfb-123">Accept</span></span>|<span data-ttu-id="49bfb-124">application/json</span><span class="sxs-lookup"><span data-stu-id="49bfb-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="49bfb-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="49bfb-125">Request body</span></span>
<span data-ttu-id="49bfb-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="49bfb-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="49bfb-127">応答</span><span class="sxs-lookup"><span data-stu-id="49bfb-127">Response</span></span>
<span data-ttu-id="49bfb-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="49bfb-128">If successful, this method returns a `200 OK` response code and a collection of [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="49bfb-129">例</span><span class="sxs-lookup"><span data-stu-id="49bfb-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="49bfb-130">要求</span><span class="sxs-lookup"><span data-stu-id="49bfb-130">Request</span></span>
<span data-ttu-id="49bfb-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="49bfb-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="49bfb-132">応答</span><span class="sxs-lookup"><span data-stu-id="49bfb-132">Response</span></span>
<span data-ttu-id="49bfb-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="49bfb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1165

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.sharedPCConfiguration",
      "id": "5206be3b-be3b-5206-3bbe-06523bbe0652",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "accountManagerPolicy": {
        "@odata.type": "microsoft.graph.sharedPCAccountManagerPolicy",
        "accountDeletionPolicy": "diskSpaceThreshold",
        "cacheAccountsAboveDiskFreePercentage": 4,
        "inactiveThresholdDays": 5,
        "removeAccountsBelowDiskFreePercentage": 5
      },
      "allowedAccounts": "domain",
      "allowLocalStorage": true,
      "disableAccountManager": true,
      "disableEduPolicies": true,
      "disablePowerPolicies": true,
      "disableSignInOnResume": true,
      "enabled": true,
      "idleTimeBeforeSleepInSeconds": 12,
      "kioskAppDisplayName": "Kiosk App Display Name value",
      "kioskAppUserModelId": "Kiosk App User Model Id value",
      "maintenanceStartTime": "11:59:24.7240000"
    }
  ]
}
```



