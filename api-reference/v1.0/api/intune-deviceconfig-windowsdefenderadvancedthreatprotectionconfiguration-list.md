---
title: windowsDefenderAdvancedThreatProtectionConfigurations のリスト
description: windowsDefenderAdvancedThreatProtectionConfiguration オブジェクトのプロパティとリレーションシップをリストします。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: d8a9b6461431281db63b93017748d6b7b2c6bd27
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826412"
---
# <a name="list-windowsdefenderadvancedthreatprotectionconfigurations"></a><span data-ttu-id="eeb38-103">windowsDefenderAdvancedThreatProtectionConfigurations のリスト</span><span class="sxs-lookup"><span data-stu-id="eeb38-103">List windowsDefenderAdvancedThreatProtectionConfigurations</span></span>

> <span data-ttu-id="eeb38-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="eeb38-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="eeb38-105">[windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="eeb38-105">List properties and relationships of the [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="eeb38-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="eeb38-106">Prerequisites</span></span>
<span data-ttu-id="eeb38-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="eeb38-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eeb38-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="eeb38-109">Permission type</span></span>|<span data-ttu-id="eeb38-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="eeb38-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eeb38-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="eeb38-111">Delegated (work or school account)</span></span>|<span data-ttu-id="eeb38-112">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="eeb38-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="eeb38-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="eeb38-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eeb38-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="eeb38-114">Not supported.</span></span>|
|<span data-ttu-id="eeb38-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="eeb38-115">Application</span></span>|<span data-ttu-id="eeb38-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="eeb38-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="eeb38-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="eeb38-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="eeb38-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="eeb38-118">Request headers</span></span>
|<span data-ttu-id="eeb38-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="eeb38-119">Header</span></span>|<span data-ttu-id="eeb38-120">値</span><span class="sxs-lookup"><span data-stu-id="eeb38-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eeb38-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="eeb38-121">Authorization</span></span>|<span data-ttu-id="eeb38-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="eeb38-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eeb38-123">Accept</span><span class="sxs-lookup"><span data-stu-id="eeb38-123">Accept</span></span>|<span data-ttu-id="eeb38-124">application/json</span><span class="sxs-lookup"><span data-stu-id="eeb38-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eeb38-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="eeb38-125">Request body</span></span>
<span data-ttu-id="eeb38-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="eeb38-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eeb38-127">応答</span><span class="sxs-lookup"><span data-stu-id="eeb38-127">Response</span></span>
<span data-ttu-id="eeb38-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="eeb38-128">If successful, this method returns a `200 OK` response code and a collection of [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eeb38-129">例</span><span class="sxs-lookup"><span data-stu-id="eeb38-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="eeb38-130">要求</span><span class="sxs-lookup"><span data-stu-id="eeb38-130">Request</span></span>
<span data-ttu-id="eeb38-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="eeb38-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="eeb38-132">応答</span><span class="sxs-lookup"><span data-stu-id="eeb38-132">Response</span></span>
<span data-ttu-id="eeb38-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="eeb38-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 508

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsDefenderAdvancedThreatProtectionConfiguration",
      "id": "294373aa-73aa-2943-aa73-4329aa734329",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "allowSampleSharing": true,
      "enableExpeditedTelemetryReporting": true
    }
  ]
}
```



