---
title: DeviceManagementScriptUserState の作成
description: 新しい deviceManagementScriptUserState オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 872c3a039d0fd474e94492aac814745da188d3aa
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33909807"
---
# <a name="create-devicemanagementscriptuserstate"></a><span data-ttu-id="042b4-103">DeviceManagementScriptUserState の作成</span><span class="sxs-lookup"><span data-stu-id="042b4-103">Create deviceManagementScriptUserState</span></span>

> <span data-ttu-id="042b4-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="042b4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="042b4-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="042b4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="042b4-106">新しい[Devicemanagementscriptuserstate](../resources/intune-devices-devicemanagementscriptuserstate.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="042b4-106">Create a new [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="042b4-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="042b4-107">Prerequisites</span></span>
<span data-ttu-id="042b4-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="042b4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="042b4-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="042b4-110">Permission type</span></span>|<span data-ttu-id="042b4-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="042b4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="042b4-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="042b4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="042b4-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="042b4-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="042b4-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="042b4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="042b4-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="042b4-115">Not supported.</span></span>|
|<span data-ttu-id="042b4-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="042b4-116">Application</span></span>|<span data-ttu-id="042b4-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="042b4-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="042b4-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="042b4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates
```

## <a name="request-headers"></a><span data-ttu-id="042b4-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="042b4-119">Request headers</span></span>
|<span data-ttu-id="042b4-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="042b4-120">Header</span></span>|<span data-ttu-id="042b4-121">値</span><span class="sxs-lookup"><span data-stu-id="042b4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="042b4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="042b4-122">Authorization</span></span>|<span data-ttu-id="042b4-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="042b4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="042b4-124">承諾</span><span class="sxs-lookup"><span data-stu-id="042b4-124">Accept</span></span>|<span data-ttu-id="042b4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="042b4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="042b4-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="042b4-126">Request body</span></span>
<span data-ttu-id="042b4-127">要求本文で、deviceManagementScriptUserState オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="042b4-127">In the request body, supply a JSON representation for the deviceManagementScriptUserState object.</span></span>

<span data-ttu-id="042b4-128">次の表に、deviceManagementScriptUserState の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="042b4-128">The following table shows the properties that are required when you create the deviceManagementScriptUserState.</span></span>

|<span data-ttu-id="042b4-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="042b4-129">Property</span></span>|<span data-ttu-id="042b4-130">型</span><span class="sxs-lookup"><span data-stu-id="042b4-130">Type</span></span>|<span data-ttu-id="042b4-131">説明</span><span class="sxs-lookup"><span data-stu-id="042b4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="042b4-132">id</span><span class="sxs-lookup"><span data-stu-id="042b4-132">id</span></span>|<span data-ttu-id="042b4-133">文字列</span><span class="sxs-lookup"><span data-stu-id="042b4-133">String</span></span>|<span data-ttu-id="042b4-134">デバイス管理スクリプトのユーザー状態エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="042b4-134">Key of the device management script user state entity.</span></span>|
|<span data-ttu-id="042b4-135">successDeviceCount</span><span class="sxs-lookup"><span data-stu-id="042b4-135">successDeviceCount</span></span>|<span data-ttu-id="042b4-136">Int32</span><span class="sxs-lookup"><span data-stu-id="042b4-136">Int32</span></span>|<span data-ttu-id="042b4-137">特定のユーザーの成功デバイス数。</span><span class="sxs-lookup"><span data-stu-id="042b4-137">Success device count for specific user.</span></span>|
|<span data-ttu-id="042b4-138">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="042b4-138">errorDeviceCount</span></span>|<span data-ttu-id="042b4-139">Int32</span><span class="sxs-lookup"><span data-stu-id="042b4-139">Int32</span></span>|<span data-ttu-id="042b4-140">特定のユーザーのエラーデバイス数。</span><span class="sxs-lookup"><span data-stu-id="042b4-140">Error device count for specific user.</span></span>|
|<span data-ttu-id="042b4-141">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="042b4-141">userPrincipalName</span></span>|<span data-ttu-id="042b4-142">String</span><span class="sxs-lookup"><span data-stu-id="042b4-142">String</span></span>|<span data-ttu-id="042b4-143">特定のユーザーのユーザープリンシパル名。</span><span class="sxs-lookup"><span data-stu-id="042b4-143">User principle name of specific user.</span></span>|



## <a name="response"></a><span data-ttu-id="042b4-144">応答</span><span class="sxs-lookup"><span data-stu-id="042b4-144">Response</span></span>
<span data-ttu-id="042b4-145">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[Devicemanagementscriptuserstate](../resources/intune-devices-devicemanagementscriptuserstate.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="042b4-145">If successful, this method returns a `201 Created` response code and a [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="042b4-146">例</span><span class="sxs-lookup"><span data-stu-id="042b4-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="042b4-147">要求</span><span class="sxs-lookup"><span data-stu-id="042b4-147">Request</span></span>
<span data-ttu-id="042b4-148">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="042b4-148">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="042b4-149">応答</span><span class="sxs-lookup"><span data-stu-id="042b4-149">Response</span></span>
<span data-ttu-id="042b4-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="042b4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




