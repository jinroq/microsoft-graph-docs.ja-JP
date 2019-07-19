---
title: DeviceManagementIntentDeviceSettingStateSummary を作成する
description: 新しい deviceManagementIntentDeviceSettingStateSummary オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 91ca4f510a70af4fff6790450a209ebec462726c
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34960329"
---
# <a name="create-devicemanagementintentdevicesettingstatesummary"></a><span data-ttu-id="d72e2-103">DeviceManagementIntentDeviceSettingStateSummary を作成する</span><span class="sxs-lookup"><span data-stu-id="d72e2-103">Create deviceManagementIntentDeviceSettingStateSummary</span></span>

> <span data-ttu-id="d72e2-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d72e2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d72e2-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d72e2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d72e2-106">新しい[deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="d72e2-106">Create a new [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d72e2-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="d72e2-107">Prerequisites</span></span>
<span data-ttu-id="d72e2-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d72e2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d72e2-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d72e2-110">Permission type</span></span>|<span data-ttu-id="d72e2-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="d72e2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d72e2-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d72e2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d72e2-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d72e2-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d72e2-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d72e2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d72e2-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d72e2-115">Not supported.</span></span>|
|<span data-ttu-id="d72e2-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d72e2-116">Application</span></span>|<span data-ttu-id="d72e2-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d72e2-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d72e2-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d72e2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intents/{deviceManagementIntentId}/deviceSettingStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="d72e2-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d72e2-119">Request headers</span></span>
|<span data-ttu-id="d72e2-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d72e2-120">Header</span></span>|<span data-ttu-id="d72e2-121">値</span><span class="sxs-lookup"><span data-stu-id="d72e2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d72e2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d72e2-122">Authorization</span></span>|<span data-ttu-id="d72e2-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="d72e2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d72e2-124">承諾</span><span class="sxs-lookup"><span data-stu-id="d72e2-124">Accept</span></span>|<span data-ttu-id="d72e2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d72e2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d72e2-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="d72e2-126">Request body</span></span>
<span data-ttu-id="d72e2-127">要求本文で、deviceManagementIntentDeviceSettingStateSummary オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="d72e2-127">In the request body, supply a JSON representation for the deviceManagementIntentDeviceSettingStateSummary object.</span></span>

<span data-ttu-id="d72e2-128">次の表に、deviceManagementIntentDeviceSettingStateSummary の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="d72e2-128">The following table shows the properties that are required when you create the deviceManagementIntentDeviceSettingStateSummary.</span></span>

|<span data-ttu-id="d72e2-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d72e2-129">Property</span></span>|<span data-ttu-id="d72e2-130">型</span><span class="sxs-lookup"><span data-stu-id="d72e2-130">Type</span></span>|<span data-ttu-id="d72e2-131">説明</span><span class="sxs-lookup"><span data-stu-id="d72e2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d72e2-132">id</span><span class="sxs-lookup"><span data-stu-id="d72e2-132">id</span></span>|<span data-ttu-id="d72e2-133">String</span><span class="sxs-lookup"><span data-stu-id="d72e2-133">String</span></span>|<span data-ttu-id="d72e2-134">ID</span><span class="sxs-lookup"><span data-stu-id="d72e2-134">The ID</span></span>|
|<span data-ttu-id="d72e2-135">settingName</span><span class="sxs-lookup"><span data-stu-id="d72e2-135">settingName</span></span>|<span data-ttu-id="d72e2-136">String</span><span class="sxs-lookup"><span data-stu-id="d72e2-136">String</span></span>|<span data-ttu-id="d72e2-137">設定の名前</span><span class="sxs-lookup"><span data-stu-id="d72e2-137">Name of a setting</span></span>|
|<span data-ttu-id="d72e2-138">compliantCount</span><span class="sxs-lookup"><span data-stu-id="d72e2-138">compliantCount</span></span>|<span data-ttu-id="d72e2-139">Int32</span><span class="sxs-lookup"><span data-stu-id="d72e2-139">Int32</span></span>|<span data-ttu-id="d72e2-140">準拠デバイスの数</span><span class="sxs-lookup"><span data-stu-id="d72e2-140">Number of compliant devices</span></span>|
|<span data-ttu-id="d72e2-141">conflictCount</span><span class="sxs-lookup"><span data-stu-id="d72e2-141">conflictCount</span></span>|<span data-ttu-id="d72e2-142">Int32</span><span class="sxs-lookup"><span data-stu-id="d72e2-142">Int32</span></span>|<span data-ttu-id="d72e2-143">競合しているデバイスの数</span><span class="sxs-lookup"><span data-stu-id="d72e2-143">Number of devices in conflict</span></span>|
|<span data-ttu-id="d72e2-144">errorCount</span><span class="sxs-lookup"><span data-stu-id="d72e2-144">errorCount</span></span>|<span data-ttu-id="d72e2-145">Int32</span><span class="sxs-lookup"><span data-stu-id="d72e2-145">Int32</span></span>|<span data-ttu-id="d72e2-146">エラー デバイスの数</span><span class="sxs-lookup"><span data-stu-id="d72e2-146">Number of error devices</span></span>|
|<span data-ttu-id="d72e2-147">nonCompliantCount</span><span class="sxs-lookup"><span data-stu-id="d72e2-147">nonCompliantCount</span></span>|<span data-ttu-id="d72e2-148">Int32</span><span class="sxs-lookup"><span data-stu-id="d72e2-148">Int32</span></span>|<span data-ttu-id="d72e2-149">準拠していないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="d72e2-149">Number of non compliant devices</span></span>|
|<span data-ttu-id="d72e2-150">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="d72e2-150">notApplicableCount</span></span>|<span data-ttu-id="d72e2-151">Int32</span><span class="sxs-lookup"><span data-stu-id="d72e2-151">Int32</span></span>|<span data-ttu-id="d72e2-152">該当しないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="d72e2-152">Number of not applicable devices</span></span>|
|<span data-ttu-id="d72e2-153">remediatedCount</span><span class="sxs-lookup"><span data-stu-id="d72e2-153">remediatedCount</span></span>|<span data-ttu-id="d72e2-154">Int32</span><span class="sxs-lookup"><span data-stu-id="d72e2-154">Int32</span></span>|<span data-ttu-id="d72e2-155">修復済みデバイスの数</span><span class="sxs-lookup"><span data-stu-id="d72e2-155">Number of remediated devices</span></span>|



## <a name="response"></a><span data-ttu-id="d72e2-156">応答</span><span class="sxs-lookup"><span data-stu-id="d72e2-156">Response</span></span>
<span data-ttu-id="d72e2-157">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="d72e2-157">If successful, this method returns a `201 Created` response code and a [deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d72e2-158">例</span><span class="sxs-lookup"><span data-stu-id="d72e2-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="d72e2-159">要求</span><span class="sxs-lookup"><span data-stu-id="d72e2-159">Request</span></span>
<span data-ttu-id="d72e2-160">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d72e2-160">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/deviceSettingStateSummaries
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

### <a name="response"></a><span data-ttu-id="d72e2-161">応答</span><span class="sxs-lookup"><span data-stu-id="d72e2-161">Response</span></span>
<span data-ttu-id="d72e2-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d72e2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





