---
title: deviceCompliancePolicySettingStateSummary の作成
description: 新しい deviceCompliancePolicySettingStateSummary オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c5c022460b744345eac048be24751fbdb6f510f7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35949735"
---
# <a name="create-devicecompliancepolicysettingstatesummary"></a><span data-ttu-id="bb13b-103">deviceCompliancePolicySettingStateSummary の作成</span><span class="sxs-lookup"><span data-stu-id="bb13b-103">Create deviceCompliancePolicySettingStateSummary</span></span>

> <span data-ttu-id="bb13b-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bb13b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bb13b-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="bb13b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bb13b-106">新しい [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="bb13b-106">Create a new [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bb13b-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="bb13b-107">Prerequisites</span></span>
<span data-ttu-id="bb13b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bb13b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bb13b-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="bb13b-110">Permission type</span></span>|<span data-ttu-id="bb13b-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="bb13b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bb13b-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="bb13b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bb13b-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb13b-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bb13b-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="bb13b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bb13b-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bb13b-115">Not supported.</span></span>|
|<span data-ttu-id="bb13b-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="bb13b-116">Application</span></span>|<span data-ttu-id="bb13b-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bb13b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bb13b-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="bb13b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicySettingStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="bb13b-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bb13b-119">Request headers</span></span>
|<span data-ttu-id="bb13b-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bb13b-120">Header</span></span>|<span data-ttu-id="bb13b-121">値</span><span class="sxs-lookup"><span data-stu-id="bb13b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bb13b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="bb13b-122">Authorization</span></span>|<span data-ttu-id="bb13b-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="bb13b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bb13b-124">承諾</span><span class="sxs-lookup"><span data-stu-id="bb13b-124">Accept</span></span>|<span data-ttu-id="bb13b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="bb13b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bb13b-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="bb13b-126">Request body</span></span>
<span data-ttu-id="bb13b-127">要求本文で、deviceCompliancePolicySettingStateSummary オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="bb13b-127">In the request body, supply a JSON representation for the deviceCompliancePolicySettingStateSummary object.</span></span>

<span data-ttu-id="bb13b-128">次の表に、deviceCompliancePolicySettingStateSummary の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="bb13b-128">The following table shows the properties that are required when you create the deviceCompliancePolicySettingStateSummary.</span></span>

