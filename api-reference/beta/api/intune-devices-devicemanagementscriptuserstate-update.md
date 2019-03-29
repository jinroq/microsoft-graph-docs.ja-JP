---
title: devicemanagementscriptuserstate の更新
description: devicemanagementscriptuserstate オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b211658c96bb9d4935af710018d1405cb8ad3bad
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30973517"
---
# <a name="update-devicemanagementscriptuserstate"></a><span data-ttu-id="0f95e-103">devicemanagementscriptuserstate の更新</span><span class="sxs-lookup"><span data-stu-id="0f95e-103">Update deviceManagementScriptUserState</span></span>

> <span data-ttu-id="0f95e-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0f95e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0f95e-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0f95e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0f95e-106">[devicemanagementscriptuserstate](../resources/intune-devices-devicemanagementscriptuserstate.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="0f95e-106">Update the properties of a [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0f95e-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="0f95e-107">Prerequisites</span></span>
<span data-ttu-id="0f95e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0f95e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0f95e-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0f95e-110">Permission type</span></span>|<span data-ttu-id="0f95e-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="0f95e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0f95e-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0f95e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0f95e-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f95e-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="0f95e-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0f95e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0f95e-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0f95e-115">Not supported.</span></span>|
|<span data-ttu-id="0f95e-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0f95e-116">Application</span></span>|<span data-ttu-id="0f95e-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0f95e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0f95e-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0f95e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates/{deviceManagementScriptUserStateId}
```

## <a name="request-headers"></a><span data-ttu-id="0f95e-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0f95e-119">Request headers</span></span>
|<span data-ttu-id="0f95e-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0f95e-120">Header</span></span>|<span data-ttu-id="0f95e-121">値</span><span class="sxs-lookup"><span data-stu-id="0f95e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0f95e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0f95e-122">Authorization</span></span>|<span data-ttu-id="0f95e-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="0f95e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0f95e-124">承諾</span><span class="sxs-lookup"><span data-stu-id="0f95e-124">Accept</span></span>|<span data-ttu-id="0f95e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0f95e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0f95e-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="0f95e-126">Request body</span></span>
<span data-ttu-id="0f95e-127">要求本文で、 [devicemanagementscriptuserstate](../resources/intune-devices-devicemanagementscriptuserstate.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="0f95e-127">In the request body, supply a JSON representation for the [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) object.</span></span>

<span data-ttu-id="0f95e-128">次の表に、 [devicemanagementscriptuserstate](../resources/intune-devices-devicemanagementscriptuserstate.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="0f95e-128">The following table shows the properties that are required when you create the [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md).</span></span>

|<span data-ttu-id="0f95e-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0f95e-129">Property</span></span>|<span data-ttu-id="0f95e-130">型</span><span class="sxs-lookup"><span data-stu-id="0f95e-130">Type</span></span>|<span data-ttu-id="0f95e-131">説明</span><span class="sxs-lookup"><span data-stu-id="0f95e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f95e-132">id</span><span class="sxs-lookup"><span data-stu-id="0f95e-132">id</span></span>|<span data-ttu-id="0f95e-133">String</span><span class="sxs-lookup"><span data-stu-id="0f95e-133">String</span></span>|<span data-ttu-id="0f95e-134">デバイス管理スクリプトのユーザー状態エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="0f95e-134">Key of the device management script user state entity.</span></span>|
|<span data-ttu-id="0f95e-135">successDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0f95e-135">successDeviceCount</span></span>|<span data-ttu-id="0f95e-136">Int32</span><span class="sxs-lookup"><span data-stu-id="0f95e-136">Int32</span></span>|<span data-ttu-id="0f95e-137">特定のユーザーの成功デバイス数。</span><span class="sxs-lookup"><span data-stu-id="0f95e-137">Success device count for specific user.</span></span>|
|<span data-ttu-id="0f95e-138">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0f95e-138">errorDeviceCount</span></span>|<span data-ttu-id="0f95e-139">Int32</span><span class="sxs-lookup"><span data-stu-id="0f95e-139">Int32</span></span>|<span data-ttu-id="0f95e-140">特定のユーザーのエラーデバイス数。</span><span class="sxs-lookup"><span data-stu-id="0f95e-140">Error device count for specific user.</span></span>|
|<span data-ttu-id="0f95e-141">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="0f95e-141">userPrincipalName</span></span>|<span data-ttu-id="0f95e-142">String</span><span class="sxs-lookup"><span data-stu-id="0f95e-142">String</span></span>|<span data-ttu-id="0f95e-143">特定のユーザーのユーザープリンシパル名。</span><span class="sxs-lookup"><span data-stu-id="0f95e-143">User principle name of specific user.</span></span>|



## <a name="response"></a><span data-ttu-id="0f95e-144">応答</span><span class="sxs-lookup"><span data-stu-id="0f95e-144">Response</span></span>
<span data-ttu-id="0f95e-145">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[devicemanagementscriptuserstate](../resources/intune-devices-devicemanagementscriptuserstate.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="0f95e-145">If successful, this method returns a `200 OK` response code and an updated [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0f95e-146">例</span><span class="sxs-lookup"><span data-stu-id="0f95e-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="0f95e-147">要求</span><span class="sxs-lookup"><span data-stu-id="0f95e-147">Request</span></span>
<span data-ttu-id="0f95e-148">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0f95e-148">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates/{deviceManagementScriptUserStateId}
Content-type: application/json
Content-length: 180

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptUserState",
  "successDeviceCount": 2,
  "errorDeviceCount": 0,
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="0f95e-149">応答</span><span class="sxs-lookup"><span data-stu-id="0f95e-149">Response</span></span>
<span data-ttu-id="0f95e-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0f95e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




