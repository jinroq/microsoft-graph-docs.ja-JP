---
title: リスト windowsPhoneEASEmailProfileConfigurations
description: WindowsPhoneEASEmailProfileConfiguration オブジェクトのプロパティと関係を一覧表示します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3f2d72610ecd66622f6a2973a6071d645913a040
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29392928"
---
# <a name="list-windowsphoneeasemailprofileconfigurations"></a><span data-ttu-id="2375a-103">リスト windowsPhoneEASEmailProfileConfigurations</span><span class="sxs-lookup"><span data-stu-id="2375a-103">List windowsPhoneEASEmailProfileConfigurations</span></span>

> <span data-ttu-id="2375a-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="2375a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="2375a-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2375a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2375a-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="2375a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2375a-107">[WindowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="2375a-107">List properties and relationships of the [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2375a-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="2375a-108">Prerequisites</span></span>
<span data-ttu-id="2375a-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2375a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="2375a-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2375a-111">Permission type</span></span>|<span data-ttu-id="2375a-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="2375a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2375a-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2375a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2375a-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="2375a-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="2375a-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2375a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2375a-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2375a-116">Not supported.</span></span>|
|<span data-ttu-id="2375a-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2375a-117">Application</span></span>|<span data-ttu-id="2375a-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2375a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2375a-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2375a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="2375a-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2375a-120">Request headers</span></span>
|<span data-ttu-id="2375a-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2375a-121">Header</span></span>|<span data-ttu-id="2375a-122">値</span><span class="sxs-lookup"><span data-stu-id="2375a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2375a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2375a-123">Authorization</span></span>|<span data-ttu-id="2375a-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="2375a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2375a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2375a-125">Accept</span></span>|<span data-ttu-id="2375a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2375a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2375a-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="2375a-127">Request body</span></span>
<span data-ttu-id="2375a-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="2375a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2375a-129">応答</span><span class="sxs-lookup"><span data-stu-id="2375a-129">Response</span></span>
<span data-ttu-id="2375a-130">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に[windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="2375a-130">If successful, this method returns a `200 OK` response code and a collection of [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2375a-131">例</span><span class="sxs-lookup"><span data-stu-id="2375a-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="2375a-132">要求</span><span class="sxs-lookup"><span data-stu-id="2375a-132">Request</span></span>
<span data-ttu-id="2375a-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2375a-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="2375a-134">応答</span><span class="sxs-lookup"><span data-stu-id="2375a-134">Response</span></span>
<span data-ttu-id="2375a-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="2375a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1099

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsPhoneEASEmailProfileConfiguration",
      "id": "554f402a-402a-554f-2a40-4f552a404f55",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "supportsScopeTags": true,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "usernameSource": "primarySmtpAddress",
      "usernameAADSource": "primarySmtpAddress",
      "userDomainNameSource": "netBiosDomainName",
      "customDomainName": "Custom Domain Name value",
      "accountName": "Account Name value",
      "applyOnlyToWindowsPhone81": true,
      "syncCalendar": true,
      "syncContacts": true,
      "syncTasks": true,
      "durationOfEmailToSync": "oneDay",
      "emailAddressSource": "primarySmtpAddress",
      "emailSyncSchedule": "asMessagesArrive",
      "hostName": "Host Name value",
      "requireSsl": true
    }
  ]
}
```




