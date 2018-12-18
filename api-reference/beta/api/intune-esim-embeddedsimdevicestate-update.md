---
title: EmbeddedSIMDeviceState を更新します。
description: EmbeddedSIMDeviceState オブジェクトのプロパティを更新します。
author: tfitzmac
ms.openlocfilehash: 7c377199caae31bb45d65f0ad557cb27fb3916b8
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27318523"
---
# <a name="update-embeddedsimdevicestate"></a><span data-ttu-id="cfe79-103">EmbeddedSIMDeviceState を更新します。</span><span class="sxs-lookup"><span data-stu-id="cfe79-103">Update embeddedSIMDeviceState</span></span>

> <span data-ttu-id="cfe79-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="cfe79-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cfe79-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cfe79-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cfe79-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="cfe79-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cfe79-107">[EmbeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="cfe79-107">Update the properties of a [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cfe79-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="cfe79-108">Prerequisites</span></span>
<span data-ttu-id="cfe79-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cfe79-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cfe79-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="cfe79-111">Permission type</span></span>|<span data-ttu-id="cfe79-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="cfe79-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cfe79-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="cfe79-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cfe79-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cfe79-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="cfe79-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="cfe79-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cfe79-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cfe79-116">Not supported.</span></span>|
|<span data-ttu-id="cfe79-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="cfe79-117">Application</span></span>|<span data-ttu-id="cfe79-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cfe79-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cfe79-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="cfe79-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/deviceStates/{embeddedSIMDeviceStateId}
```

## <a name="request-headers"></a><span data-ttu-id="cfe79-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cfe79-120">Request headers</span></span>
|<span data-ttu-id="cfe79-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cfe79-121">Header</span></span>|<span data-ttu-id="cfe79-122">値</span><span class="sxs-lookup"><span data-stu-id="cfe79-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cfe79-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="cfe79-123">Authorization</span></span>|<span data-ttu-id="cfe79-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="cfe79-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cfe79-125">Accept</span><span class="sxs-lookup"><span data-stu-id="cfe79-125">Accept</span></span>|<span data-ttu-id="cfe79-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cfe79-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cfe79-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="cfe79-127">Request body</span></span>
<span data-ttu-id="cfe79-128">要求の本文に[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="cfe79-128">In the request body, supply a JSON representation for the [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) object.</span></span>

<span data-ttu-id="cfe79-129">[EmbeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="cfe79-129">The following table shows the properties that are required when you create the [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md).</span></span>

|<span data-ttu-id="cfe79-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cfe79-130">Property</span></span>|<span data-ttu-id="cfe79-131">種類</span><span class="sxs-lookup"><span data-stu-id="cfe79-131">Type</span></span>|<span data-ttu-id="cfe79-132">説明</span><span class="sxs-lookup"><span data-stu-id="cfe79-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cfe79-133">ID</span><span class="sxs-lookup"><span data-stu-id="cfe79-133">id</span></span>|<span data-ttu-id="cfe79-134">String</span><span class="sxs-lookup"><span data-stu-id="cfe79-134">String</span></span>|<span data-ttu-id="cfe79-135">埋め込みの SIM のデバイスの状態の一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="cfe79-135">Unique identifier for the embedded SIM device status.</span></span> <span data-ttu-id="cfe79-136">システムでは、作成時に割り当てられた値が生成されます。</span><span class="sxs-lookup"><span data-stu-id="cfe79-136">System generated value assigned when created.</span></span>|
|<span data-ttu-id="cfe79-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cfe79-137">createdDateTime</span></span>|<span data-ttu-id="cfe79-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cfe79-138">DateTimeOffset</span></span>|<span data-ttu-id="cfe79-139">埋め込みの SIM のデバイスの状態が作成された時刻。</span><span class="sxs-lookup"><span data-stu-id="cfe79-139">The time the embedded SIM device status was created.</span></span> <span data-ttu-id="cfe79-140">サービス側が生成されます。</span><span class="sxs-lookup"><span data-stu-id="cfe79-140">Generated service side.</span></span>|
|<span data-ttu-id="cfe79-141">変更された日時</span><span class="sxs-lookup"><span data-stu-id="cfe79-141">modifiedDateTime</span></span>|<span data-ttu-id="cfe79-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cfe79-142">DateTimeOffset</span></span>|<span data-ttu-id="cfe79-143">埋め込み SIM デバイスのステータスが最後に修正された時間です。</span><span class="sxs-lookup"><span data-stu-id="cfe79-143">The time the embedded SIM device status was last modified.</span></span> <span data-ttu-id="cfe79-144">サービス側を更新します。</span><span class="sxs-lookup"><span data-stu-id="cfe79-144">Updated service side.</span></span>|
|<span data-ttu-id="cfe79-145">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="cfe79-145">lastSyncDateTime</span></span>|<span data-ttu-id="cfe79-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cfe79-146">DateTimeOffset</span></span>|<span data-ttu-id="cfe79-147">SIM の埋め込みデバイスが最後にチェックインする時間です。</span><span class="sxs-lookup"><span data-stu-id="cfe79-147">The time the embedded SIM device last checked in.</span></span> <span data-ttu-id="cfe79-148">サービス側を更新します。</span><span class="sxs-lookup"><span data-stu-id="cfe79-148">Updated service side.</span></span>|
|<span data-ttu-id="cfe79-149">universalIntegratedCircuitCardIdentifier</span><span class="sxs-lookup"><span data-stu-id="cfe79-149">universalIntegratedCircuitCardIdentifier</span></span>|<span data-ttu-id="cfe79-150">String</span><span class="sxs-lookup"><span data-stu-id="cfe79-150">String</span></span>|<span data-ttu-id="cfe79-151">汎用集積回路カードの識別子 (UICCID) を展開する先となるプロファイルは、ハードウェアを識別します。</span><span class="sxs-lookup"><span data-stu-id="cfe79-151">The Universal Integrated Circuit Card Identifier (UICCID) identifying the hardware onto which a profile is to be deployed.</span></span>|
|<span data-ttu-id="cfe79-152">deviceName</span><span class="sxs-lookup"><span data-stu-id="cfe79-152">deviceName</span></span>|<span data-ttu-id="cfe79-153">String</span><span class="sxs-lookup"><span data-stu-id="cfe79-153">String</span></span>|<span data-ttu-id="cfe79-154">サブスクリプションには、デバイス名などのデスクトップでの準備</span><span class="sxs-lookup"><span data-stu-id="cfe79-154">Device name to which the subscription was provisioned e.g. DESKTOP-JOE</span></span>|
|<span data-ttu-id="cfe79-155">userName</span><span class="sxs-lookup"><span data-stu-id="cfe79-155">userName</span></span>|<span data-ttu-id="cfe79-156">String</span><span class="sxs-lookup"><span data-stu-id="cfe79-156">String</span></span>|<span data-ttu-id="cfe79-157">サブスクリプションが joe@contoso.com などに準備されているユーザー名</span><span class="sxs-lookup"><span data-stu-id="cfe79-157">Username which the subscription was provisioned to e.g. joe@contoso.com</span></span>|
|<span data-ttu-id="cfe79-158">state</span><span class="sxs-lookup"><span data-stu-id="cfe79-158">state</span></span>|[<span data-ttu-id="cfe79-159">embeddedSIMDeviceStateValue</span><span class="sxs-lookup"><span data-stu-id="cfe79-159">embeddedSIMDeviceStateValue</span></span>](../resources/intune-esim-embeddedsimdevicestatevalue.md)|<span data-ttu-id="cfe79-160">デバイスに適用されるプロファイルの操作の状態。</span><span class="sxs-lookup"><span data-stu-id="cfe79-160">The state of the profile operation applied to the device.</span></span> <span data-ttu-id="cfe79-161">可能な値は、`notEvaluated`、`failed`、`installing`、`installed`、`deleting`、`error`、`deleted`、`removedByUser` です。</span><span class="sxs-lookup"><span data-stu-id="cfe79-161">Possible values are: `notEvaluated`, `failed`, `installing`, `installed`, `deleting`, `error`, `deleted`, `removedByUser`.</span></span>|
|<span data-ttu-id="cfe79-162">stateDetails</span><span class="sxs-lookup"><span data-stu-id="cfe79-162">stateDetails</span></span>|<span data-ttu-id="cfe79-163">String</span><span class="sxs-lookup"><span data-stu-id="cfe79-163">String</span></span>|<span data-ttu-id="cfe79-164">プロビジョニングの状態の説明の文字列を指定します。</span><span class="sxs-lookup"><span data-stu-id="cfe79-164">String description of the provisioning state.</span></span>|



## <a name="response"></a><span data-ttu-id="cfe79-165">応答</span><span class="sxs-lookup"><span data-stu-id="cfe79-165">Response</span></span>
<span data-ttu-id="cfe79-166">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="cfe79-166">If successful, this method returns a `200 OK` response code and an updated [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cfe79-167">例</span><span class="sxs-lookup"><span data-stu-id="cfe79-167">Example</span></span>
### <a name="request"></a><span data-ttu-id="cfe79-168">要求</span><span class="sxs-lookup"><span data-stu-id="cfe79-168">Request</span></span>
<span data-ttu-id="cfe79-169">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="cfe79-169">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/deviceStates/{embeddedSIMDeviceStateId}
Content-type: application/json
Content-length: 300

{
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "universalIntegratedCircuitCardIdentifier": "Universal Integrated Circuit Card Identifier value",
  "deviceName": "Device Name value",
  "userName": "User Name value",
  "state": "failed",
  "stateDetails": "State Details value"
}
```

### <a name="response"></a><span data-ttu-id="cfe79-170">応答</span><span class="sxs-lookup"><span data-stu-id="cfe79-170">Response</span></span>
<span data-ttu-id="cfe79-p108">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="cfe79-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





