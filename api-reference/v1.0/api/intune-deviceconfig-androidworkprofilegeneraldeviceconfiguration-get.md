---
title: androidwork profileの devic/デバイスを取得する
description: androidwork profile一般の devic/オブジェクトのプロパティとリレーションシップを読み取ります。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fbebbbc28efb46d370aff602565077ce6973ea65
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30971592"
---
# <a name="get-androidworkprofilegeneraldeviceconfiguration"></a><span data-ttu-id="de559-103">androidwork profileの devic/デバイスを取得する</span><span class="sxs-lookup"><span data-stu-id="de559-103">Get androidWorkProfileGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="de559-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="de559-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="de559-105">[androidwork profile一般](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md)の devic/オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="de559-105">Read properties and relationships of the [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="de559-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="de559-106">Prerequisites</span></span>
<span data-ttu-id="de559-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="de559-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="de559-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="de559-109">Permission type</span></span>|<span data-ttu-id="de559-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="de559-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="de559-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="de559-111">Delegated (work or school account)</span></span>|<span data-ttu-id="de559-112">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="de559-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="de559-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="de559-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="de559-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="de559-114">Not supported.</span></span>|
|<span data-ttu-id="de559-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="de559-115">Application</span></span>|<span data-ttu-id="de559-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="de559-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="de559-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="de559-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="de559-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="de559-118">Optional query parameters</span></span>
<span data-ttu-id="de559-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="de559-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="de559-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="de559-120">Request headers</span></span>
|<span data-ttu-id="de559-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="de559-121">Header</span></span>|<span data-ttu-id="de559-122">値</span><span class="sxs-lookup"><span data-stu-id="de559-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="de559-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="de559-123">Authorization</span></span>|<span data-ttu-id="de559-124">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="de559-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="de559-125">承諾</span><span class="sxs-lookup"><span data-stu-id="de559-125">Accept</span></span>|<span data-ttu-id="de559-126">application/json</span><span class="sxs-lookup"><span data-stu-id="de559-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="de559-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="de559-127">Request body</span></span>
<span data-ttu-id="de559-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="de559-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="de559-129">応答</span><span class="sxs-lookup"><span data-stu-id="de559-129">Response</span></span>
<span data-ttu-id="de559-130">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[androidwork profileprofiledevicオブジェクト](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md)を返します。</span><span class="sxs-lookup"><span data-stu-id="de559-130">If successful, this method returns a `200 OK` response code and [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="de559-131">例</span><span class="sxs-lookup"><span data-stu-id="de559-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="de559-132">要求</span><span class="sxs-lookup"><span data-stu-id="de559-132">Request</span></span>
<span data-ttu-id="de559-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="de559-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="de559-134">応答</span><span class="sxs-lookup"><span data-stu-id="de559-134">Response</span></span>
<span data-ttu-id="de559-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="de559-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2104

{
  "value": {
    "@odata.type": "#microsoft.graph.androidWorkProfileGeneralDeviceConfiguration",
    "id": "6decda7e-da7e-6dec-7eda-ec6d7edaec6d",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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
    "securityRequireVerifyApps": true
  }
}
```



