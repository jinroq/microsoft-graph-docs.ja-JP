---
title: windowsInformationProtectionPolicy の取得
description: windowsInformationProtectionPolicy オブジェクトのプロパティとリレーションシップを読み取ります。
author: tfitzmac
ms.openlocfilehash: 83c84982f55f0b891886acefac6e0c5eca57b850
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27311705"
---
# <a name="get-windowsinformationprotectionpolicy"></a><span data-ttu-id="f2198-103">windowsInformationProtectionPolicy の取得</span><span class="sxs-lookup"><span data-stu-id="f2198-103">Get windowsInformationProtectionPolicy</span></span>

> <span data-ttu-id="f2198-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="f2198-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f2198-105">[windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="f2198-105">Read properties and relationships of the [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f2198-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="f2198-106">Prerequisites</span></span>
<span data-ttu-id="f2198-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f2198-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f2198-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f2198-109">Permission type</span></span>|<span data-ttu-id="f2198-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="f2198-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f2198-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f2198-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f2198-112">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f2198-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="f2198-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f2198-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f2198-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f2198-114">Not supported.</span></span>|
|<span data-ttu-id="f2198-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f2198-115">Application</span></span>|<span data-ttu-id="f2198-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f2198-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f2198-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f2198-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f2198-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="f2198-118">Optional query parameters</span></span>
<span data-ttu-id="f2198-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="f2198-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="f2198-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f2198-120">Request headers</span></span>
|<span data-ttu-id="f2198-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f2198-121">Header</span></span>|<span data-ttu-id="f2198-122">値</span><span class="sxs-lookup"><span data-stu-id="f2198-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f2198-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f2198-123">Authorization</span></span>|<span data-ttu-id="f2198-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="f2198-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f2198-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f2198-125">Accept</span></span>|<span data-ttu-id="f2198-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f2198-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f2198-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="f2198-127">Request body</span></span>
<span data-ttu-id="f2198-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="f2198-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f2198-129">応答</span><span class="sxs-lookup"><span data-stu-id="f2198-129">Response</span></span>
<span data-ttu-id="f2198-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f2198-130">If successful, this method returns a `200 OK` response code and [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f2198-131">例</span><span class="sxs-lookup"><span data-stu-id="f2198-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="f2198-132">要求</span><span class="sxs-lookup"><span data-stu-id="f2198-132">Request</span></span>
<span data-ttu-id="f2198-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f2198-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}
```

### <a name="response"></a><span data-ttu-id="f2198-134">応答</span><span class="sxs-lookup"><span data-stu-id="f2198-134">Response</span></span>
<span data-ttu-id="f2198-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f2198-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4870

{
  "value": {
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
}
```


