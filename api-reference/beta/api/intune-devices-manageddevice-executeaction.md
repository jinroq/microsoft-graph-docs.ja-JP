---
title: executeAction アクション
description: まだ文書化されていません
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 24311c198127b2ac8fb618285e6a6eba8b44c12d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29404415"
---
# <a name="executeaction-action"></a><span data-ttu-id="ba97a-103">executeAction アクション</span><span class="sxs-lookup"><span data-stu-id="ba97a-103">executeAction action</span></span>

> <span data-ttu-id="ba97a-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ba97a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ba97a-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ba97a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ba97a-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ba97a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ba97a-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="ba97a-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ba97a-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="ba97a-108">Prerequisites</span></span>
<span data-ttu-id="ba97a-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ba97a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="ba97a-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ba97a-111">Permission type</span></span>|<span data-ttu-id="ba97a-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="ba97a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ba97a-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ba97a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ba97a-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="ba97a-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="ba97a-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ba97a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ba97a-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ba97a-116">Not supported.</span></span>|
|<span data-ttu-id="ba97a-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ba97a-117">Application</span></span>|<span data-ttu-id="ba97a-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ba97a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ba97a-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ba97a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/executeAction
POST /deviceManagement/managedDevices/executeAction
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/executeAction
```

## <a name="request-headers"></a><span data-ttu-id="ba97a-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ba97a-120">Request headers</span></span>
|<span data-ttu-id="ba97a-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ba97a-121">Header</span></span>|<span data-ttu-id="ba97a-122">値</span><span class="sxs-lookup"><span data-stu-id="ba97a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ba97a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ba97a-123">Authorization</span></span>|<span data-ttu-id="ba97a-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="ba97a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ba97a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ba97a-125">Accept</span></span>|<span data-ttu-id="ba97a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ba97a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ba97a-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="ba97a-127">Request body</span></span>
<span data-ttu-id="ba97a-128">要求本文で、パラメーターの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="ba97a-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="ba97a-129">次の表に、このアクションで使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="ba97a-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="ba97a-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ba97a-130">Property</span></span>|<span data-ttu-id="ba97a-131">型</span><span class="sxs-lookup"><span data-stu-id="ba97a-131">Type</span></span>|<span data-ttu-id="ba97a-132">説明</span><span class="sxs-lookup"><span data-stu-id="ba97a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ba97a-133">actionName</span><span class="sxs-lookup"><span data-stu-id="ba97a-133">actionName</span></span>|[<span data-ttu-id="ba97a-134">managedDeviceRemoteAction</span><span class="sxs-lookup"><span data-stu-id="ba97a-134">managedDeviceRemoteAction</span></span>](../resources/intune-devices-manageddeviceremoteaction.md)|<span data-ttu-id="ba97a-135">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="ba97a-135">Not yet documented</span></span>|
|<span data-ttu-id="ba97a-136">deviceIds</span><span class="sxs-lookup"><span data-stu-id="ba97a-136">deviceIds</span></span>|<span data-ttu-id="ba97a-137">String コレクション</span><span class="sxs-lookup"><span data-stu-id="ba97a-137">String collection</span></span>|<span data-ttu-id="ba97a-138">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="ba97a-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="ba97a-139">応答</span><span class="sxs-lookup"><span data-stu-id="ba97a-139">Response</span></span>
<span data-ttu-id="ba97a-140">かどうか、成功を返すアクション、`200 OK`応答コードおよび応答の本文には[bulkManagedDeviceActionResult](../resources/intune-devices-bulkmanageddeviceactionresult.md)です。</span><span class="sxs-lookup"><span data-stu-id="ba97a-140">If successful, this action returns a `200 OK` response code and a [bulkManagedDeviceActionResult](../resources/intune-devices-bulkmanageddeviceactionresult.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ba97a-141">例</span><span class="sxs-lookup"><span data-stu-id="ba97a-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="ba97a-142">要求</span><span class="sxs-lookup"><span data-stu-id="ba97a-142">Request</span></span>
<span data-ttu-id="ba97a-143">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ba97a-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/users/{usersId}/managedDevices/executeAction

Content-type: application/json
Content-length: 78

{
  "actionName": "delete",
  "deviceIds": [
    "Device Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="ba97a-144">応答</span><span class="sxs-lookup"><span data-stu-id="ba97a-144">Response</span></span>
<span data-ttu-id="ba97a-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ba97a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 385

{
  "value": {
    "@odata.type": "microsoft.graph.bulkManagedDeviceActionResult",
    "successfulDeviceIds": [
      "Successful Device Ids value"
    ],
    "failedDeviceIds": [
      "Failed Device Ids value"
    ],
    "notFoundDeviceIds": [
      "Not Found Device Ids value"
    ],
    "notSupportedDeviceIds": [
      "Not Supported Device Ids value"
    ]
  }
}
```




