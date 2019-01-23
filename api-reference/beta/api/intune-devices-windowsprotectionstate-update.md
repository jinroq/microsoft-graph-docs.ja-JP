---
title: WindowsProtectionState を更新します。
description: WindowsProtectionState オブジェクトのプロパティを更新します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: faad744f1a7910b693ea7f87ea0e2ab5dddd7a25
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29406207"
---
# <a name="update-windowsprotectionstate"></a><span data-ttu-id="a36a8-103">WindowsProtectionState を更新します。</span><span class="sxs-lookup"><span data-stu-id="a36a8-103">Update windowsProtectionState</span></span>

> <span data-ttu-id="a36a8-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a36a8-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a36a8-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a36a8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a36a8-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a36a8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a36a8-107">[WindowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="a36a8-107">Update the properties of a [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a36a8-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="a36a8-108">Prerequisites</span></span>
<span data-ttu-id="a36a8-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a36a8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a36a8-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a36a8-111">Permission type</span></span>|<span data-ttu-id="a36a8-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="a36a8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a36a8-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a36a8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a36a8-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a36a8-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="a36a8-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a36a8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a36a8-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a36a8-116">Not supported.</span></span>|
|<span data-ttu-id="a36a8-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a36a8-117">Application</span></span>|<span data-ttu-id="a36a8-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a36a8-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a36a8-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a36a8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsMalwareInformation/{windowsMalwareInformationId}/windowsDevicesProtectionState/{windowsProtectionStateId}
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/windowsProtectionState
```

## <a name="request-headers"></a><span data-ttu-id="a36a8-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a36a8-120">Request headers</span></span>
|<span data-ttu-id="a36a8-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a36a8-121">Header</span></span>|<span data-ttu-id="a36a8-122">値</span><span class="sxs-lookup"><span data-stu-id="a36a8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a36a8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a36a8-123">Authorization</span></span>|<span data-ttu-id="a36a8-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="a36a8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a36a8-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a36a8-125">Accept</span></span>|<span data-ttu-id="a36a8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a36a8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a36a8-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="a36a8-127">Request body</span></span>
<span data-ttu-id="a36a8-128">要求の本文に[windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="a36a8-128">In the request body, supply a JSON representation for the [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>

<span data-ttu-id="a36a8-129">[WindowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="a36a8-129">The following table shows the properties that are required when you create the [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md).</span></span>

|<span data-ttu-id="a36a8-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a36a8-130">Property</span></span>|<span data-ttu-id="a36a8-131">型</span><span class="sxs-lookup"><span data-stu-id="a36a8-131">Type</span></span>|<span data-ttu-id="a36a8-132">説明</span><span class="sxs-lookup"><span data-stu-id="a36a8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a36a8-133">id</span><span class="sxs-lookup"><span data-stu-id="a36a8-133">id</span></span>|<span data-ttu-id="a36a8-134">String</span><span class="sxs-lookup"><span data-stu-id="a36a8-134">String</span></span>|<span data-ttu-id="a36a8-135">デバイス保護の状態のオブジェクトの一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="a36a8-135">The unique Identifier for the device protection status object.</span></span> <span data-ttu-id="a36a8-136">これは、デバイスのデバイス id</span><span class="sxs-lookup"><span data-stu-id="a36a8-136">This is device id of the device</span></span>|
|<span data-ttu-id="a36a8-137">malwareProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="a36a8-137">malwareProtectionEnabled</span></span>|<span data-ttu-id="a36a8-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="a36a8-138">Boolean</span></span>|<span data-ttu-id="a36a8-139">マルウェア対策が有効になっているか</span><span class="sxs-lookup"><span data-stu-id="a36a8-139">Anti malware is enabled or not</span></span>|
|<span data-ttu-id="a36a8-140">deviceState</span><span class="sxs-lookup"><span data-stu-id="a36a8-140">deviceState</span></span>|[<span data-ttu-id="a36a8-141">windowsDeviceHealthState</span><span class="sxs-lookup"><span data-stu-id="a36a8-141">windowsDeviceHealthState</span></span>](../resources/intune-devices-windowsdevicehealthstate.md)|<span data-ttu-id="a36a8-142">コンピューターの状態 (などのクリーンな保留中の完全なスキャンまたは再起動の保留中など)。</span><span class="sxs-lookup"><span data-stu-id="a36a8-142">Computer's state (like clean or pending full scan or pending reboot etc).</span></span> <span data-ttu-id="a36a8-143">使用可能な値: `clean`、`fullScanPending`、`rebootPending`、`manualStepsPending`、`offlineScanPending`、`critical`。</span><span class="sxs-lookup"><span data-stu-id="a36a8-143">Possible values are: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.</span></span>|
|<span data-ttu-id="a36a8-144">realTimeProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="a36a8-144">realTimeProtectionEnabled</span></span>|<span data-ttu-id="a36a8-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="a36a8-145">Boolean</span></span>|<span data-ttu-id="a36a8-146">リアルタイム保護を有効または無効ですか。</span><span class="sxs-lookup"><span data-stu-id="a36a8-146">Real time protection is enabled or not?</span></span>|
|<span data-ttu-id="a36a8-147">networkInspectionSystemEnabled</span><span class="sxs-lookup"><span data-stu-id="a36a8-147">networkInspectionSystemEnabled</span></span>|<span data-ttu-id="a36a8-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="a36a8-148">Boolean</span></span>|<span data-ttu-id="a36a8-149">ネットワーク検査システムが有効か無効か。</span><span class="sxs-lookup"><span data-stu-id="a36a8-149">Network inspection system enabled or not?</span></span>|
|<span data-ttu-id="a36a8-150">quickScanOverdue</span><span class="sxs-lookup"><span data-stu-id="a36a8-150">quickScanOverdue</span></span>|<span data-ttu-id="a36a8-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="a36a8-151">Boolean</span></span>|<span data-ttu-id="a36a8-152">クイック スキャン、か期限切れですか。</span><span class="sxs-lookup"><span data-stu-id="a36a8-152">Quick scan overdue or not?</span></span>|
|<span data-ttu-id="a36a8-153">fullScanOverdue</span><span class="sxs-lookup"><span data-stu-id="a36a8-153">fullScanOverdue</span></span>|<span data-ttu-id="a36a8-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="a36a8-154">Boolean</span></span>|<span data-ttu-id="a36a8-155">完全なスキャンの期限切れかどうでしょうか。</span><span class="sxs-lookup"><span data-stu-id="a36a8-155">Full scan overdue or not?</span></span>|
|<span data-ttu-id="a36a8-156">signatureUpdateOverdue</span><span class="sxs-lookup"><span data-stu-id="a36a8-156">signatureUpdateOverdue</span></span>|<span data-ttu-id="a36a8-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="a36a8-157">Boolean</span></span>|<span data-ttu-id="a36a8-158">署名が期限切れかどうか。</span><span class="sxs-lookup"><span data-stu-id="a36a8-158">Signature out of date or not?</span></span>|
|<span data-ttu-id="a36a8-159">rebootRequired</span><span class="sxs-lookup"><span data-stu-id="a36a8-159">rebootRequired</span></span>|<span data-ttu-id="a36a8-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="a36a8-160">Boolean</span></span>|<span data-ttu-id="a36a8-161">しましたか。</span><span class="sxs-lookup"><span data-stu-id="a36a8-161">Reboot required or not?</span></span>|
|<span data-ttu-id="a36a8-162">fullScanRequired</span><span class="sxs-lookup"><span data-stu-id="a36a8-162">fullScanRequired</span></span>|<span data-ttu-id="a36a8-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="a36a8-163">Boolean</span></span>|<span data-ttu-id="a36a8-164">全体を走査するかが必要でしょうか。</span><span class="sxs-lookup"><span data-stu-id="a36a8-164">Full scan required or not?</span></span>|
|<span data-ttu-id="a36a8-165">engineVersion</span><span class="sxs-lookup"><span data-stu-id="a36a8-165">engineVersion</span></span>|<span data-ttu-id="a36a8-166">String</span><span class="sxs-lookup"><span data-stu-id="a36a8-166">String</span></span>|<span data-ttu-id="a36a8-167">現在のエンドポイントの保護エンジンのバージョン</span><span class="sxs-lookup"><span data-stu-id="a36a8-167">Current endpoint protection engine's version</span></span>|
|<span data-ttu-id="a36a8-168">signatureVersion</span><span class="sxs-lookup"><span data-stu-id="a36a8-168">signatureVersion</span></span>|<span data-ttu-id="a36a8-169">String</span><span class="sxs-lookup"><span data-stu-id="a36a8-169">String</span></span>|<span data-ttu-id="a36a8-170">マルウェア定義の現在のバージョン</span><span class="sxs-lookup"><span data-stu-id="a36a8-170">Current malware definitions version</span></span>|
|<span data-ttu-id="a36a8-171">antiMalwareVersion</span><span class="sxs-lookup"><span data-stu-id="a36a8-171">antiMalwareVersion</span></span>|<span data-ttu-id="a36a8-172">String</span><span class="sxs-lookup"><span data-stu-id="a36a8-172">String</span></span>|<span data-ttu-id="a36a8-173">現在のバージョンのマルウェア対策</span><span class="sxs-lookup"><span data-stu-id="a36a8-173">Current anti malware version</span></span>|
|<span data-ttu-id="a36a8-174">lastQuickScanDateTime</span><span class="sxs-lookup"><span data-stu-id="a36a8-174">lastQuickScanDateTime</span></span>|<span data-ttu-id="a36a8-175">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a36a8-175">DateTimeOffset</span></span>|<span data-ttu-id="a36a8-176">最後のクイック スキャンの日時</span><span class="sxs-lookup"><span data-stu-id="a36a8-176">Last quick scan datetime</span></span>|
|<span data-ttu-id="a36a8-177">lastFullScanDateTime</span><span class="sxs-lookup"><span data-stu-id="a36a8-177">lastFullScanDateTime</span></span>|<span data-ttu-id="a36a8-178">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a36a8-178">DateTimeOffset</span></span>|<span data-ttu-id="a36a8-179">最後のクイック スキャンの日時</span><span class="sxs-lookup"><span data-stu-id="a36a8-179">Last quick scan datetime</span></span>|
|<span data-ttu-id="a36a8-180">lastQuickScanSignatureVersion</span><span class="sxs-lookup"><span data-stu-id="a36a8-180">lastQuickScanSignatureVersion</span></span>|<span data-ttu-id="a36a8-181">String</span><span class="sxs-lookup"><span data-stu-id="a36a8-181">String</span></span>|<span data-ttu-id="a36a8-182">最後のクイック スキャンの署名バージョン</span><span class="sxs-lookup"><span data-stu-id="a36a8-182">Last quick scan signature version</span></span>|
|<span data-ttu-id="a36a8-183">lastFullScanSignatureVersion</span><span class="sxs-lookup"><span data-stu-id="a36a8-183">lastFullScanSignatureVersion</span></span>|<span data-ttu-id="a36a8-184">String</span><span class="sxs-lookup"><span data-stu-id="a36a8-184">String</span></span>|<span data-ttu-id="a36a8-185">最後の完全なスキャンの署名バージョン</span><span class="sxs-lookup"><span data-stu-id="a36a8-185">Last full scan signature version</span></span>|
|<span data-ttu-id="a36a8-186">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="a36a8-186">lastReportedDateTime</span></span>|<span data-ttu-id="a36a8-187">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a36a8-187">DateTimeOffset</span></span>|<span data-ttu-id="a36a8-188">最後のデバイスの状態が報告された時間</span><span class="sxs-lookup"><span data-stu-id="a36a8-188">Last device health status reported time</span></span>|



## <a name="response"></a><span data-ttu-id="a36a8-189">応答</span><span class="sxs-lookup"><span data-stu-id="a36a8-189">Response</span></span>
<span data-ttu-id="a36a8-190">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="a36a8-190">If successful, this method returns a `200 OK` response code and an updated [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a36a8-191">例</span><span class="sxs-lookup"><span data-stu-id="a36a8-191">Example</span></span>

### <a name="request"></a><span data-ttu-id="a36a8-192">要求</span><span class="sxs-lookup"><span data-stu-id="a36a8-192">Request</span></span>
<span data-ttu-id="a36a8-193">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a36a8-193">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsMalwareInformation/{windowsMalwareInformationId}/windowsDevicesProtectionState/{windowsProtectionStateId}
Content-type: application/json
Content-length: 865

{
  "@odata.type": "#microsoft.graph.windowsProtectionState",
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

### <a name="response"></a><span data-ttu-id="a36a8-194">応答</span><span class="sxs-lookup"><span data-stu-id="a36a8-194">Response</span></span>
<span data-ttu-id="a36a8-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a36a8-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




