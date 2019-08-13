---
title: DeviceManagementComplexSettingInstances を一覧表示する
description: DeviceManagementComplexSettingInstance オブジェクトのプロパティとリレーションシップをリストします。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6d176b09ee14868a9ba64a43273e3c867e15a8d9
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36343784"
---
# <a name="list-devicemanagementcomplexsettinginstances"></a><span data-ttu-id="d3a97-103">DeviceManagementComplexSettingInstances を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="d3a97-103">List deviceManagementComplexSettingInstances</span></span>

> <span data-ttu-id="d3a97-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d3a97-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d3a97-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d3a97-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d3a97-106">[Devicemanagementcomplexsettinginstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="d3a97-106">List properties and relationships of the [deviceManagementComplexSettingInstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d3a97-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="d3a97-107">Prerequisites</span></span>
<span data-ttu-id="d3a97-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d3a97-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d3a97-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d3a97-110">Permission type</span></span>|<span data-ttu-id="d3a97-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="d3a97-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d3a97-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d3a97-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d3a97-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d3a97-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="d3a97-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d3a97-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d3a97-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d3a97-115">Not supported.</span></span>|
|<span data-ttu-id="d3a97-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d3a97-116">Application</span></span>|<span data-ttu-id="d3a97-117">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d3a97-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d3a97-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d3a97-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/intents/{deviceManagementIntentId}/settings
GET /deviceManagement/templates/{deviceManagementTemplateId}/settings
GET /deviceManagement/intents/{deviceManagementIntentId}/categories/{deviceManagementIntentSettingCategoryId}/settings
GET /deviceManagement/templates/{deviceManagementTemplateId}/categories/{deviceManagementTemplateSettingCategoryId}/recommendedSettings
```

## <a name="request-headers"></a><span data-ttu-id="d3a97-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d3a97-119">Request headers</span></span>
|<span data-ttu-id="d3a97-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d3a97-120">Header</span></span>|<span data-ttu-id="d3a97-121">値</span><span class="sxs-lookup"><span data-stu-id="d3a97-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d3a97-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d3a97-122">Authorization</span></span>|<span data-ttu-id="d3a97-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="d3a97-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d3a97-124">承諾</span><span class="sxs-lookup"><span data-stu-id="d3a97-124">Accept</span></span>|<span data-ttu-id="d3a97-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d3a97-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d3a97-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="d3a97-126">Request body</span></span>
<span data-ttu-id="d3a97-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="d3a97-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d3a97-128">応答</span><span class="sxs-lookup"><span data-stu-id="d3a97-128">Response</span></span>
<span data-ttu-id="d3a97-129">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[Devicemanagementcomplexsettinginstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="d3a97-129">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementComplexSettingInstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d3a97-130">例</span><span class="sxs-lookup"><span data-stu-id="d3a97-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="d3a97-131">要求</span><span class="sxs-lookup"><span data-stu-id="d3a97-131">Request</span></span>
<span data-ttu-id="d3a97-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d3a97-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/settings
```

### <a name="response"></a><span data-ttu-id="d3a97-133">応答</span><span class="sxs-lookup"><span data-stu-id="d3a97-133">Response</span></span>
<span data-ttu-id="d3a97-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d3a97-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 256

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementComplexSettingInstance",
      "id": "4deb3935-3935-4deb-3539-eb4d3539eb4d",
      "definitionId": "Definition Id value",
      "valueJson": "Value Json value"
    }
  ]
}
```






