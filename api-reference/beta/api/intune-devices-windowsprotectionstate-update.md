---
title: WindowsProtectionState を更新します。
description: WindowsProtectionState オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 97a11b8a3a26bea6f59cf0791bc8f5356f6fdb85
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27886871"
---
# <a name="update-windowsprotectionstate"></a><span data-ttu-id="4acc5-103">WindowsProtectionState を更新します。</span><span class="sxs-lookup"><span data-stu-id="4acc5-103">Update windowsProtectionState</span></span>

> <span data-ttu-id="4acc5-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="4acc5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4acc5-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4acc5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4acc5-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="4acc5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4acc5-107">[WindowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="4acc5-107">Update the properties of a [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4acc5-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="4acc5-108">Prerequisites</span></span>
<span data-ttu-id="4acc5-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4acc5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4acc5-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4acc5-111">Permission type</span></span>|<span data-ttu-id="4acc5-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="4acc5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4acc5-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4acc5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4acc5-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4acc5-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="4acc5-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4acc5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4acc5-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4acc5-116">Not supported.</span></span>|
|<span data-ttu-id="4acc5-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4acc5-117">Application</span></span>|<span data-ttu-id="4acc5-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4acc5-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4acc5-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4acc5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsMalwareInformation/{windowsMalwareInformationId}/windowsDevicesProtectionState/{windowsProtectionStateId}
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/windowsProtectionState
```

## <a name="request-headers"></a><span data-ttu-id="4acc5-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4acc5-120">Request headers</span></span>
|<span data-ttu-id="4acc5-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4acc5-121">Header</span></span>|<span data-ttu-id="4acc5-122">値</span><span class="sxs-lookup"><span data-stu-id="4acc5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4acc5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4acc5-123">Authorization</span></span>|<span data-ttu-id="4acc5-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="4acc5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4acc5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4acc5-125">Accept</span></span>|<span data-ttu-id="4acc5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4acc5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4acc5-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="4acc5-127">Request body</span></span>
<span data-ttu-id="4acc5-128">要求の本文に[windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="4acc5-128">In the request body, supply a JSON representation for the [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object.</span></span>

<span data-ttu-id="4acc5-129">[WindowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="4acc5-129">The following table shows the properties that are required when you create the [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md).</span></span>

|<span data-ttu-id="4acc5-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4acc5-130">Property</span></span>|<span data-ttu-id="4acc5-131">種類</span><span class="sxs-lookup"><span data-stu-id="4acc5-131">Type</span></span>|<span data-ttu-id="4acc5-132">説明</span><span class="sxs-lookup"><span data-stu-id="4acc5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4acc5-133">ID</span><span class="sxs-lookup"><span data-stu-id="4acc5-133">id</span></span>|<span data-ttu-id="4acc5-134">String</span><span class="sxs-lookup"><span data-stu-id="4acc5-134">String</span></span>|<span data-ttu-id="4acc5-135">デバイス保護の状態のオブジェクトの一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="4acc5-135">The unique Identifier for the device protection status object.</span></span> <span data-ttu-id="4acc5-136">これは、デバイスのデバイス id</span><span class="sxs-lookup"><span data-stu-id="4acc5-136">This is device id of the device</span></span>|
|<span data-ttu-id="4acc5-137">malwareProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="4acc5-137">malwareProtectionEnabled</span></span>|<span data-ttu-id="4acc5-138">ブール型</span><span class="sxs-lookup"><span data-stu-id="4acc5-138">Boolean</span></span>|<span data-ttu-id="4acc5-139">マルウェア対策が有効になっているか</span><span class="sxs-lookup"><span data-stu-id="4acc5-139">Anti malware is enabled or not</span></span>|
|<span data-ttu-id="4acc5-140">deviceState</span><span class="sxs-lookup"><span data-stu-id="4acc5-140">deviceState</span></span>|[<span data-ttu-id="4acc5-141">windowsDeviceHealthState</span><span class="sxs-lookup"><span data-stu-id="4acc5-141">windowsDeviceHealthState</span></span>](../resources/intune-devices-windowsdevicehealthstate.md)|<span data-ttu-id="4acc5-142">コンピューターの状態 (などのクリーンな保留中の完全なスキャンまたは再起動の保留中など)。</span><span class="sxs-lookup"><span data-stu-id="4acc5-142">Computer's state (like clean or pending full scan or pending reboot etc).</span></span> <span data-ttu-id="4acc5-143">使用可能な値: `clean`、`fullScanPending`、`rebootPending`、`manualStepsPending`、`offlineScanPending`、`critical`。</span><span class="sxs-lookup"><span data-stu-id="4acc5-143">Possible values are: `clean`, `fullScanPending`, `rebootPending`, `manualStepsPending`, `offlineScanPending`, `critical`.</span></span>|
|<span data-ttu-id="4acc5-144">realTimeProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="4acc5-144">realTimeProtectionEnabled</span></span>|<span data-ttu-id="4acc5-145">ブール型</span><span class="sxs-lookup"><span data-stu-id="4acc5-145">Boolean</span></span>|<span data-ttu-id="4acc5-146">リアルタイム保護を有効または無効ですか。</span><span class="sxs-lookup"><span data-stu-id="4acc5-146">Real time protection is enabled or not?</span></span>|
|<span data-ttu-id="4acc5-147">networkInspectionSystemEnabled</span><span class="sxs-lookup"><span data-stu-id="4acc5-147">networkInspectionSystemEnabled</span></span>|<span data-ttu-id="4acc5-148">ブール型</span><span class="sxs-lookup"><span data-stu-id="4acc5-148">Boolean</span></span>|<span data-ttu-id="4acc5-149">ネットワーク検査システムが有効か無効か。</span><span class="sxs-lookup"><span data-stu-id="4acc5-149">Network inspection system enabled or not?</span></span>|
|<span data-ttu-id="4acc5-150">quickScanOverdue</span><span class="sxs-lookup"><span data-stu-id="4acc5-150">quickScanOverdue</span></span>|<span data-ttu-id="4acc5-151">ブール型</span><span class="sxs-lookup"><span data-stu-id="4acc5-151">Boolean</span></span>|<span data-ttu-id="4acc5-152">クイック スキャン、か期限切れですか。</span><span class="sxs-lookup"><span data-stu-id="4acc5-152">Quick scan overdue or not?</span></span>|
|<span data-ttu-id="4acc5-153">fullScanOverdue</span><span class="sxs-lookup"><span data-stu-id="4acc5-153">fullScanOverdue</span></span>|<span data-ttu-id="4acc5-154">ブール型</span><span class="sxs-lookup"><span data-stu-id="4acc5-154">Boolean</span></span>|<span data-ttu-id="4acc5-155">完全なスキャンの期限切れかどうでしょうか。</span><span class="sxs-lookup"><span data-stu-id="4acc5-155">Full scan overdue or not?</span></span>|
|<span data-ttu-id="4acc5-156">signatureUpdateOverdue</span><span class="sxs-lookup"><span data-stu-id="4acc5-156">signatureUpdateOverdue</span></span>|<span data-ttu-id="4acc5-157">ブール型</span><span class="sxs-lookup"><span data-stu-id="4acc5-157">Boolean</span></span>|<span data-ttu-id="4acc5-158">署名が期限切れかどうか。</span><span class="sxs-lookup"><span data-stu-id="4acc5-158">Signature out of date or not?</span></span>|
|<span data-ttu-id="4acc5-159">rebootRequired</span><span class="sxs-lookup"><span data-stu-id="4acc5-159">rebootRequired</span></span>|<span data-ttu-id="4acc5-160">ブール型</span><span class="sxs-lookup"><span data-stu-id="4acc5-160">Boolean</span></span>|<span data-ttu-id="4acc5-161">しましたか。</span><span class="sxs-lookup"><span data-stu-id="4acc5-161">Reboot required or not?</span></span>|
|<span data-ttu-id="4acc5-162">fullScanRequired</span><span class="sxs-lookup"><span data-stu-id="4acc5-162">fullScanRequired</span></span>|<span data-ttu-id="4acc5-163">ブール型</span><span class="sxs-lookup"><span data-stu-id="4acc5-163">Boolean</span></span>|<span data-ttu-id="4acc5-164">全体を走査するかが必要でしょうか。</span><span class="sxs-lookup"><span data-stu-id="4acc5-164">Full scan required or not?</span></span>|
|<span data-ttu-id="4acc5-165">engineVersion</span><span class="sxs-lookup"><span data-stu-id="4acc5-165">engineVersion</span></span>|<span data-ttu-id="4acc5-166">String</span><span class="sxs-lookup"><span data-stu-id="4acc5-166">String</span></span>|<span data-ttu-id="4acc5-167">現在のエンドポイントの保護エンジンのバージョン</span><span class="sxs-lookup"><span data-stu-id="4acc5-167">Current endpoint protection engine's version</span></span>|
|<span data-ttu-id="4acc5-168">signatureVersion</span><span class="sxs-lookup"><span data-stu-id="4acc5-168">signatureVersion</span></span>|<span data-ttu-id="4acc5-169">String</span><span class="sxs-lookup"><span data-stu-id="4acc5-169">String</span></span>|<span data-ttu-id="4acc5-170">マルウェア定義の現在のバージョン</span><span class="sxs-lookup"><span data-stu-id="4acc5-170">Current malware definitions version</span></span>|
|<span data-ttu-id="4acc5-171">antiMalwareVersion</span><span class="sxs-lookup"><span data-stu-id="4acc5-171">antiMalwareVersion</span></span>|<span data-ttu-id="4acc5-172">String</span><span class="sxs-lookup"><span data-stu-id="4acc5-172">String</span></span>|<span data-ttu-id="4acc5-173">現在のバージョンのマルウェア対策</span><span class="sxs-lookup"><span data-stu-id="4acc5-173">Current anti malware version</span></span>|
|<span data-ttu-id="4acc5-174">lastQuickScanDateTime</span><span class="sxs-lookup"><span data-stu-id="4acc5-174">lastQuickScanDateTime</span></span>|<span data-ttu-id="4acc5-175">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4acc5-175">DateTimeOffset</span></span>|<span data-ttu-id="4acc5-176">最後のクイック スキャンの日時</span><span class="sxs-lookup"><span data-stu-id="4acc5-176">Last quick scan datetime</span></span>|
|<span data-ttu-id="4acc5-177">lastFullScanDateTime</span><span class="sxs-lookup"><span data-stu-id="4acc5-177">lastFullScanDateTime</span></span>|<span data-ttu-id="4acc5-178">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4acc5-178">DateTimeOffset</span></span>|<span data-ttu-id="4acc5-179">最後のクイック スキャンの日時</span><span class="sxs-lookup"><span data-stu-id="4acc5-179">Last quick scan datetime</span></span>|
|<span data-ttu-id="4acc5-180">lastQuickScanSignatureVersion</span><span class="sxs-lookup"><span data-stu-id="4acc5-180">lastQuickScanSignatureVersion</span></span>|<span data-ttu-id="4acc5-181">String</span><span class="sxs-lookup"><span data-stu-id="4acc5-181">String</span></span>|<span data-ttu-id="4acc5-182">最後のクイック スキャンの署名バージョン</span><span class="sxs-lookup"><span data-stu-id="4acc5-182">Last quick scan signature version</span></span>|
|<span data-ttu-id="4acc5-183">lastFullScanSignatureVersion</span><span class="sxs-lookup"><span data-stu-id="4acc5-183">lastFullScanSignatureVersion</span></span>|<span data-ttu-id="4acc5-184">String</span><span class="sxs-lookup"><span data-stu-id="4acc5-184">String</span></span>|<span data-ttu-id="4acc5-185">最後の完全なスキャンの署名バージョン</span><span class="sxs-lookup"><span data-stu-id="4acc5-185">Last full scan signature version</span></span>|
|<span data-ttu-id="4acc5-186">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="4acc5-186">lastReportedDateTime</span></span>|<span data-ttu-id="4acc5-187">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4acc5-187">DateTimeOffset</span></span>|<span data-ttu-id="4acc5-188">最後のデバイスの状態が報告された時間</span><span class="sxs-lookup"><span data-stu-id="4acc5-188">Last device health status reported time</span></span>|



## <a name="response"></a><span data-ttu-id="4acc5-189">応答</span><span class="sxs-lookup"><span data-stu-id="4acc5-189">Response</span></span>
<span data-ttu-id="4acc5-190">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="4acc5-190">If successful, this method returns a `200 OK` response code and an updated [windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4acc5-191">例</span><span class="sxs-lookup"><span data-stu-id="4acc5-191">Example</span></span>
### <a name="request"></a><span data-ttu-id="4acc5-192">要求</span><span class="sxs-lookup"><span data-stu-id="4acc5-192">Request</span></span>
<span data-ttu-id="4acc5-193">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4acc5-193">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4acc5-194">応答</span><span class="sxs-lookup"><span data-stu-id="4acc5-194">Response</span></span>
<span data-ttu-id="4acc5-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="4acc5-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





