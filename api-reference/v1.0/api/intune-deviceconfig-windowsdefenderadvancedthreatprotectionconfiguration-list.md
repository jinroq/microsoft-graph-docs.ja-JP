---
title: windowsDefenderAdvancedThreatProtectionConfigurations のリスト
description: windowsDefenderAdvancedThreatProtectionConfiguration オブジェクトのプロパティとリレーションシップをリストします。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d4e23f07281ac689811359b773acfdc395335b03
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30984430"
---
# <a name="list-windowsdefenderadvancedthreatprotectionconfigurations"></a><span data-ttu-id="f1c79-103">windowsDefenderAdvancedThreatProtectionConfigurations のリスト</span><span class="sxs-lookup"><span data-stu-id="f1c79-103">List windowsDefenderAdvancedThreatProtectionConfigurations</span></span>

> <span data-ttu-id="f1c79-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f1c79-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f1c79-105">[windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="f1c79-105">List properties and relationships of the [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f1c79-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="f1c79-106">Prerequisites</span></span>
<span data-ttu-id="f1c79-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f1c79-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f1c79-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f1c79-109">Permission type</span></span>|<span data-ttu-id="f1c79-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="f1c79-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f1c79-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f1c79-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f1c79-112">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f1c79-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="f1c79-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f1c79-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f1c79-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f1c79-114">Not supported.</span></span>|
|<span data-ttu-id="f1c79-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f1c79-115">Application</span></span>|<span data-ttu-id="f1c79-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f1c79-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f1c79-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f1c79-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="f1c79-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f1c79-118">Request headers</span></span>
|<span data-ttu-id="f1c79-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f1c79-119">Header</span></span>|<span data-ttu-id="f1c79-120">値</span><span class="sxs-lookup"><span data-stu-id="f1c79-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f1c79-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f1c79-121">Authorization</span></span>|<span data-ttu-id="f1c79-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="f1c79-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f1c79-123">承諾</span><span class="sxs-lookup"><span data-stu-id="f1c79-123">Accept</span></span>|<span data-ttu-id="f1c79-124">application/json</span><span class="sxs-lookup"><span data-stu-id="f1c79-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f1c79-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="f1c79-125">Request body</span></span>
<span data-ttu-id="f1c79-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="f1c79-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f1c79-127">応答</span><span class="sxs-lookup"><span data-stu-id="f1c79-127">Response</span></span>
<span data-ttu-id="f1c79-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="f1c79-128">If successful, this method returns a `200 OK` response code and a collection of [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f1c79-129">例</span><span class="sxs-lookup"><span data-stu-id="f1c79-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="f1c79-130">要求</span><span class="sxs-lookup"><span data-stu-id="f1c79-130">Request</span></span>
<span data-ttu-id="f1c79-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f1c79-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="f1c79-132">応答</span><span class="sxs-lookup"><span data-stu-id="f1c79-132">Response</span></span>
<span data-ttu-id="f1c79-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f1c79-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