|<span data-ttu-id="bb13b-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bb13b-129">Property</span></span>|<span data-ttu-id="bb13b-130">型</span><span class="sxs-lookup"><span data-stu-id="bb13b-130">Type</span></span>|<span data-ttu-id="bb13b-131">説明</span><span class="sxs-lookup"><span data-stu-id="bb13b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb13b-132">id</span><span class="sxs-lookup"><span data-stu-id="bb13b-132">id</span></span>|<span data-ttu-id="bb13b-133">String</span><span class="sxs-lookup"><span data-stu-id="bb13b-133">String</span></span>|<span data-ttu-id="bb13b-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="bb13b-134">Key of the entity.</span></span>|
|<span data-ttu-id="bb13b-135">setting</span><span class="sxs-lookup"><span data-stu-id="bb13b-135">setting</span></span>|<span data-ttu-id="bb13b-136">String</span><span class="sxs-lookup"><span data-stu-id="bb13b-136">String</span></span>|<span data-ttu-id="bb13b-137">設定のクラス名とプロパティ名。</span><span class="sxs-lookup"><span data-stu-id="bb13b-137">The setting class name and property name.</span></span>|
|<span data-ttu-id="bb13b-138">settingName</span><span class="sxs-lookup"><span data-stu-id="bb13b-138">settingName</span></span>|<span data-ttu-id="bb13b-139">String</span><span class="sxs-lookup"><span data-stu-id="bb13b-139">String</span></span>|<span data-ttu-id="bb13b-140">設定の名前。</span><span class="sxs-lookup"><span data-stu-id="bb13b-140">Name of the setting.</span></span>|
|<span data-ttu-id="bb13b-141">platformType</span><span class="sxs-lookup"><span data-stu-id="bb13b-141">platformType</span></span>|[<span data-ttu-id="bb13b-142">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="bb13b-142">policyPlatformType</span></span>](../resources/intune-deviceconfig-policyplatformtype.md)|<span data-ttu-id="bb13b-143">プラットフォームを設定します。</span><span class="sxs-lookup"><span data-stu-id="bb13b-143">Setting platform.</span></span> <span data-ttu-id="bb13b-144">可能な値は、`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`all` です。</span><span class="sxs-lookup"><span data-stu-id="bb13b-144">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="bb13b-145">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="bb13b-145">unknownDeviceCount</span></span>|<span data-ttu-id="bb13b-146">Int32</span><span class="sxs-lookup"><span data-stu-id="bb13b-146">Int32</span></span>|<span data-ttu-id="bb13b-147">不明なデバイスの数</span><span class="sxs-lookup"><span data-stu-id="bb13b-147">Number of unknown devices</span></span>|
|<span data-ttu-id="bb13b-148">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="bb13b-148">notApplicableDeviceCount</span></span>|<span data-ttu-id="bb13b-149">Int32</span><span class="sxs-lookup"><span data-stu-id="bb13b-149">Int32</span></span>|<span data-ttu-id="bb13b-150">該当しないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="bb13b-150">Number of not applicable devices</span></span>|
|<span data-ttu-id="bb13b-151">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="bb13b-151">compliantDeviceCount</span></span>|<span data-ttu-id="bb13b-152">Int32</span><span class="sxs-lookup"><span data-stu-id="bb13b-152">Int32</span></span>|<span data-ttu-id="bb13b-153">準拠デバイスの数</span><span class="sxs-lookup"><span data-stu-id="bb13b-153">Number of compliant devices</span></span>|
|<span data-ttu-id="bb13b-154">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="bb13b-154">remediatedDeviceCount</span></span>|<span data-ttu-id="bb13b-155">Int32</span><span class="sxs-lookup"><span data-stu-id="bb13b-155">Int32</span></span>|<span data-ttu-id="bb13b-156">修復済みデバイスの数</span><span class="sxs-lookup"><span data-stu-id="bb13b-156">Number of remediated devices</span></span>|
|<span data-ttu-id="bb13b-157">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="bb13b-157">nonCompliantDeviceCount</span></span>|<span data-ttu-id="bb13b-158">Int32</span><span class="sxs-lookup"><span data-stu-id="bb13b-158">Int32</span></span>|<span data-ttu-id="bb13b-159">準拠していないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="bb13b-159">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="bb13b-160">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="bb13b-160">errorDeviceCount</span></span>|<span data-ttu-id="bb13b-161">Int32</span><span class="sxs-lookup"><span data-stu-id="bb13b-161">Int32</span></span>|<span data-ttu-id="bb13b-162">エラー デバイスの数</span><span class="sxs-lookup"><span data-stu-id="bb13b-162">Number of error devices</span></span>|
|<span data-ttu-id="bb13b-163">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="bb13b-163">conflictDeviceCount</span></span>|<span data-ttu-id="bb13b-164">Int32</span><span class="sxs-lookup"><span data-stu-id="bb13b-164">Int32</span></span>|<span data-ttu-id="bb13b-165">競合デバイスの数</span><span class="sxs-lookup"><span data-stu-id="bb13b-165">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="bb13b-166">応答</span><span class="sxs-lookup"><span data-stu-id="bb13b-166">Response</span></span>
<span data-ttu-id="bb13b-167">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="bb13b-167">If successful, this method returns a `201 Created` response code and a [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bb13b-168">例</span><span class="sxs-lookup"><span data-stu-id="bb13b-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="bb13b-169">要求</span><span class="sxs-lookup"><span data-stu-id="bb13b-169">Request</span></span>
<span data-ttu-id="bb13b-170">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="bb13b-170">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="bb13b-171">応答</span><span class="sxs-lookup"><span data-stu-id="bb13b-171">Response</span></span>
<span data-ttu-id="bb13b-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="bb13b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





