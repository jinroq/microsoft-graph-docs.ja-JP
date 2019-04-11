---
title: embeddedSIMDeviceState を作成する
description: 新しい embeddedSIMDeviceState オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1a2d7561f116287d73b2a0e4f781bf6fa49930ea
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31776998"
---
# <a name="create-embeddedsimdevicestate"></a><span data-ttu-id="c8c76-103">embeddedSIMDeviceState を作成する</span><span class="sxs-lookup"><span data-stu-id="c8c76-103">Create embeddedSIMDeviceState</span></span>

> <span data-ttu-id="c8c76-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c8c76-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c8c76-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c8c76-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c8c76-106">新しい[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="c8c76-106">Create a new [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c8c76-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="c8c76-107">Prerequisites</span></span>
<span data-ttu-id="c8c76-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c8c76-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c8c76-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c8c76-110">Permission type</span></span>|<span data-ttu-id="c8c76-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="c8c76-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c8c76-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c8c76-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c8c76-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c8c76-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c8c76-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c8c76-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c8c76-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c8c76-115">Not supported.</span></span>|
|<span data-ttu-id="c8c76-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c8c76-116">Application</span></span>|<span data-ttu-id="c8c76-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c8c76-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c8c76-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c8c76-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/deviceStates
```

## <a name="request-headers"></a><span data-ttu-id="c8c76-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c8c76-119">Request headers</span></span>
|<span data-ttu-id="c8c76-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c8c76-120">Header</span></span>|<span data-ttu-id="c8c76-121">値</span><span class="sxs-lookup"><span data-stu-id="c8c76-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c8c76-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c8c76-122">Authorization</span></span>|<span data-ttu-id="c8c76-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="c8c76-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c8c76-124">承諾</span><span class="sxs-lookup"><span data-stu-id="c8c76-124">Accept</span></span>|<span data-ttu-id="c8c76-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c8c76-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c8c76-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="c8c76-126">Request body</span></span>
<span data-ttu-id="c8c76-127">要求本文で、embeddedSIMDeviceState オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="c8c76-127">In the request body, supply a JSON representation for the embeddedSIMDeviceState object.</span></span>

<span data-ttu-id="c8c76-128">次の表に、embeddedSIMDeviceState の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="c8c76-128">The following table shows the properties that are required when you create the embeddedSIMDeviceState.</span></span>

|<span data-ttu-id="c8c76-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c8c76-129">Property</span></span>|<span data-ttu-id="c8c76-130">型</span><span class="sxs-lookup"><span data-stu-id="c8c76-130">Type</span></span>|<span data-ttu-id="c8c76-131">説明</span><span class="sxs-lookup"><span data-stu-id="c8c76-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c8c76-132">id</span><span class="sxs-lookup"><span data-stu-id="c8c76-132">id</span></span>|<span data-ttu-id="c8c76-133">String</span><span class="sxs-lookup"><span data-stu-id="c8c76-133">String</span></span>|<span data-ttu-id="c8c76-134">埋め込まれている SIM デバイスの状態を表す一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="c8c76-134">Unique identifier for the embedded SIM device status.</span></span> <span data-ttu-id="c8c76-135">作成時に割り当てられたシステム生成値。</span><span class="sxs-lookup"><span data-stu-id="c8c76-135">System generated value assigned when created.</span></span>|
|<span data-ttu-id="c8c76-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c8c76-136">createdDateTime</span></span>|<span data-ttu-id="c8c76-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c8c76-137">DateTimeOffset</span></span>|<span data-ttu-id="c8c76-138">埋め込み SIM デバイスの状態が作成された時刻。</span><span class="sxs-lookup"><span data-stu-id="c8c76-138">The time the embedded SIM device status was created.</span></span> <span data-ttu-id="c8c76-139">サービス側を生成しました。</span><span class="sxs-lookup"><span data-stu-id="c8c76-139">Generated service side.</span></span>|
|<span data-ttu-id="c8c76-140">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c8c76-140">modifiedDateTime</span></span>|<span data-ttu-id="c8c76-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c8c76-141">DateTimeOffset</span></span>|<span data-ttu-id="c8c76-142">埋め込み SIM デバイスの状態が最後に変更された時刻。</span><span class="sxs-lookup"><span data-stu-id="c8c76-142">The time the embedded SIM device status was last modified.</span></span> <span data-ttu-id="c8c76-143">サービス側を更新しました。</span><span class="sxs-lookup"><span data-stu-id="c8c76-143">Updated service side.</span></span>|
|<span data-ttu-id="c8c76-144">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="c8c76-144">lastSyncDateTime</span></span>|<span data-ttu-id="c8c76-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c8c76-145">DateTimeOffset</span></span>|<span data-ttu-id="c8c76-146">埋め込まれた SIM デバイスが最後にチェックインされた時刻。</span><span class="sxs-lookup"><span data-stu-id="c8c76-146">The time the embedded SIM device last checked in.</span></span> <span data-ttu-id="c8c76-147">サービス側を更新しました。</span><span class="sxs-lookup"><span data-stu-id="c8c76-147">Updated service side.</span></span>|
|<span data-ttu-id="c8c76-148">universalIntegratedCircuitCardIdentifier</span><span class="sxs-lookup"><span data-stu-id="c8c76-148">universalIntegratedCircuitCardIdentifier</span></span>|<span data-ttu-id="c8c76-149">文字列</span><span class="sxs-lookup"><span data-stu-id="c8c76-149">String</span></span>|<span data-ttu-id="c8c76-150">プロファイルが展開されるハードウェアを識別するユニバーサル統合回路カード識別子 (UICCID)。</span><span class="sxs-lookup"><span data-stu-id="c8c76-150">The Universal Integrated Circuit Card Identifier (UICCID) identifying the hardware onto which a profile is to be deployed.</span></span>|
|<span data-ttu-id="c8c76-151">deviceName</span><span class="sxs-lookup"><span data-stu-id="c8c76-151">deviceName</span></span>|<span data-ttu-id="c8c76-152">文字列</span><span class="sxs-lookup"><span data-stu-id="c8c76-152">String</span></span>|<span data-ttu-id="c8c76-153">サブスクリプションが準備されたデバイス名 (デスクトップの例: JOE)</span><span class="sxs-lookup"><span data-stu-id="c8c76-153">Device name to which the subscription was provisioned e.g. DESKTOP-JOE</span></span>|
|<span data-ttu-id="c8c76-154">userName</span><span class="sxs-lookup"><span data-stu-id="c8c76-154">userName</span></span>|<span data-ttu-id="c8c76-155">String</span><span class="sxs-lookup"><span data-stu-id="c8c76-155">String</span></span>|<span data-ttu-id="c8c76-156">サブスクリプションが準備されたユーザー名 (例:)joe@contoso.com</span><span class="sxs-lookup"><span data-stu-id="c8c76-156">Username which the subscription was provisioned to e.g. joe@contoso.com</span></span>|
|<span data-ttu-id="c8c76-157">state</span><span class="sxs-lookup"><span data-stu-id="c8c76-157">state</span></span>|[<span data-ttu-id="c8c76-158">embeddedSIMDeviceStateValue</span><span class="sxs-lookup"><span data-stu-id="c8c76-158">embeddedSIMDeviceStateValue</span></span>](../resources/intune-esim-embeddedsimdevicestatevalue.md)|<span data-ttu-id="c8c76-159">デバイスに適用されるプロファイル操作の状態。</span><span class="sxs-lookup"><span data-stu-id="c8c76-159">The state of the profile operation applied to the device.</span></span> <span data-ttu-id="c8c76-160">可能な値は、`notEvaluated`、`failed`、`installing`、`installed`、`deleting`、`error`、`deleted`、`removedByUser` です。</span><span class="sxs-lookup"><span data-stu-id="c8c76-160">Possible values are: `notEvaluated`, `failed`, `installing`, `installed`, `deleting`, `error`, `deleted`, `removedByUser`.</span></span>|
|<span data-ttu-id="c8c76-161">statedetails</span><span class="sxs-lookup"><span data-stu-id="c8c76-161">stateDetails</span></span>|<span data-ttu-id="c8c76-162">文字列</span><span class="sxs-lookup"><span data-stu-id="c8c76-162">String</span></span>|<span data-ttu-id="c8c76-163">プロビジョニング状態の文字列の説明。</span><span class="sxs-lookup"><span data-stu-id="c8c76-163">String description of the provisioning state.</span></span>|



## <a name="response"></a><span data-ttu-id="c8c76-164">応答</span><span class="sxs-lookup"><span data-stu-id="c8c76-164">Response</span></span>
<span data-ttu-id="c8c76-165">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="c8c76-165">If successful, this method returns a `201 Created` response code and a [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c8c76-166">例</span><span class="sxs-lookup"><span data-stu-id="c8c76-166">Example</span></span>

### <a name="request"></a><span data-ttu-id="c8c76-167">要求</span><span class="sxs-lookup"><span data-stu-id="c8c76-167">Request</span></span>
<span data-ttu-id="c8c76-168">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c8c76-168">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/deviceStates
Content-type: application/json
Content-length: 361

{
  "@odata.type": "#microsoft.graph.embeddedSIMDeviceState",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "universalIntegratedCircuitCardIdentifier": "Universal Integrated Circuit Card Identifier value",
  "deviceName": "Device Name value",
  "userName": "User Name value",
  "state": "failed",
  "stateDetails": "State Details value"
}
```

### <a name="response"></a><span data-ttu-id="c8c76-169">応答</span><span class="sxs-lookup"><span data-stu-id="c8c76-169">Response</span></span>
<span data-ttu-id="c8c76-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c8c76-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 529

{
  "@odata.type": "#microsoft.graph.embeddedSIMDeviceState",
  "id": "908884a3-84a3-9088-a384-8890a3848890",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "universalIntegratedCircuitCardIdentifier": "Universal Integrated Circuit Card Identifier value",
  "deviceName": "Device Name value",
  "userName": "User Name value",
  "state": "failed",
  "stateDetails": "State Details value"
}
```





