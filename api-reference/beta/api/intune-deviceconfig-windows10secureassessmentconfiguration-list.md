---
title: windows10SecureAssessmentConfigurations のリスト
description: windows10SecureAssessmentConfiguration オブジェクトのプロパティとリレーションシップをリストします。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fa583a384f118b9ffaead2f00583cef78ca0c8f5
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35715271"
---
# <a name="list-windows10secureassessmentconfigurations"></a><span data-ttu-id="fced6-103">windows10SecureAssessmentConfigurations のリスト</span><span class="sxs-lookup"><span data-stu-id="fced6-103">List windows10SecureAssessmentConfigurations</span></span>

> <span data-ttu-id="fced6-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fced6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fced6-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="fced6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fced6-106">[windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="fced6-106">List properties and relationships of the [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fced6-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="fced6-107">Prerequisites</span></span>
<span data-ttu-id="fced6-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fced6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fced6-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="fced6-110">Permission type</span></span>|<span data-ttu-id="fced6-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="fced6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fced6-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="fced6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fced6-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="fced6-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="fced6-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="fced6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fced6-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fced6-115">Not supported.</span></span>|
|<span data-ttu-id="fced6-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="fced6-116">Application</span></span>|<span data-ttu-id="fced6-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fced6-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fced6-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="fced6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="fced6-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fced6-119">Request headers</span></span>
|<span data-ttu-id="fced6-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fced6-120">Header</span></span>|<span data-ttu-id="fced6-121">値</span><span class="sxs-lookup"><span data-stu-id="fced6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fced6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="fced6-122">Authorization</span></span>|<span data-ttu-id="fced6-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="fced6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fced6-124">承諾</span><span class="sxs-lookup"><span data-stu-id="fced6-124">Accept</span></span>|<span data-ttu-id="fced6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fced6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fced6-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="fced6-126">Request body</span></span>
<span data-ttu-id="fced6-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="fced6-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fced6-128">応答</span><span class="sxs-lookup"><span data-stu-id="fced6-128">Response</span></span>
<span data-ttu-id="fced6-129">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="fced6-129">If successful, this method returns a `200 OK` response code and a collection of [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fced6-130">例</span><span class="sxs-lookup"><span data-stu-id="fced6-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="fced6-131">要求</span><span class="sxs-lookup"><span data-stu-id="fced6-131">Request</span></span>
<span data-ttu-id="fced6-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="fced6-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="fced6-133">応答</span><span class="sxs-lookup"><span data-stu-id="fced6-133">Response</span></span>
<span data-ttu-id="fced6-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="fced6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1768

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windows10SecureAssessmentConfiguration",
      "id": "f60d71be-71be-f60d-be71-0df6be710df6",
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
      "launchUri": "Launch Uri value",
      "configurationAccount": "Configuration Account value",
      "configurationAccountType": "domainAccount",
      "allowPrinting": true,
      "allowScreenCapture": true,
      "allowTextSuggestion": true,
      "localGuestAccountName": "Local Guest Account Name value",
      "assessmentAppUserModelId": "Assessment App User Model Id value"
    }
  ]
}
```





