---
title: リスト deviceManagementBooleanSettingInstances
description: DeviceManagementBooleanSettingInstance オブジェクトのプロパティとリレーションシップをリストします。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 042022881c853889e46ab1932c9fa85a5d812f46
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36313497"
---
# <a name="list-devicemanagementbooleansettinginstances"></a><span data-ttu-id="79218-103">リスト deviceManagementBooleanSettingInstances</span><span class="sxs-lookup"><span data-stu-id="79218-103">List deviceManagementBooleanSettingInstances</span></span>

> <span data-ttu-id="79218-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="79218-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="79218-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="79218-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="79218-106">[DeviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="79218-106">List properties and relationships of the [deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="79218-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="79218-107">Prerequisites</span></span>
<span data-ttu-id="79218-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="79218-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="79218-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="79218-110">Permission type</span></span>|<span data-ttu-id="79218-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="79218-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="79218-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="79218-112">Delegated (work or school account)</span></span>|<span data-ttu-id="79218-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="79218-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="79218-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="79218-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="79218-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="79218-115">Not supported.</span></span>|
|<span data-ttu-id="79218-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="79218-116">Application</span></span>|<span data-ttu-id="79218-117">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="79218-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="79218-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="79218-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="79218-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="79218-119">Request headers</span></span>
|<span data-ttu-id="79218-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="79218-120">Header</span></span>|<span data-ttu-id="79218-121">値</span><span class="sxs-lookup"><span data-stu-id="79218-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="79218-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="79218-122">Authorization</span></span>|<span data-ttu-id="79218-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="79218-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="79218-124">承諾</span><span class="sxs-lookup"><span data-stu-id="79218-124">Accept</span></span>|<span data-ttu-id="79218-125">application/json</span><span class="sxs-lookup"><span data-stu-id="79218-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="79218-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="79218-126">Request body</span></span>
<span data-ttu-id="79218-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="79218-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="79218-128">応答</span><span class="sxs-lookup"><span data-stu-id="79218-128">Response</span></span>
<span data-ttu-id="79218-129">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="79218-129">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="79218-130">例</span><span class="sxs-lookup"><span data-stu-id="79218-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="79218-131">要求</span><span class="sxs-lookup"><span data-stu-id="79218-131">Request</span></span>
<span data-ttu-id="79218-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="79218-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/settings
```

### <a name="response"></a><span data-ttu-id="79218-133">応答</span><span class="sxs-lookup"><span data-stu-id="79218-133">Response</span></span>
<span data-ttu-id="79218-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="79218-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 278

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementBooleanSettingInstance",
      "id": "bb9b0041-0041-bb9b-4100-9bbb41009bbb",
      "definitionId": "Definition Id value",
      "valueJson": "Value Json value",
      "value": true
    }
  ]
}
```






