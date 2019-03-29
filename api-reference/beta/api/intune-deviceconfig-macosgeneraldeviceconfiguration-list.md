---
title: macOSGeneralDeviceConfigurations のリスト
description: macOSGeneralDeviceConfiguration オブジェクトのプロパティとリレーションシップをリストします。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bb15598012be676ab567550acd008d3f70580784
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30973048"
---
# <a name="list-macosgeneraldeviceconfigurations"></a><span data-ttu-id="e90ba-103">macOSGeneralDeviceConfigurations のリスト</span><span class="sxs-lookup"><span data-stu-id="e90ba-103">List macOSGeneralDeviceConfigurations</span></span>

> <span data-ttu-id="e90ba-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e90ba-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e90ba-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e90ba-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e90ba-106">[macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="e90ba-106">List properties and relationships of the [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e90ba-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="e90ba-107">Prerequisites</span></span>
<span data-ttu-id="e90ba-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e90ba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e90ba-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e90ba-110">Permission type</span></span>|<span data-ttu-id="e90ba-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="e90ba-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e90ba-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e90ba-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e90ba-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e90ba-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="e90ba-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e90ba-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e90ba-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e90ba-115">Not supported.</span></span>|
|<span data-ttu-id="e90ba-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e90ba-116">Application</span></span>|<span data-ttu-id="e90ba-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e90ba-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e90ba-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e90ba-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="e90ba-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e90ba-119">Request headers</span></span>
|<span data-ttu-id="e90ba-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e90ba-120">Header</span></span>|<span data-ttu-id="e90ba-121">値</span><span class="sxs-lookup"><span data-stu-id="e90ba-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e90ba-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e90ba-122">Authorization</span></span>|<span data-ttu-id="e90ba-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="e90ba-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e90ba-124">承諾</span><span class="sxs-lookup"><span data-stu-id="e90ba-124">Accept</span></span>|<span data-ttu-id="e90ba-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e90ba-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e90ba-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="e90ba-126">Request body</span></span>
<span data-ttu-id="e90ba-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="e90ba-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e90ba-128">応答</span><span class="sxs-lookup"><span data-stu-id="e90ba-128">Response</span></span>
<span data-ttu-id="e90ba-129">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="e90ba-129">If successful, this method returns a `200 OK` response code and a collection of [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e90ba-130">例</span><span class="sxs-lookup"><span data-stu-id="e90ba-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="e90ba-131">要求</span><span class="sxs-lookup"><span data-stu-id="e90ba-131">Request</span></span>
<span data-ttu-id="e90ba-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e90ba-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="e90ba-133">応答</span><span class="sxs-lookup"><span data-stu-id="e90ba-133">Response</span></span>
<span data-ttu-id="e90ba-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e90ba-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2437

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.macOSGeneralDeviceConfiguration",
      "id": "dc356aee-6aee-dc35-ee6a-35dcee6a35dc",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "supportsScopeTags": true,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "compliantAppsList": [
        {
          "@odata.type": "microsoft.graph.appListItem",
          "name": "Name value",
          "publisher": "Publisher value",
          "appStoreUrl": "https://example.com/appStoreUrl/",
          "appId": "App Id value"
        }
      ],
      "compliantAppListType": "appsInListCompliant",
      "emailInDomainSuffixes": [
        "Email In Domain Suffixes value"
      ],
      "passwordBlockSimple": true,
      "passwordExpirationDays": 6,
      "passwordMinimumCharacterSetCount": 0,
      "passwordMinimumLength": 5,
      "passwordMinutesOfInactivityBeforeLock": 5,
      "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
      "passwordPreviousPasswordBlockCount": 2,
      "passwordRequiredType": "alphanumeric",
      "passwordRequired": true,
      "keychainBlockCloudSync": true,
      "airPrintBlocked": true,
      "airPrintForceTrustedTLS": true,
      "airPrintBlockiBeaconDiscovery": true,
      "safariBlockAutofill": true,
      "cameraBlocked": true,
      "iTunesBlockMusicService": true,
      "spotlightBlockInternetResults": true,
      "keyboardBlockDictation": true,
      "definitionLookupBlocked": true,
      "appleWatchBlockAutoUnlock": true,
      "iTunesBlockFileSharing": true,
      "iCloudBlockDocumentSync": true,
      "iCloudBlockMail": true,
      "iCloudBlockAddressBook": true,
      "iCloudBlockCalendar": true,
      "iCloudBlockReminders": true,
      "iCloudBlockBookmarks": true,
      "iCloudBlockNotes": true,
      "airDropBlocked": true,
      "passwordBlockModification": true,
      "passwordBlockFingerprintUnlock": true,
      "passwordBlockAutoFill": true,
      "passwordBlockProximityRequests": true,
      "passwordBlockAirDropSharing": true,
      "softwareUpdatesEnforcedDelayInDays": 2,
      "softwareUpdatesForceDelayed": true,
      "contentCachingBlocked": true
    }
  ]
}
```




