---
title: AndroidEasEmailProfileConfiguration の取得
description: Androide Asemailprofil/オブジェクトのプロパティとリレーションシップを読み取ります。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e8e2335262f948c7e4657fc960a3fef1dd688b62
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33933096"
---
# <a name="get-androideasemailprofileconfiguration"></a><span data-ttu-id="8d3d8-103">AndroidEasEmailProfileConfiguration の取得</span><span class="sxs-lookup"><span data-stu-id="8d3d8-103">Get androidEasEmailProfileConfiguration</span></span>

> <span data-ttu-id="8d3d8-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8d3d8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8d3d8-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="8d3d8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8d3d8-106">[Androide Asemailprofil/](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="8d3d8-106">Read properties and relationships of the [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8d3d8-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="8d3d8-107">Prerequisites</span></span>
<span data-ttu-id="8d3d8-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8d3d8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8d3d8-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8d3d8-110">Permission type</span></span>|<span data-ttu-id="8d3d8-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="8d3d8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8d3d8-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8d3d8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8d3d8-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="8d3d8-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="8d3d8-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8d3d8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8d3d8-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8d3d8-115">Not supported.</span></span>|
|<span data-ttu-id="8d3d8-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8d3d8-116">Application</span></span>|<span data-ttu-id="8d3d8-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8d3d8-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8d3d8-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8d3d8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8d3d8-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="8d3d8-119">Optional query parameters</span></span>
<span data-ttu-id="8d3d8-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="8d3d8-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8d3d8-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8d3d8-121">Request headers</span></span>
|<span data-ttu-id="8d3d8-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8d3d8-122">Header</span></span>|<span data-ttu-id="8d3d8-123">値</span><span class="sxs-lookup"><span data-stu-id="8d3d8-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8d3d8-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="8d3d8-124">Authorization</span></span>|<span data-ttu-id="8d3d8-125">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="8d3d8-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8d3d8-126">承諾</span><span class="sxs-lookup"><span data-stu-id="8d3d8-126">Accept</span></span>|<span data-ttu-id="8d3d8-127">application/json</span><span class="sxs-lookup"><span data-stu-id="8d3d8-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8d3d8-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="8d3d8-128">Request body</span></span>
<span data-ttu-id="8d3d8-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="8d3d8-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8d3d8-130">応答</span><span class="sxs-lookup"><span data-stu-id="8d3d8-130">Response</span></span>
<span data-ttu-id="8d3d8-131">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[Androide asemailprofil/](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md)のオブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="8d3d8-131">If successful, this method returns a `200 OK` response code and [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8d3d8-132">例</span><span class="sxs-lookup"><span data-stu-id="8d3d8-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="8d3d8-133">要求</span><span class="sxs-lookup"><span data-stu-id="8d3d8-133">Request</span></span>
<span data-ttu-id="8d3d8-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8d3d8-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="8d3d8-135">応答</span><span class="sxs-lookup"><span data-stu-id="8d3d8-135">Response</span></span>
<span data-ttu-id="8d3d8-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8d3d8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1036

{
  "value": {
    "@odata.type": "#microsoft.graph.androidEasEmailProfileConfiguration",
    "id": "ee5e5610-5610-ee5e-1056-5eee10565eee",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "supportsScopeTags": true,
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "accountName": "Account Name value",
    "authenticationMethod": "certificate",
    "syncCalendar": true,
    "syncContacts": true,
    "syncTasks": true,
    "syncNotes": true,
    "durationOfEmailToSync": "oneDay",
    "emailAddressSource": "primarySmtpAddress",
    "emailSyncSchedule": "asMessagesArrive",
    "hostName": "Host Name value",
    "requireSmime": true,
    "requireSsl": true,
    "usernameSource": "userPrincipalName",
    "userDomainNameSource": "netBiosDomainName",
    "customDomainName": "Custom Domain Name value"
  }
}
```




