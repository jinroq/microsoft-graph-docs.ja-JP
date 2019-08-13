---
title: リスト iosImportedPFXCertificateProfiles
description: IosImportedPFXCertificateProfile オブジェクトのプロパティとリレーションシップをリストします。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 04ec78a7a318d22162a9466e58dbcf08f9087bcb
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36339163"
---
# <a name="list-iosimportedpfxcertificateprofiles"></a><span data-ttu-id="2a578-103">リスト iosImportedPFXCertificateProfiles</span><span class="sxs-lookup"><span data-stu-id="2a578-103">List iosImportedPFXCertificateProfiles</span></span>

> <span data-ttu-id="2a578-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2a578-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2a578-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="2a578-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2a578-106">[IosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="2a578-106">List properties and relationships of the [iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2a578-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="2a578-107">Prerequisites</span></span>
<span data-ttu-id="2a578-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2a578-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2a578-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2a578-110">Permission type</span></span>|<span data-ttu-id="2a578-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="2a578-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2a578-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2a578-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2a578-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="2a578-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="2a578-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2a578-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2a578-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2a578-115">Not supported.</span></span>|
|<span data-ttu-id="2a578-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2a578-116">Application</span></span>|<span data-ttu-id="2a578-117">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="2a578-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2a578-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2a578-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="2a578-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2a578-119">Request headers</span></span>
|<span data-ttu-id="2a578-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2a578-120">Header</span></span>|<span data-ttu-id="2a578-121">値</span><span class="sxs-lookup"><span data-stu-id="2a578-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2a578-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2a578-122">Authorization</span></span>|<span data-ttu-id="2a578-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="2a578-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2a578-124">承諾</span><span class="sxs-lookup"><span data-stu-id="2a578-124">Accept</span></span>|<span data-ttu-id="2a578-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2a578-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2a578-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="2a578-126">Request body</span></span>
<span data-ttu-id="2a578-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="2a578-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2a578-128">応答</span><span class="sxs-lookup"><span data-stu-id="2a578-128">Response</span></span>
<span data-ttu-id="2a578-129">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="2a578-129">If successful, this method returns a `200 OK` response code and a collection of [iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2a578-130">例</span><span class="sxs-lookup"><span data-stu-id="2a578-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="2a578-131">要求</span><span class="sxs-lookup"><span data-stu-id="2a578-131">Request</span></span>
<span data-ttu-id="2a578-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2a578-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="2a578-133">応答</span><span class="sxs-lookup"><span data-stu-id="2a578-133">Response</span></span>
<span data-ttu-id="2a578-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="2a578-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1413

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosImportedPFXCertificateProfile",
      "id": "583b9d8c-9d8c-583b-8c9d-3b588c9d3b58",
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
      "intendedPurpose": "smimeEncryption"
    }
  ]
}
```






