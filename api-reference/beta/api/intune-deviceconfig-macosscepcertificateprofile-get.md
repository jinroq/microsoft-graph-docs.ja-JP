---
title: MacOSScepCertificateProfile の取得
description: MacOSScepCertificateProfile オブジェクトのプロパティとリレーションシップを読み取ります。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8b3689a36a081f1d81aa464eb4ac813e13aeffb9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35947089"
---
# <a name="get-macosscepcertificateprofile"></a><span data-ttu-id="2ed37-103">MacOSScepCertificateProfile の取得</span><span class="sxs-lookup"><span data-stu-id="2ed37-103">Get macOSScepCertificateProfile</span></span>

> <span data-ttu-id="2ed37-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2ed37-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2ed37-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="2ed37-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2ed37-106">[Macosscepcertificateprofile](../resources/intune-deviceconfig-macosscepcertificateprofile.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="2ed37-106">Read properties and relationships of the [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2ed37-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="2ed37-107">Prerequisites</span></span>
<span data-ttu-id="2ed37-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2ed37-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2ed37-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2ed37-110">Permission type</span></span>|<span data-ttu-id="2ed37-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="2ed37-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2ed37-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2ed37-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2ed37-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="2ed37-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="2ed37-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2ed37-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2ed37-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2ed37-115">Not supported.</span></span>|
|<span data-ttu-id="2ed37-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2ed37-116">Application</span></span>|<span data-ttu-id="2ed37-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2ed37-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2ed37-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2ed37-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2ed37-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="2ed37-119">Optional query parameters</span></span>
<span data-ttu-id="2ed37-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="2ed37-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2ed37-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2ed37-121">Request headers</span></span>
|<span data-ttu-id="2ed37-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2ed37-122">Header</span></span>|<span data-ttu-id="2ed37-123">値</span><span class="sxs-lookup"><span data-stu-id="2ed37-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2ed37-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="2ed37-124">Authorization</span></span>|<span data-ttu-id="2ed37-125">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="2ed37-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2ed37-126">承諾</span><span class="sxs-lookup"><span data-stu-id="2ed37-126">Accept</span></span>|<span data-ttu-id="2ed37-127">application/json</span><span class="sxs-lookup"><span data-stu-id="2ed37-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2ed37-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="2ed37-128">Request body</span></span>
<span data-ttu-id="2ed37-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="2ed37-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2ed37-130">応答</span><span class="sxs-lookup"><span data-stu-id="2ed37-130">Response</span></span>
<span data-ttu-id="2ed37-131">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[Macosscepcertificateprofile](../resources/intune-deviceconfig-macosscepcertificateprofile.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="2ed37-131">If successful, this method returns a `200 OK` response code and [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2ed37-132">例</span><span class="sxs-lookup"><span data-stu-id="2ed37-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="2ed37-133">要求</span><span class="sxs-lookup"><span data-stu-id="2ed37-133">Request</span></span>
<span data-ttu-id="2ed37-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2ed37-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="2ed37-135">応答</span><span class="sxs-lookup"><span data-stu-id="2ed37-135">Response</span></span>
<span data-ttu-id="2ed37-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="2ed37-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2273

{
  "value": {
    "@odata.type": "#microsoft.graph.macOSScepCertificateProfile",
    "id": "78c3929d-929d-78c3-9d92-c3789d92c378",
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
    "renewalThresholdPercentage": 10,
    "subjectNameFormat": "commonNameAsEmail",
    "subjectAlternativeNameType": "emailAddress",
    "certificateValidityPeriodValue": 14,
    "certificateValidityPeriodScale": "months",
    "scepServerUrls": [
      "Scep Server Urls value"
    ],
    "subjectNameFormatString": "Subject Name Format String value",
    "keyUsage": "digitalSignature",
    "keySize": "size2048",
    "hashAlgorithm": "sha2",
    "extendedKeyUsages": [
      {
        "@odata.type": "microsoft.graph.extendedKeyUsage",
        "name": "Name value",
        "objectIdentifier": "Object Identifier value"
      }
    ],
    "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
    "certificateStore": "machine",
    "customSubjectAlternativeNames": [
      {
        "@odata.type": "microsoft.graph.customSubjectAlternativeName",
        "sanType": "emailAddress",
        "name": "Name value"
      }
    ]
  }
}
```





