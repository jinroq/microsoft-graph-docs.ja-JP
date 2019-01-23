---
title: DeviceManagementScriptUserState を作成します。
description: 新しい deviceManagementScriptUserState オブジェクトを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 01ab54a736a5e9d1a305bff44a601494e8ec8860
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29424267"
---
# <a name="create-devicemanagementscriptuserstate"></a><span data-ttu-id="4fb6e-103">DeviceManagementScriptUserState を作成します。</span><span class="sxs-lookup"><span data-stu-id="4fb6e-103">Create deviceManagementScriptUserState</span></span>

> <span data-ttu-id="4fb6e-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="4fb6e-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="4fb6e-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4fb6e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4fb6e-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="4fb6e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4fb6e-107">新しい[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="4fb6e-107">Create a new [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4fb6e-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="4fb6e-108">Prerequisites</span></span>
<span data-ttu-id="4fb6e-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4fb6e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="4fb6e-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4fb6e-111">Permission type</span></span>|<span data-ttu-id="4fb6e-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="4fb6e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4fb6e-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4fb6e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4fb6e-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4fb6e-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="4fb6e-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4fb6e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4fb6e-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4fb6e-116">Not supported.</span></span>|
|<span data-ttu-id="4fb6e-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4fb6e-117">Application</span></span>|<span data-ttu-id="4fb6e-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4fb6e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4fb6e-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4fb6e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates
```

## <a name="request-headers"></a><span data-ttu-id="4fb6e-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4fb6e-120">Request headers</span></span>
|<span data-ttu-id="4fb6e-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4fb6e-121">Header</span></span>|<span data-ttu-id="4fb6e-122">値</span><span class="sxs-lookup"><span data-stu-id="4fb6e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4fb6e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4fb6e-123">Authorization</span></span>|<span data-ttu-id="4fb6e-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="4fb6e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4fb6e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4fb6e-125">Accept</span></span>|<span data-ttu-id="4fb6e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4fb6e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4fb6e-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="4fb6e-127">Request body</span></span>
<span data-ttu-id="4fb6e-128">要求の本文に deviceManagementScriptUserState オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="4fb6e-128">In the request body, supply a JSON representation for the deviceManagementScriptUserState object.</span></span>

<span data-ttu-id="4fb6e-129">次の表は、deviceManagementScriptUserState を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="4fb6e-129">The following table shows the properties that are required when you create the deviceManagementScriptUserState.</span></span>

|<span data-ttu-id="4fb6e-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4fb6e-130">Property</span></span>|<span data-ttu-id="4fb6e-131">型</span><span class="sxs-lookup"><span data-stu-id="4fb6e-131">Type</span></span>|<span data-ttu-id="4fb6e-132">説明</span><span class="sxs-lookup"><span data-stu-id="4fb6e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4fb6e-133">id</span><span class="sxs-lookup"><span data-stu-id="4fb6e-133">id</span></span>|<span data-ttu-id="4fb6e-134">String</span><span class="sxs-lookup"><span data-stu-id="4fb6e-134">String</span></span>|<span data-ttu-id="4fb6e-135">デバイス管理スクリプト ユーザー状態のエンティティのキーです。</span><span class="sxs-lookup"><span data-stu-id="4fb6e-135">Key of the device management script user state entity.</span></span>|
|<span data-ttu-id="4fb6e-136">successDeviceCount</span><span class="sxs-lookup"><span data-stu-id="4fb6e-136">successDeviceCount</span></span>|<span data-ttu-id="4fb6e-137">Int32</span><span class="sxs-lookup"><span data-stu-id="4fb6e-137">Int32</span></span>|<span data-ttu-id="4fb6e-138">デバイスの数の特定のユーザーに成功します。</span><span class="sxs-lookup"><span data-stu-id="4fb6e-138">Success device count for specific user.</span></span>|
|<span data-ttu-id="4fb6e-139">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="4fb6e-139">errorDeviceCount</span></span>|<span data-ttu-id="4fb6e-140">Int32</span><span class="sxs-lookup"><span data-stu-id="4fb6e-140">Int32</span></span>|<span data-ttu-id="4fb6e-141">特定のユーザー エラー デバイスの数。</span><span class="sxs-lookup"><span data-stu-id="4fb6e-141">Error device count for specific user.</span></span>|
|<span data-ttu-id="4fb6e-142">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="4fb6e-142">userPrincipalName</span></span>|<span data-ttu-id="4fb6e-143">String</span><span class="sxs-lookup"><span data-stu-id="4fb6e-143">String</span></span>|<span data-ttu-id="4fb6e-144">特定のユーザーのユーザー プリンシパル名です。</span><span class="sxs-lookup"><span data-stu-id="4fb6e-144">User principle name of specific user.</span></span>|



## <a name="response"></a><span data-ttu-id="4fb6e-145">応答</span><span class="sxs-lookup"><span data-stu-id="4fb6e-145">Response</span></span>
<span data-ttu-id="4fb6e-146">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="4fb6e-146">If successful, this method returns a `201 Created` response code and a [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4fb6e-147">例</span><span class="sxs-lookup"><span data-stu-id="4fb6e-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="4fb6e-148">要求</span><span class="sxs-lookup"><span data-stu-id="4fb6e-148">Request</span></span>
<span data-ttu-id="4fb6e-149">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4fb6e-149">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates
Content-type: application/json
Content-length: 180

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptUserState",
  "successDeviceCount": 2,
  "errorDeviceCount": 0,
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="4fb6e-150">応答</span><span class="sxs-lookup"><span data-stu-id="4fb6e-150">Response</span></span>
<span data-ttu-id="4fb6e-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="4fb6e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 229

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptUserState",
  "id": "d5a29103-9103-d5a2-0391-a2d50391a2d5",
  "successDeviceCount": 2,
  "errorDeviceCount": 0,
  "userPrincipalName": "User Principal Name value"
}
```




