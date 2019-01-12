---
title: windowsInformationProtectionPolicies のリスト
description: windowsInformationProtectionPolicy オブジェクトのプロパティとリレーションシップをリストします。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f1f8e0916b7e777a26e6dedc3c40355073ec6fc7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27991707"
---
# <a name="list-windowsinformationprotectionpolicies"></a><span data-ttu-id="7effd-103">windowsInformationProtectionPolicies のリスト</span><span class="sxs-lookup"><span data-stu-id="7effd-103">List windowsInformationProtectionPolicies</span></span>

> <span data-ttu-id="7effd-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="7effd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7effd-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7effd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7effd-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="7effd-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7effd-107">[windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="7effd-107">List properties and relationships of the [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7effd-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="7effd-108">Prerequisites</span></span>
<span data-ttu-id="7effd-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7effd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7effd-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7effd-111">Permission type</span></span>|<span data-ttu-id="7effd-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="7effd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7effd-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7effd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7effd-114">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="7effd-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="7effd-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7effd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7effd-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7effd-116">Not supported.</span></span>|
|<span data-ttu-id="7effd-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7effd-117">Application</span></span>|<span data-ttu-id="7effd-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7effd-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7effd-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7effd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/windowsInformationProtectionPolicies
```

## <a name="request-headers"></a><span data-ttu-id="7effd-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7effd-120">Request headers</span></span>
|<span data-ttu-id="7effd-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7effd-121">Header</span></span>|<span data-ttu-id="7effd-122">値</span><span class="sxs-lookup"><span data-stu-id="7effd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7effd-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7effd-123">Authorization</span></span>|<span data-ttu-id="7effd-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="7effd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7effd-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7effd-125">Accept</span></span>|<span data-ttu-id="7effd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7effd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7effd-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="7effd-127">Request body</span></span>
<span data-ttu-id="7effd-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="7effd-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7effd-129">応答</span><span class="sxs-lookup"><span data-stu-id="7effd-129">Response</span></span>
<span data-ttu-id="7effd-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="7effd-130">If successful, this method returns a `200 OK` response code and a collection of [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7effd-131">例</span><span class="sxs-lookup"><span data-stu-id="7effd-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="7effd-132">要求</span><span class="sxs-lookup"><span data-stu-id="7effd-132">Request</span></span>
<span data-ttu-id="7effd-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7effd-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/windowsInformationProtectionPolicies
```

### <a name="response"></a><span data-ttu-id="7effd-134">応答</span><span class="sxs-lookup"><span data-stu-id="7effd-134">Response</span></span>
<span data-ttu-id="7effd-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7effd-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 5158

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsInformationProtectionPolicy",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "id": "6397be61-be61-6397-61be-976361be9763",
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
      "isAssigned": true,
      "revokeOnMdmHandoffDisabled": true,
      "mdmEnrollmentUrl": "https://example.com/mdmEnrollmentUrl/",
      "windowsHelloForBusinessBlocked": true,
      "pinMinimumLength": 0,
      "pinUppercaseLetters": "requireAtLeastOne",
      "pinLowercaseLetters": "requireAtLeastOne",
      "pinSpecialCharacters": "requireAtLeastOne",
      "pinExpirationDays": 1,
      "numberOfPastPinsRemembered": 10,
      "passwordMaximumAttemptCount": 11,
      "minutesOfInactivityBeforeDeviceLock": 3,
      "daysWithoutContactBeforeUnenroll": 0
    }
  ]
}
```





