---
title: deviceConfigurationDeviceStateSummary の更新
description: deviceConfigurationDeviceStateSummary オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6f7077e76e6bfc0c0652291a491eab4e1aee0d97
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32469398"
---
# <a name="update-deviceconfigurationdevicestatesummary"></a><span data-ttu-id="09e58-103">deviceConfigurationDeviceStateSummary の更新</span><span class="sxs-lookup"><span data-stu-id="09e58-103">Update deviceConfigurationDeviceStateSummary</span></span>

> <span data-ttu-id="09e58-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="09e58-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="09e58-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="09e58-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="09e58-106">[deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="09e58-106">Update the properties of a [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="09e58-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="09e58-107">Prerequisites</span></span>
<span data-ttu-id="09e58-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="09e58-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="09e58-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="09e58-110">Permission type</span></span>|<span data-ttu-id="09e58-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="09e58-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="09e58-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="09e58-112">Delegated (work or school account)</span></span>|<span data-ttu-id="09e58-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09e58-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="09e58-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="09e58-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="09e58-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="09e58-115">Not supported.</span></span>|
|<span data-ttu-id="09e58-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="09e58-116">Application</span></span>|<span data-ttu-id="09e58-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="09e58-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="09e58-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="09e58-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationDeviceStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="09e58-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="09e58-119">Request headers</span></span>
|<span data-ttu-id="09e58-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="09e58-120">Header</span></span>|<span data-ttu-id="09e58-121">値</span><span class="sxs-lookup"><span data-stu-id="09e58-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="09e58-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="09e58-122">Authorization</span></span>|<span data-ttu-id="09e58-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="09e58-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="09e58-124">承諾</span><span class="sxs-lookup"><span data-stu-id="09e58-124">Accept</span></span>|<span data-ttu-id="09e58-125">application/json</span><span class="sxs-lookup"><span data-stu-id="09e58-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="09e58-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="09e58-126">Request body</span></span>
<span data-ttu-id="09e58-127">要求本文で、[deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="09e58-127">In the request body, supply a JSON representation for the [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object.</span></span>

<span data-ttu-id="09e58-128">次の表に、[deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="09e58-128">The following table shows the properties that are required when you create the [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md).</span></span>

|<span data-ttu-id="09e58-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="09e58-129">Property</span></span>|<span data-ttu-id="09e58-130">型</span><span class="sxs-lookup"><span data-stu-id="09e58-130">Type</span></span>|<span data-ttu-id="09e58-131">説明</span><span class="sxs-lookup"><span data-stu-id="09e58-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="09e58-132">id</span><span class="sxs-lookup"><span data-stu-id="09e58-132">id</span></span>|<span data-ttu-id="09e58-133">String</span><span class="sxs-lookup"><span data-stu-id="09e58-133">String</span></span>|<span data-ttu-id="09e58-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="09e58-134">Key of the entity.</span></span>|
|<span data-ttu-id="09e58-135">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="09e58-135">unknownDeviceCount</span></span>|<span data-ttu-id="09e58-136">Int32</span><span class="sxs-lookup"><span data-stu-id="09e58-136">Int32</span></span>|<span data-ttu-id="09e58-137">不明なデバイスの数</span><span class="sxs-lookup"><span data-stu-id="09e58-137">Number of unknown devices</span></span>|
|<span data-ttu-id="09e58-138">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="09e58-138">notApplicableDeviceCount</span></span>|<span data-ttu-id="09e58-139">Int32</span><span class="sxs-lookup"><span data-stu-id="09e58-139">Int32</span></span>|<span data-ttu-id="09e58-140">該当しないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="09e58-140">Number of not applicable devices</span></span>|
|<span data-ttu-id="09e58-141">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="09e58-141">compliantDeviceCount</span></span>|<span data-ttu-id="09e58-142">Int32</span><span class="sxs-lookup"><span data-stu-id="09e58-142">Int32</span></span>|<span data-ttu-id="09e58-143">準拠デバイスの数</span><span class="sxs-lookup"><span data-stu-id="09e58-143">Number of compliant devices</span></span>|
|<span data-ttu-id="09e58-144">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="09e58-144">remediatedDeviceCount</span></span>|<span data-ttu-id="09e58-145">Int32</span><span class="sxs-lookup"><span data-stu-id="09e58-145">Int32</span></span>|<span data-ttu-id="09e58-146">修復済みデバイスの数</span><span class="sxs-lookup"><span data-stu-id="09e58-146">Number of remediated devices</span></span>|
|<span data-ttu-id="09e58-147">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="09e58-147">nonCompliantDeviceCount</span></span>|<span data-ttu-id="09e58-148">Int32</span><span class="sxs-lookup"><span data-stu-id="09e58-148">Int32</span></span>|<span data-ttu-id="09e58-149">準拠していないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="09e58-149">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="09e58-150">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="09e58-150">errorDeviceCount</span></span>|<span data-ttu-id="09e58-151">Int32</span><span class="sxs-lookup"><span data-stu-id="09e58-151">Int32</span></span>|<span data-ttu-id="09e58-152">エラー デバイスの数</span><span class="sxs-lookup"><span data-stu-id="09e58-152">Number of error devices</span></span>|
|<span data-ttu-id="09e58-153">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="09e58-153">conflictDeviceCount</span></span>|<span data-ttu-id="09e58-154">Int32</span><span class="sxs-lookup"><span data-stu-id="09e58-154">Int32</span></span>|<span data-ttu-id="09e58-155">競合デバイスの数</span><span class="sxs-lookup"><span data-stu-id="09e58-155">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="09e58-156">応答</span><span class="sxs-lookup"><span data-stu-id="09e58-156">Response</span></span>
<span data-ttu-id="09e58-157">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="09e58-157">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="09e58-158">例</span><span class="sxs-lookup"><span data-stu-id="09e58-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="09e58-159">要求</span><span class="sxs-lookup"><span data-stu-id="09e58-159">Request</span></span>
<span data-ttu-id="09e58-160">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="09e58-160">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationDeviceStateSummaries
Content-type: application/json
Content-length: 290

{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceStateSummary",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```

### <a name="response"></a><span data-ttu-id="09e58-161">応答</span><span class="sxs-lookup"><span data-stu-id="09e58-161">Response</span></span>
<span data-ttu-id="09e58-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="09e58-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 339

{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceStateSummary",
  "id": "5db26f5a-6f5a-5db2-5a6f-b25d5a6fb25d",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```





