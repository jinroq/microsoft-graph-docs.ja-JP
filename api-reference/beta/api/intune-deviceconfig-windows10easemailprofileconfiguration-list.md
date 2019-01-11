---
title: リスト windows10EasEmailProfileConfigurations
description: Windows10EasEmailProfileConfiguration オブジェクトのプロパティと関係を一覧表示します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 4afcc59bda7749655458a2906f292d34fe1c5932
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27842351"
---
# <a name="list-windows10easemailprofileconfigurations"></a><span data-ttu-id="afeea-103">リスト windows10EasEmailProfileConfigurations</span><span class="sxs-lookup"><span data-stu-id="afeea-103">List windows10EasEmailProfileConfigurations</span></span>

> <span data-ttu-id="afeea-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="afeea-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="afeea-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="afeea-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="afeea-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="afeea-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="afeea-107">[Windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="afeea-107">List properties and relationships of the [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="afeea-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="afeea-108">Prerequisites</span></span>
<span data-ttu-id="afeea-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="afeea-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="afeea-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="afeea-111">Permission type</span></span>|<span data-ttu-id="afeea-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="afeea-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="afeea-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="afeea-113">Delegated (work or school account)</span></span>|<span data-ttu-id="afeea-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="afeea-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="afeea-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="afeea-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="afeea-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="afeea-116">Not supported.</span></span>|
|<span data-ttu-id="afeea-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="afeea-117">Application</span></span>|<span data-ttu-id="afeea-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="afeea-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="afeea-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="afeea-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="afeea-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="afeea-120">Request headers</span></span>
|<span data-ttu-id="afeea-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="afeea-121">Header</span></span>|<span data-ttu-id="afeea-122">値</span><span class="sxs-lookup"><span data-stu-id="afeea-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="afeea-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="afeea-123">Authorization</span></span>|<span data-ttu-id="afeea-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="afeea-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="afeea-125">Accept</span><span class="sxs-lookup"><span data-stu-id="afeea-125">Accept</span></span>|<span data-ttu-id="afeea-126">application/json</span><span class="sxs-lookup"><span data-stu-id="afeea-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="afeea-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="afeea-127">Request body</span></span>
<span data-ttu-id="afeea-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="afeea-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="afeea-129">応答</span><span class="sxs-lookup"><span data-stu-id="afeea-129">Response</span></span>
<span data-ttu-id="afeea-130">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に[windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="afeea-130">If successful, this method returns a `200 OK` response code and a collection of [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="afeea-131">例</span><span class="sxs-lookup"><span data-stu-id="afeea-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="afeea-132">要求</span><span class="sxs-lookup"><span data-stu-id="afeea-132">Request</span></span>
<span data-ttu-id="afeea-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="afeea-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="afeea-134">応答</span><span class="sxs-lookup"><span data-stu-id="afeea-134">Response</span></span>
<span data-ttu-id="afeea-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="afeea-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1054

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windows10EasEmailProfileConfiguration",
      "id": "9dc6f073-f073-9dc6-73f0-c69d73f0c69d",
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





