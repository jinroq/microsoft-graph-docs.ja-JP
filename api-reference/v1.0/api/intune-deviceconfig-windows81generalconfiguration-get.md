---
title: windows81GeneralConfiguration の取得
description: windows81GeneralConfiguration オブジェクトのプロパティとリレーションシップを読み取ります。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2dec869e420fbb7ab4eefa328760ec05f6ded14e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36020032"
---
# <a name="get-windows81generalconfiguration"></a><span data-ttu-id="9690a-103">windows81GeneralConfiguration の取得</span><span class="sxs-lookup"><span data-stu-id="9690a-103">Get windows81GeneralConfiguration</span></span>

> <span data-ttu-id="9690a-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="9690a-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9690a-105">[windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="9690a-105">Read properties and relationships of the [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9690a-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="9690a-106">Prerequisites</span></span>
<span data-ttu-id="9690a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9690a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9690a-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9690a-109">Permission type</span></span>|<span data-ttu-id="9690a-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="9690a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9690a-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9690a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9690a-112">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="9690a-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="9690a-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9690a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9690a-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9690a-114">Not supported.</span></span>|
|<span data-ttu-id="9690a-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9690a-115">Application</span></span>|<span data-ttu-id="9690a-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9690a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9690a-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9690a-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9690a-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="9690a-118">Optional query parameters</span></span>
<span data-ttu-id="9690a-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="9690a-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9690a-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9690a-120">Request headers</span></span>
|<span data-ttu-id="9690a-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9690a-121">Header</span></span>|<span data-ttu-id="9690a-122">値</span><span class="sxs-lookup"><span data-stu-id="9690a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9690a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9690a-123">Authorization</span></span>|<span data-ttu-id="9690a-124">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="9690a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9690a-125">承諾</span><span class="sxs-lookup"><span data-stu-id="9690a-125">Accept</span></span>|<span data-ttu-id="9690a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9690a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9690a-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="9690a-127">Request body</span></span>
<span data-ttu-id="9690a-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="9690a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9690a-129">応答</span><span class="sxs-lookup"><span data-stu-id="9690a-129">Response</span></span>
<span data-ttu-id="9690a-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="9690a-130">If successful, this method returns a `200 OK` response code and [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9690a-131">例</span><span class="sxs-lookup"><span data-stu-id="9690a-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="9690a-132">要求</span><span class="sxs-lookup"><span data-stu-id="9690a-132">Request</span></span>
<span data-ttu-id="9690a-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="9690a-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="9690a-134">応答</span><span class="sxs-lookup"><span data-stu-id="9690a-134">Response</span></span>
<span data-ttu-id="9690a-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="9690a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1964

{
  "value": {
    "@odata.type": "#microsoft.graph.windows81GeneralConfiguration",
    "id": "0e9285b5-85b5-0e92-b585-920eb585920e",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "accountsBlockAddingNonMicrosoftAccountEmail": true,
    "applyOnlyToWindows81": true,
    "browserBlockAutofill": true,
    "browserBlockAutomaticDetectionOfIntranetSites": true,
    "browserBlockEnterpriseModeAccess": true,
    "browserBlockJavaScript": true,
    "browserBlockPlugins": true,
    "browserBlockPopups": true,
    "browserBlockSendingDoNotTrackHeader": true,
    "browserBlockSingleWordEntryOnIntranetSites": true,
    "browserRequireSmartScreen": true,
    "browserEnterpriseModeSiteListLocation": "Browser Enterprise Mode Site List Location value",
    "browserInternetSecurityLevel": "medium",
    "browserIntranetSecurityLevel": "low",
    "browserLoggingReportLocation": "Browser Logging Report Location value",
    "browserRequireHighSecurityForRestrictedSites": true,
    "browserRequireFirewall": true,
    "browserRequireFraudWarning": true,
    "browserTrustedSitesSecurityLevel": "low",
    "cellularBlockDataRoaming": true,
    "diagnosticsBlockDataSubmission": true,
    "passwordBlockPicturePasswordAndPin": true,
    "passwordExpirationDays": 6,
    "passwordMinimumLength": 5,
    "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
    "passwordMinimumCharacterSetCount": 0,
    "passwordPreviousPasswordBlockCount": 2,
    "passwordRequiredType": "alphanumeric",
    "passwordSignInFailureCountBeforeFactoryReset": 12,
    "storageRequireDeviceEncryption": true,
    "updatesRequireAutomaticUpdates": true,
    "userAccountControlSettings": "alwaysNotify",
    "workFoldersUrl": "https://example.com/workFoldersUrl/"
  }
}
```



