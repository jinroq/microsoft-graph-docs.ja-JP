---
title: windows81GeneralConfigurations のリスト
description: windows81GeneralConfiguration オブジェクトのプロパティとリレーションシップをリストします。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8de52c48f773259bca1c959bc1b221ba5537cc4d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425422"
---
# <a name="list-windows81generalconfigurations"></a><span data-ttu-id="bebaf-103">windows81GeneralConfigurations のリスト</span><span class="sxs-lookup"><span data-stu-id="bebaf-103">List windows81GeneralConfigurations</span></span>

> <span data-ttu-id="bebaf-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="bebaf-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="bebaf-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bebaf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bebaf-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="bebaf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bebaf-107">[windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="bebaf-107">List properties and relationships of the [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bebaf-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="bebaf-108">Prerequisites</span></span>
<span data-ttu-id="bebaf-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bebaf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="bebaf-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="bebaf-111">Permission type</span></span>|<span data-ttu-id="bebaf-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="bebaf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bebaf-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="bebaf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bebaf-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="bebaf-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="bebaf-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="bebaf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bebaf-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bebaf-116">Not supported.</span></span>|
|<span data-ttu-id="bebaf-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="bebaf-117">Application</span></span>|<span data-ttu-id="bebaf-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bebaf-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bebaf-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="bebaf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="bebaf-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bebaf-120">Request headers</span></span>
|<span data-ttu-id="bebaf-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bebaf-121">Header</span></span>|<span data-ttu-id="bebaf-122">値</span><span class="sxs-lookup"><span data-stu-id="bebaf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bebaf-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bebaf-123">Authorization</span></span>|<span data-ttu-id="bebaf-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="bebaf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bebaf-125">Accept</span><span class="sxs-lookup"><span data-stu-id="bebaf-125">Accept</span></span>|<span data-ttu-id="bebaf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bebaf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bebaf-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="bebaf-127">Request body</span></span>
<span data-ttu-id="bebaf-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="bebaf-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bebaf-129">応答</span><span class="sxs-lookup"><span data-stu-id="bebaf-129">Response</span></span>
<span data-ttu-id="bebaf-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="bebaf-130">If successful, this method returns a `200 OK` response code and a collection of [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bebaf-131">例</span><span class="sxs-lookup"><span data-stu-id="bebaf-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="bebaf-132">要求</span><span class="sxs-lookup"><span data-stu-id="bebaf-132">Request</span></span>
<span data-ttu-id="bebaf-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="bebaf-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="bebaf-134">応答</span><span class="sxs-lookup"><span data-stu-id="bebaf-134">Response</span></span>
<span data-ttu-id="bebaf-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="bebaf-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2313

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windows81GeneralConfiguration",
      "id": "0e9285b5-85b5-0e92-b585-920eb585920e",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "supportsScopeTags": true,
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
      "minimumAutoInstallClassification": "recommendedAndImportant",
      "updatesMinimumAutoInstallClassification": "recommendedAndImportant",
      "updatesRequireAutomaticUpdates": true,
      "userAccountControlSettings": "alwaysNotify",
      "workFoldersUrl": "https://example.com/workFoldersUrl/"
    }
  ]
}
```




