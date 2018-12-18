---
title: Get sharedPCConfiguration
description: sharedPCConfiguration オブジェクトのプロパティとリレーションシップを読み取ります。
author: tfitzmac
ms.openlocfilehash: 477103638c0d0315ee285c21b4572328038759fa
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27344759"
---
# <a name="get-sharedpcconfiguration"></a><span data-ttu-id="96245-103">Get sharedPCConfiguration</span><span class="sxs-lookup"><span data-stu-id="96245-103">Get sharedPCConfiguration</span></span>

> <span data-ttu-id="96245-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="96245-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="96245-105">[sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="96245-105">Read properties and relationships of the [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="96245-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="96245-106">Prerequisites</span></span>
<span data-ttu-id="96245-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="96245-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="96245-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="96245-109">Permission type</span></span>|<span data-ttu-id="96245-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="96245-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="96245-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="96245-111">Delegated (work or school account)</span></span>|<span data-ttu-id="96245-112">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="96245-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="96245-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="96245-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="96245-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="96245-114">Not supported.</span></span>|
|<span data-ttu-id="96245-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="96245-115">Application</span></span>|<span data-ttu-id="96245-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="96245-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="96245-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="96245-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="96245-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="96245-118">Optional query parameters</span></span>
<span data-ttu-id="96245-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="96245-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="96245-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="96245-120">Request headers</span></span>
|<span data-ttu-id="96245-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="96245-121">Header</span></span>|<span data-ttu-id="96245-122">値</span><span class="sxs-lookup"><span data-stu-id="96245-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="96245-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="96245-123">Authorization</span></span>|<span data-ttu-id="96245-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="96245-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="96245-125">Accept</span><span class="sxs-lookup"><span data-stu-id="96245-125">Accept</span></span>|<span data-ttu-id="96245-126">application/json</span><span class="sxs-lookup"><span data-stu-id="96245-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="96245-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="96245-127">Request body</span></span>
<span data-ttu-id="96245-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="96245-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="96245-129">応答</span><span class="sxs-lookup"><span data-stu-id="96245-129">Response</span></span>
<span data-ttu-id="96245-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="96245-130">If successful, this method returns a `200 OK` response code and [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="96245-131">例</span><span class="sxs-lookup"><span data-stu-id="96245-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="96245-132">要求</span><span class="sxs-lookup"><span data-stu-id="96245-132">Request</span></span>
<span data-ttu-id="96245-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="96245-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="96245-134">応答</span><span class="sxs-lookup"><span data-stu-id="96245-134">Response</span></span>
<span data-ttu-id="96245-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="96245-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1101

{
  "value": {
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
}
```



