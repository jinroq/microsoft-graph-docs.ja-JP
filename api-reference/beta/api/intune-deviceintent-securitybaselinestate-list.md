---
title: リスト securityBaselineStates
description: securityBaselineState オブジェクトのプロパティとリレーションシップをリストします。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4d1c334b5f377d4fd31e2209bf6940fc2bf65a76
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31783494"
---
# <a name="list-securitybaselinestates"></a><span data-ttu-id="95283-103">リスト securityBaselineStates</span><span class="sxs-lookup"><span data-stu-id="95283-103">List securityBaselineStates</span></span>

> <span data-ttu-id="95283-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="95283-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="95283-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="95283-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="95283-106">[securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="95283-106">List properties and relationships of the [securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="95283-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="95283-107">Prerequisites</span></span>
<span data-ttu-id="95283-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="95283-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="95283-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="95283-110">Permission type</span></span>|<span data-ttu-id="95283-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="95283-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="95283-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="95283-112">Delegated (work or school account)</span></span>|<span data-ttu-id="95283-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="95283-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="95283-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="95283-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="95283-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="95283-115">Not supported.</span></span>|
|<span data-ttu-id="95283-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="95283-116">Application</span></span>|<span data-ttu-id="95283-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="95283-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="95283-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="95283-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managedDevices/{managedDeviceId}/securityBaselineStates
```

## <a name="request-headers"></a><span data-ttu-id="95283-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="95283-119">Request headers</span></span>
|<span data-ttu-id="95283-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="95283-120">Header</span></span>|<span data-ttu-id="95283-121">値</span><span class="sxs-lookup"><span data-stu-id="95283-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="95283-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="95283-122">Authorization</span></span>|<span data-ttu-id="95283-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="95283-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="95283-124">承諾</span><span class="sxs-lookup"><span data-stu-id="95283-124">Accept</span></span>|<span data-ttu-id="95283-125">application/json</span><span class="sxs-lookup"><span data-stu-id="95283-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="95283-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="95283-126">Request body</span></span>
<span data-ttu-id="95283-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="95283-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="95283-128">応答</span><span class="sxs-lookup"><span data-stu-id="95283-128">Response</span></span>
<span data-ttu-id="95283-129">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="95283-129">If successful, this method returns a `200 OK` response code and a collection of [securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="95283-130">例</span><span class="sxs-lookup"><span data-stu-id="95283-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="95283-131">要求</span><span class="sxs-lookup"><span data-stu-id="95283-131">Request</span></span>
<span data-ttu-id="95283-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="95283-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/securityBaselineStates
```

### <a name="response"></a><span data-ttu-id="95283-133">応答</span><span class="sxs-lookup"><span data-stu-id="95283-133">Response</span></span>
<span data-ttu-id="95283-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="95283-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 273

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.securityBaselineState",
      "id": "23dc2503-2503-23dc-0325-dc230325dc23",
      "securityBaselineTemplateId": "Security Baseline Template Id value",
      "displayName": "Display Name value"
    }
  ]
}
```



