---
title: windows81GeneralConfigurations のリスト
description: windows81GeneralConfiguration オブジェクトのプロパティとリレーションシップをリストします。
ms.openlocfilehash: 259f47dd6317abf9a0e57fa19d28f284d190536e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27020545"
---
# <a name="list-windows81generalconfigurations"></a><span data-ttu-id="0a8ea-103">windows81GeneralConfigurations のリスト</span><span class="sxs-lookup"><span data-stu-id="0a8ea-103">List windows81GeneralConfigurations</span></span>

> <span data-ttu-id="0a8ea-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="0a8ea-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0a8ea-105">[windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="0a8ea-105">List properties and relationships of the [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0a8ea-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="0a8ea-106">Prerequisites</span></span>
<span data-ttu-id="0a8ea-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0a8ea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0a8ea-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0a8ea-109">Permission type</span></span>|<span data-ttu-id="0a8ea-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="0a8ea-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0a8ea-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0a8ea-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0a8ea-112">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="0a8ea-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="0a8ea-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0a8ea-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0a8ea-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0a8ea-114">Not supported.</span></span>|
|<span data-ttu-id="0a8ea-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0a8ea-115">Application</span></span>|<span data-ttu-id="0a8ea-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0a8ea-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0a8ea-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0a8ea-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="0a8ea-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0a8ea-118">Request headers</span></span>
|<span data-ttu-id="0a8ea-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0a8ea-119">Header</span></span>|<span data-ttu-id="0a8ea-120">値</span><span class="sxs-lookup"><span data-stu-id="0a8ea-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0a8ea-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="0a8ea-121">Authorization</span></span>|<span data-ttu-id="0a8ea-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="0a8ea-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0a8ea-123">Accept</span><span class="sxs-lookup"><span data-stu-id="0a8ea-123">Accept</span></span>|<span data-ttu-id="0a8ea-124">application/json</span><span class="sxs-lookup"><span data-stu-id="0a8ea-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0a8ea-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="0a8ea-125">Request body</span></span>
<span data-ttu-id="0a8ea-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="0a8ea-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0a8ea-127">応答</span><span class="sxs-lookup"><span data-stu-id="0a8ea-127">Response</span></span>
<span data-ttu-id="0a8ea-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="0a8ea-128">If successful, this method returns a `200 OK` response code and a collection of [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0a8ea-129">例</span><span class="sxs-lookup"><span data-stu-id="0a8ea-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="0a8ea-130">要求</span><span class="sxs-lookup"><span data-stu-id="0a8ea-130">Request</span></span>
<span data-ttu-id="0a8ea-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0a8ea-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="0a8ea-132">応答</span><span class="sxs-lookup"><span data-stu-id="0a8ea-132">Response</span></span>
<span data-ttu-id="0a8ea-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0a8ea-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2058

{
  "value": [
    {
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
  ]
}
```



