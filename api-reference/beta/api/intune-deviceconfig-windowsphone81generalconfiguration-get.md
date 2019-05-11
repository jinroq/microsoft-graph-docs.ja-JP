---
title: Get windowsPhone81GeneralConfiguration
description: windowsPhone81GeneralConfiguration オブジェクトのプロパティとリレーションシップを読み取ります。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 49bfc832fa3b09d6b534a3b3380baff6c103d205
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33917766"
---
# <a name="get-windowsphone81generalconfiguration"></a><span data-ttu-id="14999-103">Get windowsPhone81GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="14999-103">Get windowsPhone81GeneralConfiguration</span></span>

> <span data-ttu-id="14999-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="14999-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="14999-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="14999-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="14999-106">[windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="14999-106">Read properties and relationships of the [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="14999-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="14999-107">Prerequisites</span></span>
<span data-ttu-id="14999-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="14999-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="14999-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="14999-110">Permission type</span></span>|<span data-ttu-id="14999-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="14999-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="14999-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="14999-112">Delegated (work or school account)</span></span>|<span data-ttu-id="14999-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="14999-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="14999-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="14999-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="14999-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="14999-115">Not supported.</span></span>|
|<span data-ttu-id="14999-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="14999-116">Application</span></span>|<span data-ttu-id="14999-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="14999-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="14999-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="14999-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="14999-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="14999-119">Optional query parameters</span></span>
<span data-ttu-id="14999-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="14999-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="14999-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="14999-121">Request headers</span></span>
|<span data-ttu-id="14999-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="14999-122">Header</span></span>|<span data-ttu-id="14999-123">値</span><span class="sxs-lookup"><span data-stu-id="14999-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="14999-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="14999-124">Authorization</span></span>|<span data-ttu-id="14999-125">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="14999-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="14999-126">承諾</span><span class="sxs-lookup"><span data-stu-id="14999-126">Accept</span></span>|<span data-ttu-id="14999-127">application/json</span><span class="sxs-lookup"><span data-stu-id="14999-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="14999-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="14999-128">Request body</span></span>
<span data-ttu-id="14999-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="14999-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="14999-130">応答</span><span class="sxs-lookup"><span data-stu-id="14999-130">Response</span></span>
<span data-ttu-id="14999-131">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="14999-131">If successful, this method returns a `200 OK` response code and [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="14999-132">例</span><span class="sxs-lookup"><span data-stu-id="14999-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="14999-133">要求</span><span class="sxs-lookup"><span data-stu-id="14999-133">Request</span></span>
<span data-ttu-id="14999-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="14999-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="14999-135">応答</span><span class="sxs-lookup"><span data-stu-id="14999-135">Response</span></span>
<span data-ttu-id="14999-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="14999-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1840

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsPhone81GeneralConfiguration",
    "id": "f5e0e34d-e34d-f5e0-4de3-e0f54de3e0f5",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "supportsScopeTags": true,
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "applyOnlyToWindowsPhone81": true,
    "appsBlockCopyPaste": true,
    "bluetoothBlocked": true,
    "cameraBlocked": true,
    "cellularBlockWifiTethering": true,
    "compliantAppsList": [
      {
        "@odata.type": "microsoft.graph.appListItem",
        "name": "Name value",
        "publisher": "Publisher value",
        "appStoreUrl": "https://example.com/appStoreUrl/",
        "appId": "App Id value"
      }
    ],
    "compliantAppListType": "appsInListCompliant",
    "diagnosticDataBlockSubmission": true,
    "emailBlockAddingAccounts": true,
    "locationServicesBlocked": true,
    "microsoftAccountBlocked": true,
    "nfcBlocked": true,
    "passwordBlockSimple": true,
    "passwordExpirationDays": 6,
    "passwordMinimumLength": 5,
    "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
    "passwordMinimumCharacterSetCount": 0,
    "passwordPreviousPasswordBlockCount": 2,
    "passwordSignInFailureCountBeforeFactoryReset": 12,
    "passwordRequiredType": "alphanumeric",
    "passwordRequired": true,
    "screenCaptureBlocked": true,
    "storageBlockRemovableStorage": true,
    "storageRequireEncryption": true,
    "webBrowserBlocked": true,
    "wifiBlocked": true,
    "wifiBlockAutomaticConnectHotspots": true,
    "wifiBlockHotspotReporting": true,
    "windowsStoreBlocked": true
  }
}
```




