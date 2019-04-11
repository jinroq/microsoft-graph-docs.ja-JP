---
title: macOSDeviceFeaturesConfiguration の取得
description: macOSDeviceFeaturesConfiguration オブジェクトのプロパティとリレーションシップを読み取ります。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 304d365248b05dc1cc0b823905f8f9d189eb3478
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31805384"
---
# <a name="get-macosdevicefeaturesconfiguration"></a><span data-ttu-id="e2859-103">macOSDeviceFeaturesConfiguration の取得</span><span class="sxs-lookup"><span data-stu-id="e2859-103">Get macOSDeviceFeaturesConfiguration</span></span>

> <span data-ttu-id="e2859-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e2859-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e2859-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e2859-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e2859-106">[macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="e2859-106">Read properties and relationships of the [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e2859-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="e2859-107">Prerequisites</span></span>
<span data-ttu-id="e2859-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e2859-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e2859-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e2859-110">Permission type</span></span>|<span data-ttu-id="e2859-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="e2859-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e2859-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e2859-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e2859-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e2859-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="e2859-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e2859-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e2859-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e2859-115">Not supported.</span></span>|
|<span data-ttu-id="e2859-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e2859-116">Application</span></span>|<span data-ttu-id="e2859-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e2859-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e2859-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e2859-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e2859-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="e2859-119">Optional query parameters</span></span>
<span data-ttu-id="e2859-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="e2859-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e2859-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e2859-121">Request headers</span></span>
|<span data-ttu-id="e2859-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e2859-122">Header</span></span>|<span data-ttu-id="e2859-123">値</span><span class="sxs-lookup"><span data-stu-id="e2859-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e2859-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="e2859-124">Authorization</span></span>|<span data-ttu-id="e2859-125">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="e2859-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e2859-126">承諾</span><span class="sxs-lookup"><span data-stu-id="e2859-126">Accept</span></span>|<span data-ttu-id="e2859-127">application/json</span><span class="sxs-lookup"><span data-stu-id="e2859-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e2859-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="e2859-128">Request body</span></span>
<span data-ttu-id="e2859-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="e2859-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e2859-130">応答</span><span class="sxs-lookup"><span data-stu-id="e2859-130">Response</span></span>
<span data-ttu-id="e2859-131">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="e2859-131">If successful, this method returns a `200 OK` response code and [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e2859-132">例</span><span class="sxs-lookup"><span data-stu-id="e2859-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="e2859-133">要求</span><span class="sxs-lookup"><span data-stu-id="e2859-133">Request</span></span>
<span data-ttu-id="e2859-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e2859-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="e2859-135">応答</span><span class="sxs-lookup"><span data-stu-id="e2859-135">Response</span></span>
<span data-ttu-id="e2859-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e2859-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1613

{
  "value": {
    "@odata.type": "#microsoft.graph.macOSDeviceFeaturesConfiguration",
    "id": "49fa957d-957d-49fa-7d95-fa497d95fa49",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "supportsScopeTags": true,
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "airPrintDestinations": [
      {
        "@odata.type": "microsoft.graph.airPrintDestination",
        "ipAddress": "Ip Address value",
        "resourcePath": "Resource Path value",
        "port": 4,
        "forceTls": true
      }
    ],
    "autoLaunchItems": [
      {
        "@odata.type": "microsoft.graph.macOSLaunchItem",
        "path": "Path value",
        "hide": true
      }
    ],
    "adminShowHostInfo": true,
    "loginWindowText": "Login Window Text value",
    "authorizedUsersListHidden": true,
    "authorizedUsersListHideLocalUsers": true,
    "authorizedUsersListHideMobileAccounts": true,
    "authorizedUsersListIncludeNetworkUsers": true,
    "authorizedUsersListHideAdminUsers": true,
    "authorizedUsersListShowOtherManagedUsers": true,
    "shutDownDisabled": true,
    "restartDisabled": true,
    "sleepDisabled": true,
    "consoleAccessDisabled": true,
    "shutDownDisabledWhileLoggedIn": true,
    "restartDisabledWhileLoggedIn": true,
    "powerOffDisabledWhileLoggedIn": true,
    "logOutDisabledWhileLoggedIn": true,
    "screenLockDisableImmediate": true
  }
}
```





