---
title: リスト Androidforwork の各 Deviceconfigurん
description: Androidforwork の各オブジェクトのプロパティとリレーションシップをリストします。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b9cc54b6491661169d264a01a1a0a4f0dbcb4369
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36312139"
---
# <a name="list-androidforworkgeneraldeviceconfigurations"></a><span data-ttu-id="db230-103">リスト Androidforwork の各 Deviceconfigurん</span><span class="sxs-lookup"><span data-stu-id="db230-103">List androidForWorkGeneralDeviceConfigurations</span></span>

> <span data-ttu-id="db230-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="db230-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="db230-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="db230-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="db230-106">[Androidforwork](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md)の各オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="db230-106">List properties and relationships of the [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="db230-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="db230-107">Prerequisites</span></span>
<span data-ttu-id="db230-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="db230-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="db230-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="db230-110">Permission type</span></span>|<span data-ttu-id="db230-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="db230-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="db230-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="db230-112">Delegated (work or school account)</span></span>|<span data-ttu-id="db230-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="db230-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="db230-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="db230-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="db230-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="db230-115">Not supported.</span></span>|
|<span data-ttu-id="db230-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="db230-116">Application</span></span>|<span data-ttu-id="db230-117">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="db230-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="db230-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="db230-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="db230-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="db230-119">Request headers</span></span>
|<span data-ttu-id="db230-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="db230-120">Header</span></span>|<span data-ttu-id="db230-121">値</span><span class="sxs-lookup"><span data-stu-id="db230-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="db230-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="db230-122">Authorization</span></span>|<span data-ttu-id="db230-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="db230-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="db230-124">承諾</span><span class="sxs-lookup"><span data-stu-id="db230-124">Accept</span></span>|<span data-ttu-id="db230-125">application/json</span><span class="sxs-lookup"><span data-stu-id="db230-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="db230-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="db230-126">Request body</span></span>
<span data-ttu-id="db230-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="db230-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="db230-128">応答</span><span class="sxs-lookup"><span data-stu-id="db230-128">Response</span></span>
<span data-ttu-id="db230-129">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[Androidforwork](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md)の各オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="db230-129">If successful, this method returns a `200 OK` response code and a collection of [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="db230-130">例</span><span class="sxs-lookup"><span data-stu-id="db230-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="db230-131">要求</span><span class="sxs-lookup"><span data-stu-id="db230-131">Request</span></span>
<span data-ttu-id="db230-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="db230-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="db230-133">応答</span><span class="sxs-lookup"><span data-stu-id="db230-133">Response</span></span>
<span data-ttu-id="db230-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="db230-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3288

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidForWorkGeneralDeviceConfiguration",
      "id": "a931a366-a366-a931-66a3-31a966a331a9",
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
      "passwordBlockFingerprintUnlock": true,
      "passwordBlockTrustAgents": true,
      "passwordExpirationDays": 6,
      "passwordMinimumLength": 5,
      "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
      "passwordPreviousPasswordBlockCount": 2,
      "passwordSignInFailureCountBeforeFactoryReset": 12,
      "passwordRequiredType": "lowSecurityBiometric",
      "workProfileDataSharingType": "preventAny",
      "workProfileBlockNotificationsWhileDeviceLocked": true,
      "workProfileBlockAddingAccounts": true,
      "workProfileBluetoothEnableContactSharing": true,
      "workProfileBlockScreenCapture": true,
      "workProfileBlockCrossProfileCallerId": true,
      "workProfileBlockCamera": true,
      "workProfileBlockCrossProfileContactsSearch": true,
      "workProfileBlockCrossProfileCopyPaste": true,
      "workProfileDefaultAppPermissionPolicy": "prompt",
      "workProfilePasswordBlockFingerprintUnlock": true,
      "workProfilePasswordBlockTrustAgents": true,
      "workProfilePasswordExpirationDays": 1,
      "workProfilePasswordMinimumLength": 0,
      "workProfilePasswordMinNumericCharacters": 7,
      "workProfilePasswordMinNonLetterCharacters": 9,
      "workProfilePasswordMinLetterCharacters": 6,
      "workProfilePasswordMinLowerCaseCharacters": 9,
      "workProfilePasswordMinUpperCaseCharacters": 9,
      "workProfilePasswordMinSymbolCharacters": 6,
      "workProfilePasswordMinutesOfInactivityBeforeScreenTimeout": 9,
      "workProfilePasswordPreviousPasswordBlockCount": 13,
      "workProfilePasswordSignInFailureCountBeforeFactoryReset": 7,
      "workProfilePasswordRequiredType": "lowSecurityBiometric",
      "workProfileRequirePassword": true,
      "securityRequireVerifyApps": true,
      "vpnAlwaysOnPackageIdentifier": "Vpn Always On Package Identifier value",
      "vpnEnableAlwaysOnLockdownMode": true
    }
  ]
}
```






