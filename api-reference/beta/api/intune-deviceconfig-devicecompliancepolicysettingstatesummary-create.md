---
title: deviceCompliancePolicySettingStateSummary の作成
description: 新しい deviceCompliancePolicySettingStateSummary オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b75ab93677f36ff63e3b49679e281b3e2e9f2e25
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27963018"
---
# <a name="create-devicecompliancepolicysettingstatesummary"></a><span data-ttu-id="d4e78-103">deviceCompliancePolicySettingStateSummary の作成</span><span class="sxs-lookup"><span data-stu-id="d4e78-103">Create deviceCompliancePolicySettingStateSummary</span></span>

> <span data-ttu-id="d4e78-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d4e78-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d4e78-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d4e78-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d4e78-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="d4e78-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d4e78-107">新しい [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="d4e78-107">Create a new [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d4e78-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="d4e78-108">Prerequisites</span></span>
<span data-ttu-id="d4e78-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d4e78-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d4e78-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d4e78-111">Permission type</span></span>|<span data-ttu-id="d4e78-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="d4e78-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d4e78-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d4e78-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d4e78-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4e78-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d4e78-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d4e78-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d4e78-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d4e78-116">Not supported.</span></span>|
|<span data-ttu-id="d4e78-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d4e78-117">Application</span></span>|<span data-ttu-id="d4e78-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d4e78-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d4e78-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d4e78-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicySettingStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="d4e78-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d4e78-120">Request headers</span></span>
|<span data-ttu-id="d4e78-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d4e78-121">Header</span></span>|<span data-ttu-id="d4e78-122">値</span><span class="sxs-lookup"><span data-stu-id="d4e78-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d4e78-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d4e78-123">Authorization</span></span>|<span data-ttu-id="d4e78-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="d4e78-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d4e78-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d4e78-125">Accept</span></span>|<span data-ttu-id="d4e78-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d4e78-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d4e78-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="d4e78-127">Request body</span></span>
<span data-ttu-id="d4e78-128">要求本文で、deviceCompliancePolicySettingStateSummary オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="d4e78-128">In the request body, supply a JSON representation for the deviceCompliancePolicySettingStateSummary object.</span></span>

<span data-ttu-id="d4e78-129">次の表に、deviceCompliancePolicySettingStateSummary の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="d4e78-129">The following table shows the properties that are required when you create the deviceCompliancePolicySettingStateSummary.</span></span>

