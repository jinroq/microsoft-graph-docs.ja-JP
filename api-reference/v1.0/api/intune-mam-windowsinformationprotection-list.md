---
title: windowsInformationProtections のリスト
description: windowsInformationProtection オブジェクトのプロパティとリレーションシップをリストします。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5554baa268580060ba92bb1159bd0fde1460c232
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36020543"
---
# <a name="list-windowsinformationprotections"></a><span data-ttu-id="c3639-103">windowsInformationProtections のリスト</span><span class="sxs-lookup"><span data-stu-id="c3639-103">List windowsInformationProtections</span></span>

> <span data-ttu-id="c3639-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c3639-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c3639-105">[windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="c3639-105">List properties and relationships of the [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c3639-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="c3639-106">Prerequisites</span></span>
<span data-ttu-id="c3639-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c3639-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c3639-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c3639-109">Permission type</span></span>|<span data-ttu-id="c3639-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="c3639-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c3639-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c3639-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c3639-112">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c3639-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="c3639-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c3639-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c3639-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c3639-114">Not supported.</span></span>|
|<span data-ttu-id="c3639-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c3639-115">Application</span></span>|<span data-ttu-id="c3639-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c3639-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c3639-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c3639-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppPolicies
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies
```

## <a name="request-headers"></a><span data-ttu-id="c3639-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c3639-118">Request headers</span></span>
|<span data-ttu-id="c3639-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c3639-119">Header</span></span>|<span data-ttu-id="c3639-120">値</span><span class="sxs-lookup"><span data-stu-id="c3639-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c3639-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c3639-121">Authorization</span></span>|<span data-ttu-id="c3639-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="c3639-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c3639-123">承諾</span><span class="sxs-lookup"><span data-stu-id="c3639-123">Accept</span></span>|<span data-ttu-id="c3639-124">application/json</span><span class="sxs-lookup"><span data-stu-id="c3639-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c3639-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="c3639-125">Request body</span></span>
<span data-ttu-id="c3639-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="c3639-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c3639-127">応答</span><span class="sxs-lookup"><span data-stu-id="c3639-127">Response</span></span>
<span data-ttu-id="c3639-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="c3639-128">If successful, this method returns a `200 OK` response code and a collection of [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c3639-129">例</span><span class="sxs-lookup"><span data-stu-id="c3639-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="c3639-130">要求</span><span class="sxs-lookup"><span data-stu-id="c3639-130">Request</span></span>
<span data-ttu-id="c3639-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c3639-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppPolicies
```

### <a name="response"></a><span data-ttu-id="c3639-132">応答</span><span class="sxs-lookup"><span data-stu-id="c3639-132">Response</span></span>
<span data-ttu-id="c3639-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c3639-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4601

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsInformationProtection",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "id": "ca339419-9419-ca33-1994-33ca199433ca",
      "version": "Version value",
      "enforcementLevel": "encryptAndAuditOnly",
      "enterpriseDomain": "Enterprise Domain value",
      "enterpriseProtectedDomainNames": [
        {
          "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
          "displayName": "Display Name value",
          "resources": [
            "Resources value"
          ]
        }
      ],
      "protectionUnderLockConfigRequired": true,
      "dataRecoveryCertificate": {
        "@odata.type": "microsoft.graph.windowsInformationProtectionDataRecoveryCertificate",
        "subjectName": "Subject Name value",
        "description": "Description value",
        "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
        "certificate": "Y2VydGlmaWNhdGU="
      },
      "revokeOnUnenrollDisabled": true,
      "rightsManagementServicesTemplateId": "abf7b16f-b16f-abf7-6fb1-f7ab6fb1f7ab",
      "azureRightsManagementServicesAllowed": true,
      "iconsVisible": true,
      "protectedApps": [
        {
          "@odata.type": "microsoft.graph.windowsInformationProtectionStoreApp",
          "displayName": "Display Name value",
          "description": "Description value",
          "publisherName": "Publisher Name value",
          "productName": "Product Name value",
          "denied": true
        }
      ],
      "exemptApps": [
        {
          "@odata.type": "microsoft.graph.windowsInformationProtectionStoreApp",
          "displayName": "Display Name value",
          "description": "Description value",
          "publisherName": "Publisher Name value",
          "productName": "Product Name value",
          "denied": true
        }
      ],
      "enterpriseNetworkDomainNames": [
        {
          "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
          "displayName": "Display Name value",
          "resources": [
            "Resources value"
          ]
        }
      ],
      "enterpriseProxiedDomains": [
        {
          "@odata.type": "microsoft.graph.windowsInformationProtectionProxiedDomainCollection",
          "displayName": "Display Name value",
          "proxiedDomains": [
            {
              "@odata.type": "microsoft.graph.proxiedDomain",
              "ipAddressOrFQDN": "Ip Address Or FQDN value",
              "proxy": "Proxy value"
            }
          ]
        }
      ],
      "enterpriseIPRanges": [
        {
          "@odata.type": "microsoft.graph.windowsInformationProtectionIPRangeCollection",
          "displayName": "Display Name value",
          "ranges": [
            {
              "@odata.type": "microsoft.graph.iPv6Range",
              "lowerAddress": "Lower Address value",
              "upperAddress": "Upper Address value"
            }
          ]
        }
      ],
      "enterpriseIPRangesAreAuthoritative": true,
      "enterpriseProxyServers": [
        {
          "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
          "displayName": "Display Name value",
          "resources": [
            "Resources value"
          ]
        }
      ],
      "enterpriseInternalProxyServers": [
        {
          "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
          "displayName": "Display Name value",
          "resources": [
            "Resources value"
          ]
        }
      ],
      "enterpriseProxyServersAreAuthoritative": true,
      "neutralDomainResources": [
        {
          "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
          "displayName": "Display Name value",
          "resources": [
            "Resources value"
          ]
        }
      ],
      "indexingEncryptedStoresOrItemsBlocked": true,
      "smbAutoEncryptedFileExtensions": [
        {
          "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
          "displayName": "Display Name value",
          "resources": [
            "Resources value"
          ]
        }
      ],
      "isAssigned": true
    }
  ]
}
```



