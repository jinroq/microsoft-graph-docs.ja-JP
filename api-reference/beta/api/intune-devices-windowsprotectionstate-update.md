---
title: WindowsProtectionState を更新します。
description: WindowsProtectionState オブジェクトのプロパティを更新します。
ms.openlocfilehash: f1323baa9a6611e5f6057456fbbefbaddefa626e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071888"
---
# <a name="update-windowsprotectionstate"></a><span data-ttu-id="fca7e-103">WindowsProtectionState を更新します。</span><span class="sxs-lookup"><span data-stu-id="fca7e-103">Update windowsProtectionState</span></span>

> <span data-ttu-id="fca7e-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="fca7e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fca7e-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fca7e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fca7e-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="fca7e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fca7e-107">[WindowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="fca7e-107">Update the properties of a [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fca7e-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="fca7e-108">Prerequisites</span></span>
<span data-ttu-id="fca7e-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fca7e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fca7e-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="fca7e-111">Permission type</span></span>|<span data-ttu-id="fca7e-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="fca7e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fca7e-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="fca7e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fca7e-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fca7e-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="fca7e-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="fca7e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fca7e-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fca7e-116">Not supported.</span></span>|
|<span data-ttu-id="fca7e-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="fca7e-117">Application</span></span>|<span data-ttu-id="fca7e-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fca7e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fca7e-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="fca7e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsMalwareInformation/{windowsMalwareInformationId}/windowsDevicesProtectionState/{windowsProtectionStateId}
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/windowsProtectionState
```

## <a name="request-headers"></a><span data-ttu-id="fca7e-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fca7e-120">Request headers</span></span>
|<span data-ttu-id="fca7e-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fca7e-121">Header</span></span>|<span data-ttu-id="fca7e-122">値</span><span class="sxs-lookup"><span data-stu-id="fca7e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fca7e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fca7e-123">Authorization</span></span>|<span data-ttu-id="fca7e-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="fca7e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fca7e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="fca7e-125">Accept</span></span>|<span data-ttu-id="fca7e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fca7e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fca7e-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="fca7e-127">Request body</span></span>
<span data-ttu-id="fca7e-128">要求の本文に[windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="fca7e-128">In the request body, supply a JSON representation for the [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>

<span data-ttu-id="fca7e-129">[WindowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="fca7e-129">The following table shows the properties that are required when you create the [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md).</span></span>

|<span data-ttu-id="fca7e-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fca7e-130">Property</span></span>|<span data-ttu-id="fca7e-131">型</span><span class="sxs-lookup"><span data-stu-id="fca7e-131">Type</span></span>|<span data-ttu-id="fca7e-132">説明</span><span class="sxs-lookup"><span data-stu-id="fca7e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fca7e-133">id</span><span class="sxs-lookup"><span data-stu-id="fca7e-133">id</span></span>|<span data-ttu-id="fca7e-134">String</span><span class="sxs-lookup"><span data-stu-id="fca7e-134">String</span></span>|<span data-ttu-id="fca7e-135">デバイス保護の状態のオブジェクトの一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="fca7e-135">The unique Identifier for the device protection status object.</span></span> <span data-ttu-id="fca7e-136">これは、デバイスのデバイス id</span><span class="sxs-lookup"><span data-stu-id="fca7e-136">This is device id of the device</span></span>|
|<span data-ttu-id="fca7e-137">malwareProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="fca7e-137">malwareProtectionEnabled</span></span>|<span data-ttu-id="fca7e-138">ブール値</span><span class="sxs-lookup"><span data-stu-id="fca7e-138">Boolean</span></span>|<span data-ttu-id="fca7e-139">マルウェア対策が有効になっているか</span><span class="sxs-lookup"><span data-stu-id="fca7e-139">Anti malware is enabled or not</span></span>|
|<span data-ttu-id="fca7e-140">deviceState</span><span class="sxs-lookup"><span data-stu-id="fca7e-140">deviceState</span></span>|[<span data-ttu-id="fca7e-141">windowsDeviceHealthState</span><span class="sxs-lookup"><span data-stu-id="fca7e-141">windowsDeviceHealthState</span></span>](../resources/intune-devices-windowsdevicehealthstate.md)|<span data-ttu-id="fca7e-142">コンピューターの状態 (などのクリーンな保留中の完全なスキャンまたは再起動の保留中など)。</span><span class="sxs-lookup"><span data-stu-id="fca7e-142">Computer's state (like clean or pending full scan or pending reboot etc).</span></span> <span data-ttu-id="fca7e-143">使用可能な値: `clean`、`fullScanPending`、`rebootPending`、`manualStepsPending`、`offlineScanPending`、`critical`。</span><span class="sxs-lookup"><span data-stu-id="fca7e-143">Possible values are: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.</span></span>|
|<span data-ttu-id="fca7e-144">realTimeProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="fca7e-144">realTimeProtectionEnabled</span></span>|<span data-ttu-id="fca7e-145">ブール値</span><span class="sxs-lookup"><span data-stu-id="fca7e-145">Boolean</span></span>|<span data-ttu-id="fca7e-146">リアルタイム保護を有効または無効ですか。</span><span class="sxs-lookup"><span data-stu-id="fca7e-146">Real time protection is enabled or not?</span></span>|
|<span data-ttu-id="fca7e-147">networkInspectionSystemEnabled</span><span class="sxs-lookup"><span data-stu-id="fca7e-147">networkInspectionSystemEnabled</span></span>|<span data-ttu-id="fca7e-148">ブール値</span><span class="sxs-lookup"><span data-stu-id="fca7e-148">Boolean</span></span>|<span data-ttu-id="fca7e-149">ネットワーク検査システムが有効か無効か。</span><span class="sxs-lookup"><span data-stu-id="fca7e-149">Network inspection system enabled or not?</span></span>|
|<span data-ttu-id="fca7e-150">quickScanOverdue</span><span class="sxs-lookup"><span data-stu-id="fca7e-150">quickScanOverdue</span></span>|<span data-ttu-id="fca7e-151">ブール値</span><span class="sxs-lookup"><span data-stu-id="fca7e-151">Boolean</span></span>|<span data-ttu-id="fca7e-152">クイック スキャン、か期限切れですか。</span><span class="sxs-lookup"><span data-stu-id="fca7e-152">Quick scan overdue or not?</span></span>|
|<span data-ttu-id="fca7e-153">fullScanOverdue</span><span class="sxs-lookup"><span data-stu-id="fca7e-153">fullScanOverdue</span></span>|<span data-ttu-id="fca7e-154">ブール値</span><span class="sxs-lookup"><span data-stu-id="fca7e-154">Boolean</span></span>|<span data-ttu-id="fca7e-155">完全なスキャンの期限切れかどうでしょうか。</span><span class="sxs-lookup"><span data-stu-id="fca7e-155">Full scan overdue or not?</span></span>|
|<span data-ttu-id="fca7e-156">signatureUpdateOverdue</span><span class="sxs-lookup"><span data-stu-id="fca7e-156">signatureUpdateOverdue</span></span>|<span data-ttu-id="fca7e-157">ブール値</span><span class="sxs-lookup"><span data-stu-id="fca7e-157">Boolean</span></span>|<span data-ttu-id="fca7e-158">署名が期限切れかどうか。</span><span class="sxs-lookup"><span data-stu-id="fca7e-158">Signature out of date or not?</span></span>|
|<span data-ttu-id="fca7e-159">rebootRequired</span><span class="sxs-lookup"><span data-stu-id="fca7e-159">rebootRequired</span></span>|<span data-ttu-id="fca7e-160">ブール値</span><span class="sxs-lookup"><span data-stu-id="fca7e-160">Boolean</span></span>|<span data-ttu-id="fca7e-161">しましたか。</span><span class="sxs-lookup"><span data-stu-id="fca7e-161">Reboot required or not?</span></span>|
|<span data-ttu-id="fca7e-162">fullScanRequired</span><span class="sxs-lookup"><span data-stu-id="fca7e-162">fullScanRequired</span></span>|<span data-ttu-id="fca7e-163">ブール値</span><span class="sxs-lookup"><span data-stu-id="fca7e-163">Boolean</span></span>|<span data-ttu-id="fca7e-164">全体を走査するかが必要でしょうか。</span><span class="sxs-lookup"><span data-stu-id="fca7e-164">Full scan required or not?</span></span>|
|<span data-ttu-id="fca7e-165">engineVersion</span><span class="sxs-lookup"><span data-stu-id="fca7e-165">engineVersion</span></span>|<span data-ttu-id="fca7e-166">String</span><span class="sxs-lookup"><span data-stu-id="fca7e-166">String</span></span>|<span data-ttu-id="fca7e-167">現在のエンドポイントの保護エンジンのバージョン</span><span class="sxs-lookup"><span data-stu-id="fca7e-167">Current endpoint protection engine's version</span></span>|
|<span data-ttu-id="fca7e-168">signatureVersion</span><span class="sxs-lookup"><span data-stu-id="fca7e-168">signatureVersion</span></span>|<span data-ttu-id="fca7e-169">String</span><span class="sxs-lookup"><span data-stu-id="fca7e-169">String</span></span>|<span data-ttu-id="fca7e-170">マルウェア定義の現在のバージョン</span><span class="sxs-lookup"><span data-stu-id="fca7e-170">Current malware definitions version</span></span>|
|<span data-ttu-id="fca7e-171">antiMalwareVersion</span><span class="sxs-lookup"><span data-stu-id="fca7e-171">antiMalwareVersion</span></span>|<span data-ttu-id="fca7e-172">String</span><span class="sxs-lookup"><span data-stu-id="fca7e-172">String</span></span>|<span data-ttu-id="fca7e-173">現在のバージョンのマルウェア対策</span><span class="sxs-lookup"><span data-stu-id="fca7e-173">Current anti malware version</span></span>|
|<span data-ttu-id="fca7e-174">lastQuickScanDateTime</span><span class="sxs-lookup"><span data-stu-id="fca7e-174">lastQuickScanDateTime</span></span>|<span data-ttu-id="fca7e-175">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fca7e-175">DateTimeOffset</span></span>|<span data-ttu-id="fca7e-176">最後のクイック スキャンの日時</span><span class="sxs-lookup"><span data-stu-id="fca7e-176">Last quick scan datetime</span></span>|
|<span data-ttu-id="fca7e-177">lastFullScanDateTime</span><span class="sxs-lookup"><span data-stu-id="fca7e-177">lastFullScanDateTime</span></span>|<span data-ttu-id="fca7e-178">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fca7e-178">DateTimeOffset</span></span>|<span data-ttu-id="fca7e-179">最後のクイック スキャンの日時</span><span class="sxs-lookup"><span data-stu-id="fca7e-179">Last quick scan datetime</span></span>|
|<span data-ttu-id="fca7e-180">lastQuickScanSignatureVersion</span><span class="sxs-lookup"><span data-stu-id="fca7e-180">lastQuickScanSignatureVersion</span></span>|<span data-ttu-id="fca7e-181">String</span><span class="sxs-lookup"><span data-stu-id="fca7e-181">String</span></span>|<span data-ttu-id="fca7e-182">最後のクイック スキャンの署名バージョン</span><span class="sxs-lookup"><span data-stu-id="fca7e-182">Last quick scan signature version</span></span>|
|<span data-ttu-id="fca7e-183">lastFullScanSignatureVersion</span><span class="sxs-lookup"><span data-stu-id="fca7e-183">lastFullScanSignatureVersion</span></span>|<span data-ttu-id="fca7e-184">String</span><span class="sxs-lookup"><span data-stu-id="fca7e-184">String</span></span>|<span data-ttu-id="fca7e-185">最後の完全なスキャンの署名バージョン</span><span class="sxs-lookup"><span data-stu-id="fca7e-185">Last full scan signature version</span></span>|
|<span data-ttu-id="fca7e-186">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="fca7e-186">lastReportedDateTime</span></span>|<span data-ttu-id="fca7e-187">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fca7e-187">DateTimeOffset</span></span>|<span data-ttu-id="fca7e-188">最後のデバイスの状態が報告された時間</span><span class="sxs-lookup"><span data-stu-id="fca7e-188">Last device health status reported time</span></span>|



## <a name="response"></a><span data-ttu-id="fca7e-189">応答</span><span class="sxs-lookup"><span data-stu-id="fca7e-189">Response</span></span>
<span data-ttu-id="fca7e-190">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="fca7e-190">If successful, this method returns a `200 OK` response code and an updated [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fca7e-191">例</span><span class="sxs-lookup"><span data-stu-id="fca7e-191">Example</span></span>
### <a name="request"></a><span data-ttu-id="fca7e-192">要求</span><span class="sxs-lookup"><span data-stu-id="fca7e-192">Request</span></span>
<span data-ttu-id="fca7e-193">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="fca7e-193">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsMalwareInformation/{windowsMalwareInformationId}/windowsDevicesProtectionState/{windowsProtectionStateId}
Content-type: application/json
Content-length: 804

{
  "malwareProtectionEnabled": true,
  "deviceState": "fullScanPending",
  "realTimeProtectionEnabled": true,
  "networkInspectionSystemEnabled": true,
  "quickScanOverdue": true,
  "fullScanOverdue": true,
  "signatureUpdateOverdue": true,
  "rebootRequired": true,
  "fullScanRequired": true,
  "engineVersion": "Engine Version value",
  "signatureVersion": "Signature Version value",
  "antiMalwareVersion": "Anti Malware Version value",
  "lastQuickScanDateTime": "2016-12-31T23:58:27.5900669-08:00",
  "lastFullScanDateTime": "2017-01-01T00:01:44.9405639-08:00",
  "lastQuickScanSignatureVersion": "Last Quick Scan Signature Version value",
  "lastFullScanSignatureVersion": "Last Full Scan Signature Version value",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00"
}
```

### <a name="response"></a><span data-ttu-id="fca7e-194">応答</span><span class="sxs-lookup"><span data-stu-id="fca7e-194">Response</span></span>
<span data-ttu-id="fca7e-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="fca7e-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 914

{
  "@odata.type": "#microsoft.graph.windowsProtectionState",
  "id": "1ac6ea5a-ea5a-1ac6-5aea-c61a5aeac61a",
  "malwareProtectionEnabled": true,
  "deviceState": "fullScanPending",
  "realTimeProtectionEnabled": true,
  "networkInspectionSystemEnabled": true,
  "quickScanOverdue": true,
  "fullScanOverdue": true,
  "signatureUpdateOverdue": true,
  "rebootRequired": true,
  "fullScanRequired": true,
  "engineVersion": "Engine Version value",
  "signatureVersion": "Signature Version value",
  "antiMalwareVersion": "Anti Malware Version value",
  "lastQuickScanDateTime": "2016-12-31T23:58:27.5900669-08:00",
  "lastFullScanDateTime": "2017-01-01T00:01:44.9405639-08:00",
  "lastQuickScanSignatureVersion": "Last Quick Scan Signature Version value",
  "lastFullScanSignatureVersion": "Last Full Scan Signature Version value",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00"
}
```