|<span data-ttu-id="d4e78-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d4e78-130">Property</span></span>|<span data-ttu-id="d4e78-131">種類</span><span class="sxs-lookup"><span data-stu-id="d4e78-131">Type</span></span>|<span data-ttu-id="d4e78-132">説明</span><span class="sxs-lookup"><span data-stu-id="d4e78-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d4e78-133">ID</span><span class="sxs-lookup"><span data-stu-id="d4e78-133">id</span></span>|<span data-ttu-id="d4e78-134">String</span><span class="sxs-lookup"><span data-stu-id="d4e78-134">String</span></span>|<span data-ttu-id="d4e78-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="d4e78-135">Key of the entity.</span></span>|
|<span data-ttu-id="d4e78-136">setting</span><span class="sxs-lookup"><span data-stu-id="d4e78-136">setting</span></span>|<span data-ttu-id="d4e78-137">String</span><span class="sxs-lookup"><span data-stu-id="d4e78-137">String</span></span>|<span data-ttu-id="d4e78-138">設定のクラス名とプロパティ名。</span><span class="sxs-lookup"><span data-stu-id="d4e78-138">The setting class name and property name.</span></span>|
|<span data-ttu-id="d4e78-139">settingName</span><span class="sxs-lookup"><span data-stu-id="d4e78-139">settingName</span></span>|<span data-ttu-id="d4e78-140">String</span><span class="sxs-lookup"><span data-stu-id="d4e78-140">String</span></span>|<span data-ttu-id="d4e78-141">設定の名前。</span><span class="sxs-lookup"><span data-stu-id="d4e78-141">Name of the setting.</span></span>|
|<span data-ttu-id="d4e78-142">platformType</span><span class="sxs-lookup"><span data-stu-id="d4e78-142">platformType</span></span>|[<span data-ttu-id="d4e78-143">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="d4e78-143">policyPlatformType</span></span>](../resources/intune-deviceconfig-policyplatformtype.md)|<span data-ttu-id="d4e78-144">設定のプラットフォームです。</span><span class="sxs-lookup"><span data-stu-id="d4e78-144">Setting platform.</span></span> <span data-ttu-id="d4e78-145">可能な値は、`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`all` です。</span><span class="sxs-lookup"><span data-stu-id="d4e78-145">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="d4e78-146">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d4e78-146">unknownDeviceCount</span></span>|<span data-ttu-id="d4e78-147">Int32</span><span class="sxs-lookup"><span data-stu-id="d4e78-147">Int32</span></span>|<span data-ttu-id="d4e78-148">不明なデバイスの数</span><span class="sxs-lookup"><span data-stu-id="d4e78-148">Number of unknown devices</span></span>|
|<span data-ttu-id="d4e78-149">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d4e78-149">notApplicableDeviceCount</span></span>|<span data-ttu-id="d4e78-150">Int32</span><span class="sxs-lookup"><span data-stu-id="d4e78-150">Int32</span></span>|<span data-ttu-id="d4e78-151">該当しないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="d4e78-151">Number of not applicable devices</span></span>|
|<span data-ttu-id="d4e78-152">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d4e78-152">compliantDeviceCount</span></span>|<span data-ttu-id="d4e78-153">Int32</span><span class="sxs-lookup"><span data-stu-id="d4e78-153">Int32</span></span>|<span data-ttu-id="d4e78-154">準拠デバイスの数</span><span class="sxs-lookup"><span data-stu-id="d4e78-154">Number of compliant devices</span></span>|
|<span data-ttu-id="d4e78-155">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d4e78-155">remediatedDeviceCount</span></span>|<span data-ttu-id="d4e78-156">Int32</span><span class="sxs-lookup"><span data-stu-id="d4e78-156">Int32</span></span>|<span data-ttu-id="d4e78-157">修復済みデバイスの数</span><span class="sxs-lookup"><span data-stu-id="d4e78-157">Number of remediated devices</span></span>|
|<span data-ttu-id="d4e78-158">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d4e78-158">nonCompliantDeviceCount</span></span>|<span data-ttu-id="d4e78-159">Int32</span><span class="sxs-lookup"><span data-stu-id="d4e78-159">Int32</span></span>|<span data-ttu-id="d4e78-160">準拠していないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="d4e78-160">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="d4e78-161">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d4e78-161">errorDeviceCount</span></span>|<span data-ttu-id="d4e78-162">Int32</span><span class="sxs-lookup"><span data-stu-id="d4e78-162">Int32</span></span>|<span data-ttu-id="d4e78-163">エラー デバイスの数</span><span class="sxs-lookup"><span data-stu-id="d4e78-163">Number of error devices</span></span>|
|<span data-ttu-id="d4e78-164">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d4e78-164">conflictDeviceCount</span></span>|<span data-ttu-id="d4e78-165">Int32</span><span class="sxs-lookup"><span data-stu-id="d4e78-165">Int32</span></span>|<span data-ttu-id="d4e78-166">競合デバイスの数</span><span class="sxs-lookup"><span data-stu-id="d4e78-166">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="d4e78-167">応答</span><span class="sxs-lookup"><span data-stu-id="d4e78-167">Response</span></span>
<span data-ttu-id="d4e78-168">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="d4e78-168">If successful, this method returns a `201 Created` response code and a [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d4e78-169">例</span><span class="sxs-lookup"><span data-stu-id="d4e78-169">Example</span></span>
### <a name="request"></a><span data-ttu-id="d4e78-170">要求</span><span class="sxs-lookup"><span data-stu-id="d4e78-170">Request</span></span>
<span data-ttu-id="d4e78-171">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d4e78-171">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicySettingStateSummaries
Content-type: application/json
Content-length: 402

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicySettingStateSummary",
  "setting": "Setting value",
  "settingName": "Setting Name value",
  "platformType": "androidForWork",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```

### <a name="response"></a><span data-ttu-id="d4e78-172">応答</span><span class="sxs-lookup"><span data-stu-id="d4e78-172">Response</span></span>
<span data-ttu-id="d4e78-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d4e78-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 451

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicySettingStateSummary",
  "id": "7474d6d5-d6d5-7474-d5d6-7474d5d67474",
  "setting": "Setting value",
  "settingName": "Setting Name value",
  "platformType": "androidForWork",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```





