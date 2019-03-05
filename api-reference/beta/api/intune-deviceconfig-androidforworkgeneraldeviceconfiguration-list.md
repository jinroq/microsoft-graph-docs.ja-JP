---
title: リスト androidforwork の各 deviceconfigurん
description: androidforwork の各オブジェクトのプロパティとリレーションシップをリストします。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 734a788905bcb910093fb8ac7ff96580d14588cd
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30143394"
---
# <a name="list-androidforworkgeneraldeviceconfigurations"></a><span data-ttu-id="8a1ce-103">リスト androidforwork の各 deviceconfigurん</span><span class="sxs-lookup"><span data-stu-id="8a1ce-103">List androidForWorkGeneralDeviceConfigurations</span></span>

> <span data-ttu-id="8a1ce-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8a1ce-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8a1ce-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="8a1ce-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8a1ce-106">[androidforwork](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md)の各オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="8a1ce-106">List properties and relationships of the [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8a1ce-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="8a1ce-107">Prerequisites</span></span>
<span data-ttu-id="8a1ce-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8a1ce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="8a1ce-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8a1ce-110">Permission type</span></span>|<span data-ttu-id="8a1ce-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="8a1ce-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8a1ce-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8a1ce-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8a1ce-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="8a1ce-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="8a1ce-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8a1ce-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8a1ce-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8a1ce-115">Not supported.</span></span>|
|<span data-ttu-id="8a1ce-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8a1ce-116">Application</span></span>|<span data-ttu-id="8a1ce-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8a1ce-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8a1ce-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8a1ce-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="8a1ce-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8a1ce-119">Request headers</span></span>
|<span data-ttu-id="8a1ce-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8a1ce-120">Header</span></span>|<span data-ttu-id="8a1ce-121">値</span><span class="sxs-lookup"><span data-stu-id="8a1ce-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8a1ce-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8a1ce-122">Authorization</span></span>|<span data-ttu-id="8a1ce-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="8a1ce-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8a1ce-124">承諾</span><span class="sxs-lookup"><span data-stu-id="8a1ce-124">Accept</span></span>|<span data-ttu-id="8a1ce-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8a1ce-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8a1ce-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="8a1ce-126">Request body</span></span>
<span data-ttu-id="8a1ce-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="8a1ce-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8a1ce-128">応答</span><span class="sxs-lookup"><span data-stu-id="8a1ce-128">Response</span></span>
<span data-ttu-id="8a1ce-129">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[androidforwork](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md)の各オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="8a1ce-129">If successful, this method returns a `200 OK` response code and a collection of [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8a1ce-130">例</span><span class="sxs-lookup"><span data-stu-id="8a1ce-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="8a1ce-131">要求</span><span class="sxs-lookup"><span data-stu-id="8a1ce-131">Request</span></span>
<span data-ttu-id="8a1ce-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8a1ce-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="8a1ce-133">応答</span><span class="sxs-lookup"><span data-stu-id="8a1ce-133">Response</span></span>
<span data-ttu-id="8a1ce-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8a1ce-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2431

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




