---
title: DeviceManagementScriptUserStates のリスト
description: DeviceManagementScriptUserState オブジェクトのプロパティとリレーションシップをリストします。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d00469f62e3823ee08f8fdcc15cb832e4935d60e
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36348796"
---
# <a name="list-devicemanagementscriptuserstates"></a><span data-ttu-id="8dcfe-103">DeviceManagementScriptUserStates のリスト</span><span class="sxs-lookup"><span data-stu-id="8dcfe-103">List deviceManagementScriptUserStates</span></span>

> <span data-ttu-id="8dcfe-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8dcfe-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8dcfe-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="8dcfe-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8dcfe-106">[Devicemanagementscriptuserstate](../resources/intune-devices-devicemanagementscriptuserstate.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="8dcfe-106">List properties and relationships of the [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8dcfe-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="8dcfe-107">Prerequisites</span></span>
<span data-ttu-id="8dcfe-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8dcfe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8dcfe-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8dcfe-110">Permission type</span></span>|<span data-ttu-id="8dcfe-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="8dcfe-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8dcfe-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8dcfe-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8dcfe-113">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="8dcfe-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="8dcfe-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8dcfe-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8dcfe-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8dcfe-115">Not supported.</span></span>|
|<span data-ttu-id="8dcfe-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8dcfe-116">Application</span></span>|<span data-ttu-id="8dcfe-117">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="8dcfe-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8dcfe-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8dcfe-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates
```

## <a name="request-headers"></a><span data-ttu-id="8dcfe-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8dcfe-119">Request headers</span></span>
|<span data-ttu-id="8dcfe-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8dcfe-120">Header</span></span>|<span data-ttu-id="8dcfe-121">値</span><span class="sxs-lookup"><span data-stu-id="8dcfe-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8dcfe-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8dcfe-122">Authorization</span></span>|<span data-ttu-id="8dcfe-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="8dcfe-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8dcfe-124">承諾</span><span class="sxs-lookup"><span data-stu-id="8dcfe-124">Accept</span></span>|<span data-ttu-id="8dcfe-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8dcfe-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8dcfe-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="8dcfe-126">Request body</span></span>
<span data-ttu-id="8dcfe-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="8dcfe-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8dcfe-128">応答</span><span class="sxs-lookup"><span data-stu-id="8dcfe-128">Response</span></span>
<span data-ttu-id="8dcfe-129">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[Devicemanagementscriptuserstate](../resources/intune-devices-devicemanagementscriptuserstate.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="8dcfe-129">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8dcfe-130">例</span><span class="sxs-lookup"><span data-stu-id="8dcfe-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="8dcfe-131">要求</span><span class="sxs-lookup"><span data-stu-id="8dcfe-131">Request</span></span>
<span data-ttu-id="8dcfe-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8dcfe-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates
```

### <a name="response"></a><span data-ttu-id="8dcfe-133">応答</span><span class="sxs-lookup"><span data-stu-id="8dcfe-133">Response</span></span>
<span data-ttu-id="8dcfe-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8dcfe-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 282

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementScriptUserState",
      "id": "d5a29103-9103-d5a2-0391-a2d50391a2d5",
      "successDeviceCount": 2,
      "errorDeviceCount": 0,
      "userPrincipalName": "User Principal Name value"
    }
  ]
}
```






