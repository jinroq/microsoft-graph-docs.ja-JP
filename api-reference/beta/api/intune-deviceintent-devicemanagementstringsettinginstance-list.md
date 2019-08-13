---
title: DeviceManagementStringSettingInstances を一覧表示する
description: DeviceManagementStringSettingInstance オブジェクトのプロパティとリレーションシップをリストします。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e9a5285cec30a7d631c81346f0c9a85303dbb7bc
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36313161"
---
# <a name="list-devicemanagementstringsettinginstances"></a><span data-ttu-id="f86f8-103">DeviceManagementStringSettingInstances を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="f86f8-103">List deviceManagementStringSettingInstances</span></span>

> <span data-ttu-id="f86f8-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f86f8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f86f8-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f86f8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f86f8-106">[Devicemanagementstringsettinginstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="f86f8-106">List properties and relationships of the [deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f86f8-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="f86f8-107">Prerequisites</span></span>
<span data-ttu-id="f86f8-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f86f8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f86f8-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f86f8-110">Permission type</span></span>|<span data-ttu-id="f86f8-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="f86f8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f86f8-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f86f8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f86f8-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f86f8-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="f86f8-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f86f8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f86f8-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f86f8-115">Not supported.</span></span>|
|<span data-ttu-id="f86f8-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f86f8-116">Application</span></span>|<span data-ttu-id="f86f8-117">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f86f8-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f86f8-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f86f8-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="f86f8-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f86f8-119">Request headers</span></span>
|<span data-ttu-id="f86f8-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f86f8-120">Header</span></span>|<span data-ttu-id="f86f8-121">値</span><span class="sxs-lookup"><span data-stu-id="f86f8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f86f8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f86f8-122">Authorization</span></span>|<span data-ttu-id="f86f8-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="f86f8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f86f8-124">承諾</span><span class="sxs-lookup"><span data-stu-id="f86f8-124">Accept</span></span>|<span data-ttu-id="f86f8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f86f8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f86f8-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="f86f8-126">Request body</span></span>
<span data-ttu-id="f86f8-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="f86f8-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f86f8-128">応答</span><span class="sxs-lookup"><span data-stu-id="f86f8-128">Response</span></span>
<span data-ttu-id="f86f8-129">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[Devicemanagementstringsettinginstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="f86f8-129">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f86f8-130">例</span><span class="sxs-lookup"><span data-stu-id="f86f8-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="f86f8-131">要求</span><span class="sxs-lookup"><span data-stu-id="f86f8-131">Request</span></span>
<span data-ttu-id="f86f8-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f86f8-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/settings
```

### <a name="response"></a><span data-ttu-id="f86f8-133">応答</span><span class="sxs-lookup"><span data-stu-id="f86f8-133">Response</span></span>
<span data-ttu-id="f86f8-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f86f8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 286

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementStringSettingInstance",
      "id": "fef30638-0638-fef3-3806-f3fe3806f3fe",
      "definitionId": "Definition Id value",
      "valueJson": "Value Json value",
      "value": "Value value"
    }
  ]
}
```






