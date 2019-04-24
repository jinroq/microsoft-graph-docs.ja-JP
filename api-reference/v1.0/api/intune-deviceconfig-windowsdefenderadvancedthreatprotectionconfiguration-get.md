---
title: windowsDefenderAdvancedThreatProtectionConfiguration の取得
description: windowsDefenderAdvancedThreatProtectionConfiguration オブジェクトのプロパティとリレーションシップを読み取ります。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 37b03894bd9ec8607d0bc8651a1282867d2685af
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32585013"
---
# <a name="get-windowsdefenderadvancedthreatprotectionconfiguration"></a><span data-ttu-id="f38b7-103">windowsDefenderAdvancedThreatProtectionConfiguration の取得</span><span class="sxs-lookup"><span data-stu-id="f38b7-103">Get windowsDefenderAdvancedThreatProtectionConfiguration</span></span>

> <span data-ttu-id="f38b7-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f38b7-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f38b7-105">[windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="f38b7-105">Read properties and relationships of the [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f38b7-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="f38b7-106">Prerequisites</span></span>
<span data-ttu-id="f38b7-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f38b7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f38b7-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f38b7-109">Permission type</span></span>|<span data-ttu-id="f38b7-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="f38b7-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f38b7-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f38b7-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f38b7-112">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f38b7-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="f38b7-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f38b7-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f38b7-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f38b7-114">Not supported.</span></span>|
|<span data-ttu-id="f38b7-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f38b7-115">Application</span></span>|<span data-ttu-id="f38b7-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f38b7-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f38b7-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f38b7-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f38b7-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="f38b7-118">Optional query parameters</span></span>
<span data-ttu-id="f38b7-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="f38b7-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f38b7-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f38b7-120">Request headers</span></span>
|<span data-ttu-id="f38b7-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f38b7-121">Header</span></span>|<span data-ttu-id="f38b7-122">値</span><span class="sxs-lookup"><span data-stu-id="f38b7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f38b7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f38b7-123">Authorization</span></span>|<span data-ttu-id="f38b7-124">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="f38b7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f38b7-125">承諾</span><span class="sxs-lookup"><span data-stu-id="f38b7-125">Accept</span></span>|<span data-ttu-id="f38b7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f38b7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f38b7-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="f38b7-127">Request body</span></span>
<span data-ttu-id="f38b7-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="f38b7-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f38b7-129">応答</span><span class="sxs-lookup"><span data-stu-id="f38b7-129">Response</span></span>
<span data-ttu-id="f38b7-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f38b7-130">If successful, this method returns a `200 OK` response code and [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f38b7-131">例</span><span class="sxs-lookup"><span data-stu-id="f38b7-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="f38b7-132">要求</span><span class="sxs-lookup"><span data-stu-id="f38b7-132">Request</span></span>
<span data-ttu-id="f38b7-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f38b7-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="f38b7-134">応答</span><span class="sxs-lookup"><span data-stu-id="f38b7-134">Response</span></span>
<span data-ttu-id="f38b7-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f38b7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 476

{
  "value": {
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
}
```



