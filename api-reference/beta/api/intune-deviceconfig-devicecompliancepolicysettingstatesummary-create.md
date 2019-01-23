---
title: deviceCompliancePolicySettingStateSummary の作成
description: 新しい deviceCompliancePolicySettingStateSummary オブジェクトを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 48bbae6e0252e7c0199d84802c71228ccbfebc04
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29414187"
---
# <a name="create-devicecompliancepolicysettingstatesummary"></a><span data-ttu-id="24b46-103">deviceCompliancePolicySettingStateSummary の作成</span><span class="sxs-lookup"><span data-stu-id="24b46-103">Create deviceCompliancePolicySettingStateSummary</span></span>

> <span data-ttu-id="24b46-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="24b46-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="24b46-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="24b46-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="24b46-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="24b46-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="24b46-107">新しい [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="24b46-107">Create a new [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="24b46-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="24b46-108">Prerequisites</span></span>
<span data-ttu-id="24b46-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="24b46-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="24b46-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="24b46-111">Permission type</span></span>|<span data-ttu-id="24b46-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="24b46-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="24b46-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="24b46-113">Delegated (work or school account)</span></span>|<span data-ttu-id="24b46-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="24b46-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="24b46-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="24b46-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="24b46-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="24b46-116">Not supported.</span></span>|
|<span data-ttu-id="24b46-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="24b46-117">Application</span></span>|<span data-ttu-id="24b46-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="24b46-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="24b46-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="24b46-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicySettingStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="24b46-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="24b46-120">Request headers</span></span>
|<span data-ttu-id="24b46-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="24b46-121">Header</span></span>|<span data-ttu-id="24b46-122">値</span><span class="sxs-lookup"><span data-stu-id="24b46-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="24b46-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="24b46-123">Authorization</span></span>|<span data-ttu-id="24b46-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="24b46-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="24b46-125">Accept</span><span class="sxs-lookup"><span data-stu-id="24b46-125">Accept</span></span>|<span data-ttu-id="24b46-126">application/json</span><span class="sxs-lookup"><span data-stu-id="24b46-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="24b46-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="24b46-127">Request body</span></span>
<span data-ttu-id="24b46-128">要求本文で、deviceCompliancePolicySettingStateSummary オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="24b46-128">In the request body, supply a JSON representation for the deviceCompliancePolicySettingStateSummary object.</span></span>

<span data-ttu-id="24b46-129">次の表に、deviceCompliancePolicySettingStateSummary の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="24b46-129">The following table shows the properties that are required when you create the deviceCompliancePolicySettingStateSummary.</span></span>

|<span data-ttu-id="24b46-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="24b46-130">Property</span></span>|<span data-ttu-id="24b46-131">型</span><span class="sxs-lookup"><span data-stu-id="24b46-131">Type</span></span>|<span data-ttu-id="24b46-132">説明</span><span class="sxs-lookup"><span data-stu-id="24b46-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="24b46-133">id</span><span class="sxs-lookup"><span data-stu-id="24b46-133">id</span></span>|<span data-ttu-id="24b46-134">String</span><span class="sxs-lookup"><span data-stu-id="24b46-134">String</span></span>|<span data-ttu-id="24b46-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="24b46-135">Key of the entity.</span></span>|
|<span data-ttu-id="24b46-136">setting</span><span class="sxs-lookup"><span data-stu-id="24b46-136">setting</span></span>|<span data-ttu-id="24b46-137">String</span><span class="sxs-lookup"><span data-stu-id="24b46-137">String</span></span>|<span data-ttu-id="24b46-138">設定のクラス名とプロパティ名。</span><span class="sxs-lookup"><span data-stu-id="24b46-138">The setting class name and property name.</span></span>|
|<span data-ttu-id="24b46-139">settingName</span><span class="sxs-lookup"><span data-stu-id="24b46-139">settingName</span></span>|<span data-ttu-id="24b46-140">String</span><span class="sxs-lookup"><span data-stu-id="24b46-140">String</span></span>|<span data-ttu-id="24b46-141">設定の名前。</span><span class="sxs-lookup"><span data-stu-id="24b46-141">Name of the setting.</span></span>|
|<span data-ttu-id="24b46-142">platformType</span><span class="sxs-lookup"><span data-stu-id="24b46-142">platformType</span></span>|[<span data-ttu-id="24b46-143">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="24b46-143">policyPlatformType</span></span>](../resources/intune-deviceconfig-policyplatformtype.md)|<span data-ttu-id="24b46-144">設定のプラットフォームです。</span><span class="sxs-lookup"><span data-stu-id="24b46-144">Setting platform.</span></span> <span data-ttu-id="24b46-145">可能な値は、`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`all` です。</span><span class="sxs-lookup"><span data-stu-id="24b46-145">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="24b46-146">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="24b46-146">unknownDeviceCount</span></span>|<span data-ttu-id="24b46-147">Int32</span><span class="sxs-lookup"><span data-stu-id="24b46-147">Int32</span></span>|<span data-ttu-id="24b46-148">不明なデバイスの数</span><span class="sxs-lookup"><span data-stu-id="24b46-148">Number of unknown devices</span></span>|
|<span data-ttu-id="24b46-149">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="24b46-149">notApplicableDeviceCount</span></span>|<span data-ttu-id="24b46-150">Int32</span><span class="sxs-lookup"><span data-stu-id="24b46-150">Int32</span></span>|<span data-ttu-id="24b46-151">該当しないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="24b46-151">Number of not applicable devices</span></span>|
|<span data-ttu-id="24b46-152">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="24b46-152">compliantDeviceCount</span></span>|<span data-ttu-id="24b46-153">Int32</span><span class="sxs-lookup"><span data-stu-id="24b46-153">Int32</span></span>|<span data-ttu-id="24b46-154">準拠デバイスの数</span><span class="sxs-lookup"><span data-stu-id="24b46-154">Number of compliant devices</span></span>|
|<span data-ttu-id="24b46-155">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="24b46-155">remediatedDeviceCount</span></span>|<span data-ttu-id="24b46-156">Int32</span><span class="sxs-lookup"><span data-stu-id="24b46-156">Int32</span></span>|<span data-ttu-id="24b46-157">修復済みデバイスの数</span><span class="sxs-lookup"><span data-stu-id="24b46-157">Number of remediated devices</span></span>|
|<span data-ttu-id="24b46-158">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="24b46-158">nonCompliantDeviceCount</span></span>|<span data-ttu-id="24b46-159">Int32</span><span class="sxs-lookup"><span data-stu-id="24b46-159">Int32</span></span>|<span data-ttu-id="24b46-160">準拠していないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="24b46-160">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="24b46-161">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="24b46-161">errorDeviceCount</span></span>|<span data-ttu-id="24b46-162">Int32</span><span class="sxs-lookup"><span data-stu-id="24b46-162">Int32</span></span>|<span data-ttu-id="24b46-163">エラー デバイスの数</span><span class="sxs-lookup"><span data-stu-id="24b46-163">Number of error devices</span></span>|
|<span data-ttu-id="24b46-164">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="24b46-164">conflictDeviceCount</span></span>|<span data-ttu-id="24b46-165">Int32</span><span class="sxs-lookup"><span data-stu-id="24b46-165">Int32</span></span>|<span data-ttu-id="24b46-166">競合デバイスの数</span><span class="sxs-lookup"><span data-stu-id="24b46-166">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="24b46-167">応答</span><span class="sxs-lookup"><span data-stu-id="24b46-167">Response</span></span>
<span data-ttu-id="24b46-168">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="24b46-168">If successful, this method returns a `201 Created` response code and a [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="24b46-169">例</span><span class="sxs-lookup"><span data-stu-id="24b46-169">Example</span></span>

### <a name="request"></a><span data-ttu-id="24b46-170">要求</span><span class="sxs-lookup"><span data-stu-id="24b46-170">Request</span></span>
<span data-ttu-id="24b46-171">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="24b46-171">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="24b46-172">応答</span><span class="sxs-lookup"><span data-stu-id="24b46-172">Response</span></span>
<span data-ttu-id="24b46-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="24b46-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




