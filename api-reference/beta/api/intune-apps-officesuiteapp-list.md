---
title: リスト officeSuiteApps
description: officeSuiteApp オブジェクトのプロパティとリレーションシップをリストします。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e4d0d7172c29c9385b0772f551d4c817bac8da4b
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30150100"
---
# <a name="list-officesuiteapps"></a><span data-ttu-id="d0ead-103">リスト officeSuiteApps</span><span class="sxs-lookup"><span data-stu-id="d0ead-103">List officeSuiteApps</span></span>

> <span data-ttu-id="d0ead-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d0ead-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d0ead-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d0ead-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d0ead-106">[officeSuiteApp](../resources/intune-apps-officesuiteapp.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="d0ead-106">List properties and relationships of the [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d0ead-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="d0ead-107">Prerequisites</span></span>
<span data-ttu-id="d0ead-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d0ead-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="d0ead-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d0ead-110">Permission type</span></span>|<span data-ttu-id="d0ead-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="d0ead-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d0ead-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d0ead-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d0ead-113">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="d0ead-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="d0ead-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d0ead-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d0ead-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d0ead-115">Not supported.</span></span>|
|<span data-ttu-id="d0ead-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d0ead-116">Application</span></span>|<span data-ttu-id="d0ead-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d0ead-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d0ead-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d0ead-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="d0ead-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d0ead-119">Request headers</span></span>
|<span data-ttu-id="d0ead-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d0ead-120">Header</span></span>|<span data-ttu-id="d0ead-121">値</span><span class="sxs-lookup"><span data-stu-id="d0ead-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d0ead-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d0ead-122">Authorization</span></span>|<span data-ttu-id="d0ead-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="d0ead-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d0ead-124">承諾</span><span class="sxs-lookup"><span data-stu-id="d0ead-124">Accept</span></span>|<span data-ttu-id="d0ead-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d0ead-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d0ead-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="d0ead-126">Request body</span></span>
<span data-ttu-id="d0ead-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="d0ead-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d0ead-128">応答</span><span class="sxs-lookup"><span data-stu-id="d0ead-128">Response</span></span>
<span data-ttu-id="d0ead-129">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[officeSuiteApp](../resources/intune-apps-officesuiteapp.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="d0ead-129">If successful, this method returns a `200 OK` response code and a collection of [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d0ead-130">例</span><span class="sxs-lookup"><span data-stu-id="d0ead-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="d0ead-131">要求</span><span class="sxs-lookup"><span data-stu-id="d0ead-131">Request</span></span>
<span data-ttu-id="d0ead-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d0ead-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="d0ead-133">応答</span><span class="sxs-lookup"><span data-stu-id="d0ead-133">Response</span></span>
<span data-ttu-id="d0ead-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d0ead-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1977

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.officeSuiteApp",
      "id": "9b263b46-3b46-9b26-463b-269b463b269b",
      "displayName": "Display Name value",
      "description": "Description value",
      "publisher": "Publisher value",
      "largeIcon": {
        "@odata.type": "microsoft.graph.mimeContent",
        "type": "Type value",
        "value": "dmFsdWU="
      },
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "isFeatured": true,
      "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
      "informationUrl": "https://example.com/informationUrl/",
      "owner": "Owner value",
      "developer": "Developer value",
      "notes": "Notes value",
      "uploadState": 11,
      "publishingState": "processing",
      "isAssigned": true,
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "autoAcceptEula": true,
      "productIds": [
        "o365BusinessRetail"
      ],
      "excludedApps": {
        "@odata.type": "microsoft.graph.excludedApps",
        "access": true,
        "excel": true,
        "groove": true,
        "infoPath": true,
        "lync": true,
        "oneDrive": true,
        "oneNote": true,
        "outlook": true,
        "powerPoint": true,
        "publisher": true,
        "sharePointDesigner": true,
        "visio": true,
        "word": true
      },
      "useSharedComputerActivation": true,
      "updateChannel": "current",
      "officePlatformArchitecture": "x86",
      "localesToInstall": [
        "Locales To Install value"
      ],
      "installProgressDisplayLevel": "full",
      "shouldUninstallOlderVersionsOfOffice": true,
      "targetVersion": "Target Version value",
      "updateVersion": "Update Version value",
      "officeConfigurationXml": "b2ZmaWNlQ29uZmlndXJhdGlvblhtbA=="
    }
  ]
}
```




