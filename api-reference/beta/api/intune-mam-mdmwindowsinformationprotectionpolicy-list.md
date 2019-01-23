---
title: mdmWindowsInformationProtectionPolicies のリスト
description: mdmWindowsInformationProtectionPolicy オブジェクトのプロパティとリレーションシップをリストします。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c1cf0712a41261a93bca73e3c6308a5e191dbe83
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29411625"
---
# <a name="list-mdmwindowsinformationprotectionpolicies"></a><span data-ttu-id="a04fe-103">mdmWindowsInformationProtectionPolicies のリスト</span><span class="sxs-lookup"><span data-stu-id="a04fe-103">List mdmWindowsInformationProtectionPolicies</span></span>

> <span data-ttu-id="a04fe-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a04fe-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a04fe-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a04fe-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a04fe-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a04fe-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a04fe-107">[mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="a04fe-107">List properties and relationships of the [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a04fe-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="a04fe-108">Prerequisites</span></span>
<span data-ttu-id="a04fe-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a04fe-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a04fe-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a04fe-111">Permission type</span></span>|<span data-ttu-id="a04fe-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="a04fe-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a04fe-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a04fe-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a04fe-114">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="a04fe-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="a04fe-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a04fe-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a04fe-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a04fe-116">Not supported.</span></span>|
|<span data-ttu-id="a04fe-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a04fe-117">Application</span></span>|<span data-ttu-id="a04fe-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a04fe-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a04fe-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a04fe-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mdmWindowsInformationProtectionPolicies
```

## <a name="request-headers"></a><span data-ttu-id="a04fe-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a04fe-120">Request headers</span></span>
|<span data-ttu-id="a04fe-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a04fe-121">Header</span></span>|<span data-ttu-id="a04fe-122">値</span><span class="sxs-lookup"><span data-stu-id="a04fe-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a04fe-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a04fe-123">Authorization</span></span>|<span data-ttu-id="a04fe-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="a04fe-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a04fe-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a04fe-125">Accept</span></span>|<span data-ttu-id="a04fe-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a04fe-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a04fe-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="a04fe-127">Request body</span></span>
<span data-ttu-id="a04fe-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="a04fe-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a04fe-129">応答</span><span class="sxs-lookup"><span data-stu-id="a04fe-129">Response</span></span>
<span data-ttu-id="a04fe-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="a04fe-130">If successful, this method returns a `200 OK` response code and a collection of [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a04fe-131">例</span><span class="sxs-lookup"><span data-stu-id="a04fe-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="a04fe-132">要求</span><span class="sxs-lookup"><span data-stu-id="a04fe-132">Request</span></span>
<span data-ttu-id="a04fe-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a04fe-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mdmWindowsInformationProtectionPolicies
```

### <a name="response"></a><span data-ttu-id="a04fe-134">応答</span><span class="sxs-lookup"><span data-stu-id="a04fe-134">Response</span></span>
<span data-ttu-id="a04fe-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a04fe-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4684

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mdmWindowsInformationProtectionPolicy",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "id": "8efb0c35-0c35-8efb-350c-fb8e350cfb8e",
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




