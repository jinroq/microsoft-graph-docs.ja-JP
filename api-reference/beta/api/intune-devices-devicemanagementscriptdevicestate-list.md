---
title: リスト deviceManagementScriptDeviceStates
description: DeviceManagementScriptDeviceState オブジェクトのプロパティと関係を一覧表示します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: aec150805b9e272b1289bc2445678f5bb3118e9b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27858423"
---
# <a name="list-devicemanagementscriptdevicestates"></a><span data-ttu-id="cf012-103">リスト deviceManagementScriptDeviceStates</span><span class="sxs-lookup"><span data-stu-id="cf012-103">List deviceManagementScriptDeviceStates</span></span>

> <span data-ttu-id="cf012-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="cf012-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cf012-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cf012-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cf012-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="cf012-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cf012-107">[DeviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="cf012-107">List properties and relationships of the [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cf012-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="cf012-108">Prerequisites</span></span>
<span data-ttu-id="cf012-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cf012-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cf012-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="cf012-111">Permission type</span></span>|<span data-ttu-id="cf012-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="cf012-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cf012-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="cf012-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cf012-114">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="cf012-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="cf012-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="cf012-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cf012-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cf012-116">Not supported.</span></span>|
|<span data-ttu-id="cf012-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="cf012-117">Application</span></span>|<span data-ttu-id="cf012-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cf012-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cf012-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="cf012-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates/{deviceManagementScriptUserStateId}/deviceRunStates
```

## <a name="request-headers"></a><span data-ttu-id="cf012-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cf012-120">Request headers</span></span>
|<span data-ttu-id="cf012-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cf012-121">Header</span></span>|<span data-ttu-id="cf012-122">値</span><span class="sxs-lookup"><span data-stu-id="cf012-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cf012-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="cf012-123">Authorization</span></span>|<span data-ttu-id="cf012-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="cf012-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cf012-125">Accept</span><span class="sxs-lookup"><span data-stu-id="cf012-125">Accept</span></span>|<span data-ttu-id="cf012-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cf012-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cf012-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="cf012-127">Request body</span></span>
<span data-ttu-id="cf012-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="cf012-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cf012-129">応答</span><span class="sxs-lookup"><span data-stu-id="cf012-129">Response</span></span>
<span data-ttu-id="cf012-130">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="cf012-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cf012-131">例</span><span class="sxs-lookup"><span data-stu-id="cf012-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="cf012-132">要求</span><span class="sxs-lookup"><span data-stu-id="cf012-132">Request</span></span>
<span data-ttu-id="cf012-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="cf012-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates
```

### <a name="response"></a><span data-ttu-id="cf012-134">応答</span><span class="sxs-lookup"><span data-stu-id="cf012-134">Response</span></span>
<span data-ttu-id="cf012-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="cf012-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 391

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementScriptDeviceState",
      "id": "39440cba-0cba-3944-ba0c-4439ba0c4439",
      "runState": "success",
      "resultMessage": "Result Message value",
      "lastStateUpdateDateTime": "2017-01-01T00:02:58.4418045-08:00",
      "errorCode": 9,
      "errorDescription": "Error Description value"
    }
  ]
}
```





