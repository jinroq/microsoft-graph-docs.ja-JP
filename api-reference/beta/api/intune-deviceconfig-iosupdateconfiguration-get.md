---
title: Get iosUpdateConfiguration
description: iosUpdateConfiguration オブジェクトのプロパティとリレーションシップを読み取ります。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 98f718c6efa21e29a3471858f19977e08e8f1a40
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35947859"
---
# <a name="get-iosupdateconfiguration"></a><span data-ttu-id="6f243-103">Get iosUpdateConfiguration</span><span class="sxs-lookup"><span data-stu-id="6f243-103">Get iosUpdateConfiguration</span></span>

> <span data-ttu-id="6f243-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6f243-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6f243-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="6f243-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6f243-106">[iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="6f243-106">Read properties and relationships of the [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6f243-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="6f243-107">Prerequisites</span></span>
<span data-ttu-id="6f243-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6f243-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6f243-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6f243-110">Permission type</span></span>|<span data-ttu-id="6f243-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="6f243-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6f243-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6f243-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6f243-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="6f243-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="6f243-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6f243-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6f243-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6f243-115">Not supported.</span></span>|
|<span data-ttu-id="6f243-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6f243-116">Application</span></span>|<span data-ttu-id="6f243-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6f243-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6f243-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6f243-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6f243-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="6f243-119">Optional query parameters</span></span>
<span data-ttu-id="6f243-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="6f243-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6f243-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6f243-121">Request headers</span></span>
|<span data-ttu-id="6f243-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6f243-122">Header</span></span>|<span data-ttu-id="6f243-123">値</span><span class="sxs-lookup"><span data-stu-id="6f243-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6f243-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="6f243-124">Authorization</span></span>|<span data-ttu-id="6f243-125">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="6f243-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6f243-126">承諾</span><span class="sxs-lookup"><span data-stu-id="6f243-126">Accept</span></span>|<span data-ttu-id="6f243-127">application/json</span><span class="sxs-lookup"><span data-stu-id="6f243-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6f243-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="6f243-128">Request body</span></span>
<span data-ttu-id="6f243-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="6f243-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6f243-130">応答</span><span class="sxs-lookup"><span data-stu-id="6f243-130">Response</span></span>
<span data-ttu-id="6f243-131">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="6f243-131">If successful, this method returns a `200 OK` response code and [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6f243-132">例</span><span class="sxs-lookup"><span data-stu-id="6f243-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="6f243-133">要求</span><span class="sxs-lookup"><span data-stu-id="6f243-133">Request</span></span>
<span data-ttu-id="6f243-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="6f243-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="6f243-135">応答</span><span class="sxs-lookup"><span data-stu-id="6f243-135">Response</span></span>
<span data-ttu-id="6f243-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="6f243-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1526

{
  "value": {
    "@odata.type": "#microsoft.graph.iosUpdateConfiguration",
    "id": "321aef09-ef09-321a-09ef-1a3209ef1a32",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "supportsScopeTags": true,
    "deviceManagementApplicabilityRuleOsEdition": {
      "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
      "osEditionTypes": [
        "windows10EnterpriseN"
      ],
      "name": "Name value",
      "ruleType": "exclude"
    },
    "deviceManagementApplicabilityRuleOsVersion": {
      "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
      "minOSVersion": "Min OSVersion value",
      "maxOSVersion": "Max OSVersion value",
      "name": "Name value",
      "ruleType": "exclude"
    },
    "deviceManagementApplicabilityRuleDeviceMode": {
      "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
      "deviceMode": "sModeConfiguration",
      "name": "Name value",
      "ruleType": "exclude"
    },
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "isEnabled": true,
    "activeHoursStart": "12:00:05.5020000",
    "activeHoursEnd": "11:59:00.8990000",
    "scheduledInstallDays": [
      "monday"
    ],
    "utcTimeOffsetInMinutes": 6,
    "enforcedSoftwareUpdateDelayInDays": 1
  }
}
```





