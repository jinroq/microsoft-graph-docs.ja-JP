---
title: DeviceManagementScriptUserState を作成します。
description: 新しい deviceManagementScriptUserState オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 76be7695b64b660ec4da3b2d4d19928ea7b57bff
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27873354"
---
# <a name="create-devicemanagementscriptuserstate"></a><span data-ttu-id="72888-103">DeviceManagementScriptUserState を作成します。</span><span class="sxs-lookup"><span data-stu-id="72888-103">Create deviceManagementScriptUserState</span></span>

> <span data-ttu-id="72888-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="72888-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="72888-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="72888-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="72888-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="72888-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="72888-107">新しい[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="72888-107">Create a new [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="72888-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="72888-108">Prerequisites</span></span>
<span data-ttu-id="72888-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="72888-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="72888-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="72888-111">Permission type</span></span>|<span data-ttu-id="72888-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="72888-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="72888-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="72888-113">Delegated (work or school account)</span></span>|<span data-ttu-id="72888-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="72888-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="72888-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="72888-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="72888-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="72888-116">Not supported.</span></span>|
|<span data-ttu-id="72888-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="72888-117">Application</span></span>|<span data-ttu-id="72888-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="72888-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="72888-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="72888-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates
```

## <a name="request-headers"></a><span data-ttu-id="72888-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="72888-120">Request headers</span></span>
|<span data-ttu-id="72888-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="72888-121">Header</span></span>|<span data-ttu-id="72888-122">値</span><span class="sxs-lookup"><span data-stu-id="72888-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="72888-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="72888-123">Authorization</span></span>|<span data-ttu-id="72888-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="72888-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="72888-125">Accept</span><span class="sxs-lookup"><span data-stu-id="72888-125">Accept</span></span>|<span data-ttu-id="72888-126">application/json</span><span class="sxs-lookup"><span data-stu-id="72888-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="72888-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="72888-127">Request body</span></span>
<span data-ttu-id="72888-128">要求の本文に deviceManagementScriptUserState オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="72888-128">In the request body, supply a JSON representation for the deviceManagementScriptUserState object.</span></span>

<span data-ttu-id="72888-129">次の表は、deviceManagementScriptUserState を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="72888-129">The following table shows the properties that are required when you create the deviceManagementScriptUserState.</span></span>

|<span data-ttu-id="72888-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="72888-130">Property</span></span>|<span data-ttu-id="72888-131">種類</span><span class="sxs-lookup"><span data-stu-id="72888-131">Type</span></span>|<span data-ttu-id="72888-132">説明</span><span class="sxs-lookup"><span data-stu-id="72888-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="72888-133">ID</span><span class="sxs-lookup"><span data-stu-id="72888-133">id</span></span>|<span data-ttu-id="72888-134">String</span><span class="sxs-lookup"><span data-stu-id="72888-134">String</span></span>|<span data-ttu-id="72888-135">デバイス管理スクリプト ユーザー状態のエンティティのキーです。</span><span class="sxs-lookup"><span data-stu-id="72888-135">Key of the device management script user state entity.</span></span>|
|<span data-ttu-id="72888-136">successDeviceCount</span><span class="sxs-lookup"><span data-stu-id="72888-136">successDeviceCount</span></span>|<span data-ttu-id="72888-137">Int32</span><span class="sxs-lookup"><span data-stu-id="72888-137">Int32</span></span>|<span data-ttu-id="72888-138">デバイスの数の特定のユーザーに成功します。</span><span class="sxs-lookup"><span data-stu-id="72888-138">Success device count for specific user.</span></span>|
|<span data-ttu-id="72888-139">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="72888-139">errorDeviceCount</span></span>|<span data-ttu-id="72888-140">Int32</span><span class="sxs-lookup"><span data-stu-id="72888-140">Int32</span></span>|<span data-ttu-id="72888-141">特定のユーザー エラー デバイスの数。</span><span class="sxs-lookup"><span data-stu-id="72888-141">Error device count for specific user.</span></span>|
|<span data-ttu-id="72888-142">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="72888-142">userPrincipalName</span></span>|<span data-ttu-id="72888-143">String</span><span class="sxs-lookup"><span data-stu-id="72888-143">String</span></span>|<span data-ttu-id="72888-144">特定のユーザーのユーザー プリンシパル名です。</span><span class="sxs-lookup"><span data-stu-id="72888-144">User principle name of specific user.</span></span>|



## <a name="response"></a><span data-ttu-id="72888-145">応答</span><span class="sxs-lookup"><span data-stu-id="72888-145">Response</span></span>
<span data-ttu-id="72888-146">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="72888-146">If successful, this method returns a `201 Created` response code and a [deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="72888-147">例</span><span class="sxs-lookup"><span data-stu-id="72888-147">Example</span></span>
### <a name="request"></a><span data-ttu-id="72888-148">要求</span><span class="sxs-lookup"><span data-stu-id="72888-148">Request</span></span>
<span data-ttu-id="72888-149">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="72888-149">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="72888-150">応答</span><span class="sxs-lookup"><span data-stu-id="72888-150">Response</span></span>
<span data-ttu-id="72888-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="72888-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





