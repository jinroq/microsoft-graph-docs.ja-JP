---
title: advancedThreatProtectionOnboardingStateSummary の更新
description: advancedThreatProtectionOnboardingStateSummary オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 94d146bc9696e02e824af02732b6e22b70533535
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30144857"
---
# <a name="update-advancedthreatprotectiononboardingstatesummary"></a><span data-ttu-id="35b99-103">advancedThreatProtectionOnboardingStateSummary の更新</span><span class="sxs-lookup"><span data-stu-id="35b99-103">Update advancedThreatProtectionOnboardingStateSummary</span></span>

> <span data-ttu-id="35b99-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="35b99-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="35b99-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="35b99-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="35b99-106">[advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="35b99-106">Update the properties of a [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="35b99-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="35b99-107">Prerequisites</span></span>
<span data-ttu-id="35b99-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="35b99-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="35b99-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="35b99-110">Permission type</span></span>|<span data-ttu-id="35b99-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="35b99-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="35b99-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="35b99-112">Delegated (work or school account)</span></span>|<span data-ttu-id="35b99-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="35b99-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="35b99-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="35b99-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="35b99-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="35b99-115">Not supported.</span></span>|
|<span data-ttu-id="35b99-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="35b99-116">Application</span></span>|<span data-ttu-id="35b99-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="35b99-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="35b99-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="35b99-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/advancedThreatProtectionOnboardingStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="35b99-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="35b99-119">Request headers</span></span>
|<span data-ttu-id="35b99-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="35b99-120">Header</span></span>|<span data-ttu-id="35b99-121">値</span><span class="sxs-lookup"><span data-stu-id="35b99-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="35b99-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="35b99-122">Authorization</span></span>|<span data-ttu-id="35b99-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="35b99-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="35b99-124">承諾</span><span class="sxs-lookup"><span data-stu-id="35b99-124">Accept</span></span>|<span data-ttu-id="35b99-125">application/json</span><span class="sxs-lookup"><span data-stu-id="35b99-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="35b99-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="35b99-126">Request body</span></span>
<span data-ttu-id="35b99-127">要求本文で、 [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="35b99-127">In the request body, supply a JSON representation for the [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) object.</span></span>

<span data-ttu-id="35b99-128">次の表に、 [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="35b99-128">The following table shows the properties that are required when you create the [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md).</span></span>

|<span data-ttu-id="35b99-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="35b99-129">Property</span></span>|<span data-ttu-id="35b99-130">型</span><span class="sxs-lookup"><span data-stu-id="35b99-130">Type</span></span>|<span data-ttu-id="35b99-131">説明</span><span class="sxs-lookup"><span data-stu-id="35b99-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="35b99-132">id</span><span class="sxs-lookup"><span data-stu-id="35b99-132">id</span></span>|<span data-ttu-id="35b99-133">String</span><span class="sxs-lookup"><span data-stu-id="35b99-133">String</span></span>|<span data-ttu-id="35b99-134">一意識別子</span><span class="sxs-lookup"><span data-stu-id="35b99-134">Unique Identifier</span></span>|
|<span data-ttu-id="35b99-135">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="35b99-135">unknownDeviceCount</span></span>|<span data-ttu-id="35b99-136">Int32</span><span class="sxs-lookup"><span data-stu-id="35b99-136">Int32</span></span>|<span data-ttu-id="35b99-137">不明なデバイスの数</span><span class="sxs-lookup"><span data-stu-id="35b99-137">Number of unknown devices</span></span>|
|<span data-ttu-id="35b99-138">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="35b99-138">notApplicableDeviceCount</span></span>|<span data-ttu-id="35b99-139">Int32</span><span class="sxs-lookup"><span data-stu-id="35b99-139">Int32</span></span>|<span data-ttu-id="35b99-140">該当しないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="35b99-140">Number of not applicable devices</span></span>|
|<span data-ttu-id="35b99-141">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="35b99-141">compliantDeviceCount</span></span>|<span data-ttu-id="35b99-142">Int32</span><span class="sxs-lookup"><span data-stu-id="35b99-142">Int32</span></span>|<span data-ttu-id="35b99-143">準拠デバイスの数</span><span class="sxs-lookup"><span data-stu-id="35b99-143">Number of compliant devices</span></span>|
|<span data-ttu-id="35b99-144">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="35b99-144">remediatedDeviceCount</span></span>|<span data-ttu-id="35b99-145">Int32</span><span class="sxs-lookup"><span data-stu-id="35b99-145">Int32</span></span>|<span data-ttu-id="35b99-146">修復済みデバイスの数</span><span class="sxs-lookup"><span data-stu-id="35b99-146">Number of remediated devices</span></span>|
|<span data-ttu-id="35b99-147">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="35b99-147">nonCompliantDeviceCount</span></span>|<span data-ttu-id="35b99-148">Int32</span><span class="sxs-lookup"><span data-stu-id="35b99-148">Int32</span></span>|<span data-ttu-id="35b99-149">準拠していないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="35b99-149">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="35b99-150">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="35b99-150">errorDeviceCount</span></span>|<span data-ttu-id="35b99-151">Int32</span><span class="sxs-lookup"><span data-stu-id="35b99-151">Int32</span></span>|<span data-ttu-id="35b99-152">エラー デバイスの数</span><span class="sxs-lookup"><span data-stu-id="35b99-152">Number of error devices</span></span>|
|<span data-ttu-id="35b99-153">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="35b99-153">conflictDeviceCount</span></span>|<span data-ttu-id="35b99-154">Int32</span><span class="sxs-lookup"><span data-stu-id="35b99-154">Int32</span></span>|<span data-ttu-id="35b99-155">競合デバイスの数</span><span class="sxs-lookup"><span data-stu-id="35b99-155">Number of conflict devices</span></span>|
|<span data-ttu-id="35b99-156">notAssignedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="35b99-156">notAssignedDeviceCount</span></span>|<span data-ttu-id="35b99-157">Int32</span><span class="sxs-lookup"><span data-stu-id="35b99-157">Int32</span></span>|<span data-ttu-id="35b99-158">割り当てられていないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="35b99-158">Number of not assigned devices</span></span>|



## <a name="response"></a><span data-ttu-id="35b99-159">応答</span><span class="sxs-lookup"><span data-stu-id="35b99-159">Response</span></span>
<span data-ttu-id="35b99-160">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="35b99-160">If successful, this method returns a `200 OK` response code and an updated [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="35b99-161">例</span><span class="sxs-lookup"><span data-stu-id="35b99-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="35b99-162">要求</span><span class="sxs-lookup"><span data-stu-id="35b99-162">Request</span></span>
<span data-ttu-id="35b99-163">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="35b99-163">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/advancedThreatProtectionOnboardingStateSummary
Content-type: application/json
Content-length: 331

{
  "@odata.type": "#microsoft.graph.advancedThreatProtectionOnboardingStateSummary",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3,
  "notAssignedDeviceCount": 6
}
```

### <a name="response"></a><span data-ttu-id="35b99-164">応答</span><span class="sxs-lookup"><span data-stu-id="35b99-164">Response</span></span>
<span data-ttu-id="35b99-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="35b99-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 380

{
  "@odata.type": "#microsoft.graph.advancedThreatProtectionOnboardingStateSummary",
  "id": "74089602-9602-7408-0296-087402960874",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3,
  "notAssignedDeviceCount": 6
}
```




