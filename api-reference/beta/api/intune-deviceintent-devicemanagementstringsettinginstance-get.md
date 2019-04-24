---
title: devicemanagementstringsettinginstance を取得する
description: devicemanagementstringsettinginstance オブジェクトのプロパティとリレーションシップを読み取ります。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1084c57fb60b083c5c3dda21cfc33746f642692d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32466715"
---
# <a name="get-devicemanagementstringsettinginstance"></a><span data-ttu-id="5e488-103">devicemanagementstringsettinginstance を取得する</span><span class="sxs-lookup"><span data-stu-id="5e488-103">Get deviceManagementStringSettingInstance</span></span>

> <span data-ttu-id="5e488-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5e488-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5e488-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="5e488-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5e488-106">[devicemanagementstringsettinginstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="5e488-106">Read properties and relationships of the [deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5e488-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="5e488-107">Prerequisites</span></span>
<span data-ttu-id="5e488-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5e488-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5e488-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5e488-110">Permission type</span></span>|<span data-ttu-id="5e488-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="5e488-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5e488-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5e488-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5e488-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="5e488-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="5e488-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5e488-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5e488-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5e488-115">Not supported.</span></span>|
|<span data-ttu-id="5e488-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5e488-116">Application</span></span>|<span data-ttu-id="5e488-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5e488-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5e488-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5e488-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/intents/{deviceManagementIntentId}/settings/{deviceManagementSettingInstanceId}
GET /deviceManagement/templates/{deviceManagementTemplateId}/settings/{deviceManagementSettingInstanceId}
GET /deviceManagement/intents/{deviceManagementIntentId}/categories/{deviceManagementIntentSettingCategoryId}/settings/{deviceManagementSettingInstanceId}
GET /deviceManagement/templates/{deviceManagementTemplateId}/categories/{deviceManagementTemplateSettingCategoryId}/recommendedSettings/{deviceManagementSettingInstanceId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5e488-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="5e488-119">Optional query parameters</span></span>
<span data-ttu-id="5e488-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="5e488-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5e488-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5e488-121">Request headers</span></span>
|<span data-ttu-id="5e488-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5e488-122">Header</span></span>|<span data-ttu-id="5e488-123">値</span><span class="sxs-lookup"><span data-stu-id="5e488-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5e488-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="5e488-124">Authorization</span></span>|<span data-ttu-id="5e488-125">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="5e488-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5e488-126">承諾</span><span class="sxs-lookup"><span data-stu-id="5e488-126">Accept</span></span>|<span data-ttu-id="5e488-127">application/json</span><span class="sxs-lookup"><span data-stu-id="5e488-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5e488-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="5e488-128">Request body</span></span>
<span data-ttu-id="5e488-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="5e488-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5e488-130">応答</span><span class="sxs-lookup"><span data-stu-id="5e488-130">Response</span></span>
<span data-ttu-id="5e488-131">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[devicemanagementstringsettinginstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="5e488-131">If successful, this method returns a `200 OK` response code and [deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5e488-132">例</span><span class="sxs-lookup"><span data-stu-id="5e488-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="5e488-133">要求</span><span class="sxs-lookup"><span data-stu-id="5e488-133">Request</span></span>
<span data-ttu-id="5e488-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="5e488-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/settings/{deviceManagementSettingInstanceId}
```

### <a name="response"></a><span data-ttu-id="5e488-135">応答</span><span class="sxs-lookup"><span data-stu-id="5e488-135">Response</span></span>
<span data-ttu-id="5e488-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="5e488-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 262

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementStringSettingInstance",
    "id": "fef30638-0638-fef3-3806-f3fe3806f3fe",
    "definitionId": "Definition Id value",
    "valueJson": "Value Json value",
    "value": "Value value"
  }
}
```





