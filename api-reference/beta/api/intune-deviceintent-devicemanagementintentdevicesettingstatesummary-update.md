---
title: deviceManagementIntentDeviceSettingStateSummary の更新
description: deviceManagementIntentDeviceSettingStateSummary オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 46a57541278e5da44e5af6e2a3717a310a1b4b98
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/08/2019
ms.locfileid: "31522399"
---
# <a name="update-devicemanagementintentdevicesettingstatesummary"></a><span data-ttu-id="d96cf-103">deviceManagementIntentDeviceSettingStateSummary の更新</span><span class="sxs-lookup"><span data-stu-id="d96cf-103">Update deviceManagementIntentDeviceSettingStateSummary</span></span>

> <span data-ttu-id="d96cf-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d96cf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d96cf-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d96cf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d96cf-106">[deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="d96cf-106">Update the properties of a [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d96cf-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="d96cf-107">Prerequisites</span></span>
<span data-ttu-id="d96cf-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d96cf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d96cf-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d96cf-110">Permission type</span></span>|<span data-ttu-id="d96cf-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="d96cf-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d96cf-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d96cf-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d96cf-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d96cf-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d96cf-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d96cf-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d96cf-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d96cf-115">Not supported.</span></span>|
|<span data-ttu-id="d96cf-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d96cf-116">Application</span></span>|<span data-ttu-id="d96cf-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d96cf-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d96cf-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d96cf-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intents/{deviceManagementIntentId}/deviceSettingStateSummaries/{deviceManagementIntentDeviceSettingStateSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="d96cf-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d96cf-119">Request headers</span></span>
|<span data-ttu-id="d96cf-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d96cf-120">Header</span></span>|<span data-ttu-id="d96cf-121">値</span><span class="sxs-lookup"><span data-stu-id="d96cf-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d96cf-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d96cf-122">Authorization</span></span>|<span data-ttu-id="d96cf-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="d96cf-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d96cf-124">承諾</span><span class="sxs-lookup"><span data-stu-id="d96cf-124">Accept</span></span>|<span data-ttu-id="d96cf-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d96cf-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d96cf-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="d96cf-126">Request body</span></span>
<span data-ttu-id="d96cf-127">要求本文で、 [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="d96cf-127">In the request body, supply a JSON representation for the [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) object.</span></span>

<span data-ttu-id="d96cf-128">次の表に、 [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="d96cf-128">The following table shows the properties that are required when you create the [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md).</span></span>

|<span data-ttu-id="d96cf-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d96cf-129">Property</span></span>|<span data-ttu-id="d96cf-130">型</span><span class="sxs-lookup"><span data-stu-id="d96cf-130">Type</span></span>|<span data-ttu-id="d96cf-131">説明</span><span class="sxs-lookup"><span data-stu-id="d96cf-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d96cf-132">id</span><span class="sxs-lookup"><span data-stu-id="d96cf-132">id</span></span>|<span data-ttu-id="d96cf-133">String</span><span class="sxs-lookup"><span data-stu-id="d96cf-133">String</span></span>|<span data-ttu-id="d96cf-134">ID</span><span class="sxs-lookup"><span data-stu-id="d96cf-134">The ID</span></span>|
|<span data-ttu-id="d96cf-135">settingName</span><span class="sxs-lookup"><span data-stu-id="d96cf-135">settingName</span></span>|<span data-ttu-id="d96cf-136">String</span><span class="sxs-lookup"><span data-stu-id="d96cf-136">String</span></span>|<span data-ttu-id="d96cf-137">設定の名前</span><span class="sxs-lookup"><span data-stu-id="d96cf-137">Name of a setting</span></span>|
|<span data-ttu-id="d96cf-138">compliantCount</span><span class="sxs-lookup"><span data-stu-id="d96cf-138">compliantCount</span></span>|<span data-ttu-id="d96cf-139">Int32</span><span class="sxs-lookup"><span data-stu-id="d96cf-139">Int32</span></span>|<span data-ttu-id="d96cf-140">準拠デバイスの数</span><span class="sxs-lookup"><span data-stu-id="d96cf-140">Number of compliant devices</span></span>|
|<span data-ttu-id="d96cf-141">conflictCount</span><span class="sxs-lookup"><span data-stu-id="d96cf-141">conflictCount</span></span>|<span data-ttu-id="d96cf-142">Int32</span><span class="sxs-lookup"><span data-stu-id="d96cf-142">Int32</span></span>|<span data-ttu-id="d96cf-143">競合しているデバイスの数</span><span class="sxs-lookup"><span data-stu-id="d96cf-143">Number of devices in conflict</span></span>|
|<span data-ttu-id="d96cf-144">errorCount</span><span class="sxs-lookup"><span data-stu-id="d96cf-144">errorCount</span></span>|<span data-ttu-id="d96cf-145">Int32</span><span class="sxs-lookup"><span data-stu-id="d96cf-145">Int32</span></span>|<span data-ttu-id="d96cf-146">エラー デバイスの数</span><span class="sxs-lookup"><span data-stu-id="d96cf-146">Number of error devices</span></span>|
|<span data-ttu-id="d96cf-147">nonCompliantCount</span><span class="sxs-lookup"><span data-stu-id="d96cf-147">nonCompliantCount</span></span>|<span data-ttu-id="d96cf-148">Int32</span><span class="sxs-lookup"><span data-stu-id="d96cf-148">Int32</span></span>|<span data-ttu-id="d96cf-149">準拠していないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="d96cf-149">Number of non compliant devices</span></span>|
|<span data-ttu-id="d96cf-150">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="d96cf-150">notApplicableCount</span></span>|<span data-ttu-id="d96cf-151">Int32</span><span class="sxs-lookup"><span data-stu-id="d96cf-151">Int32</span></span>|<span data-ttu-id="d96cf-152">該当しないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="d96cf-152">Number of not applicable devices</span></span>|
|<span data-ttu-id="d96cf-153">remediatedCount</span><span class="sxs-lookup"><span data-stu-id="d96cf-153">remediatedCount</span></span>|<span data-ttu-id="d96cf-154">Int32</span><span class="sxs-lookup"><span data-stu-id="d96cf-154">Int32</span></span>|<span data-ttu-id="d96cf-155">修復済みデバイスの数</span><span class="sxs-lookup"><span data-stu-id="d96cf-155">Number of remediated devices</span></span>|



## <a name="response"></a><span data-ttu-id="d96cf-156">応答</span><span class="sxs-lookup"><span data-stu-id="d96cf-156">Response</span></span>
<span data-ttu-id="d96cf-157">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="d96cf-157">If successful, this method returns a `200 OK` response code and an updated [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d96cf-158">例</span><span class="sxs-lookup"><span data-stu-id="d96cf-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="d96cf-159">要求</span><span class="sxs-lookup"><span data-stu-id="d96cf-159">Request</span></span>
<span data-ttu-id="d96cf-160">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d96cf-160">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/deviceSettingStateSummaries/{deviceManagementIntentDeviceSettingStateSummaryId}
Content-type: application/json
Content-length: 280

{
  "@odata.type": "#microsoft.graph.deviceManagementIntentDeviceSettingStateSummary",
  "settingName": "Setting Name value",
  "compliantCount": 14,
  "conflictCount": 13,
  "errorCount": 10,
  "nonCompliantCount": 1,
  "notApplicableCount": 2,
  "remediatedCount": 15
}
```

### <a name="response"></a><span data-ttu-id="d96cf-161">応答</span><span class="sxs-lookup"><span data-stu-id="d96cf-161">Response</span></span>
<span data-ttu-id="d96cf-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d96cf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 329

{
  "@odata.type": "#microsoft.graph.deviceManagementIntentDeviceSettingStateSummary",
  "id": "d3d3a75f-a75f-d3d3-5fa7-d3d35fa7d3d3",
  "settingName": "Setting Name value",
  "compliantCount": 14,
  "conflictCount": 13,
  "errorCount": 10,
  "nonCompliantCount": 1,
  "notApplicableCount": 2,
  "remediatedCount": 15
}
```







