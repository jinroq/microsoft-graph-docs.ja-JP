---
title: macOSGeneralDeviceConfigurations のリスト
description: macOSGeneralDeviceConfiguration オブジェクトのプロパティとリレーションシップをリストします。
author: tfitzmac
ms.openlocfilehash: c9523d10de17845642925cc30e59ca86b26008a6
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27301807"
---
# <a name="list-macosgeneraldeviceconfigurations"></a><span data-ttu-id="521e6-103">macOSGeneralDeviceConfigurations のリスト</span><span class="sxs-lookup"><span data-stu-id="521e6-103">List macOSGeneralDeviceConfigurations</span></span>

> <span data-ttu-id="521e6-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="521e6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="521e6-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="521e6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="521e6-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="521e6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="521e6-107">[macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="521e6-107">List properties and relationships of the [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="521e6-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="521e6-108">Prerequisites</span></span>
<span data-ttu-id="521e6-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="521e6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="521e6-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="521e6-111">Permission type</span></span>|<span data-ttu-id="521e6-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="521e6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="521e6-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="521e6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="521e6-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="521e6-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="521e6-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="521e6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="521e6-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="521e6-116">Not supported.</span></span>|
|<span data-ttu-id="521e6-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="521e6-117">Application</span></span>|<span data-ttu-id="521e6-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="521e6-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="521e6-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="521e6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="521e6-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="521e6-120">Request headers</span></span>
|<span data-ttu-id="521e6-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="521e6-121">Header</span></span>|<span data-ttu-id="521e6-122">値</span><span class="sxs-lookup"><span data-stu-id="521e6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="521e6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="521e6-123">Authorization</span></span>|<span data-ttu-id="521e6-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="521e6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="521e6-125">Accept</span><span class="sxs-lookup"><span data-stu-id="521e6-125">Accept</span></span>|<span data-ttu-id="521e6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="521e6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="521e6-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="521e6-127">Request body</span></span>
<span data-ttu-id="521e6-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="521e6-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="521e6-129">応答</span><span class="sxs-lookup"><span data-stu-id="521e6-129">Response</span></span>
<span data-ttu-id="521e6-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="521e6-130">If successful, this method returns a `200 OK` response code and a collection of [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="521e6-131">例</span><span class="sxs-lookup"><span data-stu-id="521e6-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="521e6-132">要求</span><span class="sxs-lookup"><span data-stu-id="521e6-132">Request</span></span>
<span data-ttu-id="521e6-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="521e6-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="521e6-134">応答</span><span class="sxs-lookup"><span data-stu-id="521e6-134">Response</span></span>
<span data-ttu-id="521e6-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="521e6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2178

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
      "passwordBlockFingerprintUnlock": true
    }
  ]
}
```




