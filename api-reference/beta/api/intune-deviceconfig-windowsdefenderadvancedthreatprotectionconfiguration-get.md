---
title: windowsDefenderAdvancedThreatProtectionConfiguration の取得
description: windowsDefenderAdvancedThreatProtectionConfiguration オブジェクトのプロパティとリレーションシップを読み取ります。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0d1c0318158323a8ef7d7cdbcba5fbb76ae1c76f
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31796305"
---
# <a name="get-windowsdefenderadvancedthreatprotectionconfiguration"></a><span data-ttu-id="e8789-103">windowsDefenderAdvancedThreatProtectionConfiguration の取得</span><span class="sxs-lookup"><span data-stu-id="e8789-103">Get windowsDefenderAdvancedThreatProtectionConfiguration</span></span>

> <span data-ttu-id="e8789-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e8789-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e8789-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e8789-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e8789-106">[windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="e8789-106">Read properties and relationships of the [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e8789-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="e8789-107">Prerequisites</span></span>
<span data-ttu-id="e8789-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e8789-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e8789-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e8789-110">Permission type</span></span>|<span data-ttu-id="e8789-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="e8789-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e8789-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e8789-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e8789-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e8789-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="e8789-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e8789-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e8789-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e8789-115">Not supported.</span></span>|
|<span data-ttu-id="e8789-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e8789-116">Application</span></span>|<span data-ttu-id="e8789-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e8789-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e8789-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e8789-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e8789-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="e8789-119">Optional query parameters</span></span>
<span data-ttu-id="e8789-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="e8789-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e8789-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e8789-121">Request headers</span></span>
|<span data-ttu-id="e8789-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e8789-122">Header</span></span>|<span data-ttu-id="e8789-123">値</span><span class="sxs-lookup"><span data-stu-id="e8789-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e8789-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="e8789-124">Authorization</span></span>|<span data-ttu-id="e8789-125">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="e8789-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e8789-126">承諾</span><span class="sxs-lookup"><span data-stu-id="e8789-126">Accept</span></span>|<span data-ttu-id="e8789-127">application/json</span><span class="sxs-lookup"><span data-stu-id="e8789-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e8789-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="e8789-128">Request body</span></span>
<span data-ttu-id="e8789-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="e8789-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e8789-130">応答</span><span class="sxs-lookup"><span data-stu-id="e8789-130">Response</span></span>
<span data-ttu-id="e8789-131">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="e8789-131">If successful, this method returns a `200 OK` response code and [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e8789-132">例</span><span class="sxs-lookup"><span data-stu-id="e8789-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="e8789-133">要求</span><span class="sxs-lookup"><span data-stu-id="e8789-133">Request</span></span>
<span data-ttu-id="e8789-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e8789-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="e8789-135">応答</span><span class="sxs-lookup"><span data-stu-id="e8789-135">Response</span></span>
<span data-ttu-id="e8789-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e8789-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1057

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsDefenderAdvancedThreatProtectionConfiguration",
    "id": "294373aa-73aa-2943-aa73-4329aa734329",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "supportsScopeTags": true,
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "advancedThreatProtectionOnboardingBlob": "Advanced Threat Protection Onboarding Blob value",
    "advancedThreatProtectionOnboardingFilename": "Advanced Threat Protection Onboarding Filename value",
    "advancedThreatProtectionAutoPopulateOnboardingBlob": true,
    "allowSampleSharing": true,
    "enableExpeditedTelemetryReporting": true,
    "advancedThreatProtectionOffboardingBlob": "Advanced Threat Protection Offboarding Blob value",
    "advancedThreatProtectionOffboardingFilename": "Advanced Threat Protection Offboarding Filename value"
  }
}
```





