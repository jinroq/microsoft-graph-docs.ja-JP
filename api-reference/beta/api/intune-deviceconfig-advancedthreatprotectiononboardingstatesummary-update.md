---
title: AdvancedThreatProtectionOnboardingStateSummary を更新します。
description: AdvancedThreatProtectionOnboardingStateSummary オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 423e1c9862d0e42e7d85efacd17cdd5f1733e0e9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27929495"
---
# <a name="update-advancedthreatprotectiononboardingstatesummary"></a><span data-ttu-id="8983c-103">AdvancedThreatProtectionOnboardingStateSummary を更新します。</span><span class="sxs-lookup"><span data-stu-id="8983c-103">Update advancedThreatProtectionOnboardingStateSummary</span></span>

> <span data-ttu-id="8983c-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="8983c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8983c-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8983c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8983c-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="8983c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8983c-107">[AdvancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="8983c-107">Update the properties of a [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8983c-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="8983c-108">Prerequisites</span></span>
<span data-ttu-id="8983c-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8983c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8983c-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8983c-111">Permission type</span></span>|<span data-ttu-id="8983c-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="8983c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8983c-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8983c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8983c-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8983c-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8983c-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8983c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8983c-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8983c-116">Not supported.</span></span>|
|<span data-ttu-id="8983c-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8983c-117">Application</span></span>|<span data-ttu-id="8983c-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8983c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8983c-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8983c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/advancedThreatProtectionOnboardingStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="8983c-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8983c-120">Request headers</span></span>
|<span data-ttu-id="8983c-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8983c-121">Header</span></span>|<span data-ttu-id="8983c-122">値</span><span class="sxs-lookup"><span data-stu-id="8983c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8983c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8983c-123">Authorization</span></span>|<span data-ttu-id="8983c-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="8983c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8983c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8983c-125">Accept</span></span>|<span data-ttu-id="8983c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8983c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8983c-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="8983c-127">Request body</span></span>
<span data-ttu-id="8983c-128">要求の本文に[advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="8983c-128">In the request body, supply a JSON representation for the [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) object.</span></span>

<span data-ttu-id="8983c-129">[AdvancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="8983c-129">The following table shows the properties that are required when you create the [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md).</span></span>

|<span data-ttu-id="8983c-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8983c-130">Property</span></span>|<span data-ttu-id="8983c-131">型</span><span class="sxs-lookup"><span data-stu-id="8983c-131">Type</span></span>|<span data-ttu-id="8983c-132">説明</span><span class="sxs-lookup"><span data-stu-id="8983c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8983c-133">ID</span><span class="sxs-lookup"><span data-stu-id="8983c-133">id</span></span>|<span data-ttu-id="8983c-134">String</span><span class="sxs-lookup"><span data-stu-id="8983c-134">String</span></span>|<span data-ttu-id="8983c-135">一意識別子</span><span class="sxs-lookup"><span data-stu-id="8983c-135">Unique Identifier</span></span>|
|<span data-ttu-id="8983c-136">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8983c-136">unknownDeviceCount</span></span>|<span data-ttu-id="8983c-137">Int32</span><span class="sxs-lookup"><span data-stu-id="8983c-137">Int32</span></span>|<span data-ttu-id="8983c-138">不明なデバイスの数</span><span class="sxs-lookup"><span data-stu-id="8983c-138">Number of unknown devices</span></span>|
|<span data-ttu-id="8983c-139">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8983c-139">notApplicableDeviceCount</span></span>|<span data-ttu-id="8983c-140">Int32</span><span class="sxs-lookup"><span data-stu-id="8983c-140">Int32</span></span>|<span data-ttu-id="8983c-141">該当しないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="8983c-141">Number of not applicable devices</span></span>|
|<span data-ttu-id="8983c-142">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8983c-142">compliantDeviceCount</span></span>|<span data-ttu-id="8983c-143">Int32</span><span class="sxs-lookup"><span data-stu-id="8983c-143">Int32</span></span>|<span data-ttu-id="8983c-144">準拠デバイスの数</span><span class="sxs-lookup"><span data-stu-id="8983c-144">Number of compliant devices</span></span>|
|<span data-ttu-id="8983c-145">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8983c-145">remediatedDeviceCount</span></span>|<span data-ttu-id="8983c-146">Int32</span><span class="sxs-lookup"><span data-stu-id="8983c-146">Int32</span></span>|<span data-ttu-id="8983c-147">修復済みデバイスの数</span><span class="sxs-lookup"><span data-stu-id="8983c-147">Number of remediated devices</span></span>|
|<span data-ttu-id="8983c-148">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8983c-148">nonCompliantDeviceCount</span></span>|<span data-ttu-id="8983c-149">Int32</span><span class="sxs-lookup"><span data-stu-id="8983c-149">Int32</span></span>|<span data-ttu-id="8983c-150">準拠していないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="8983c-150">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="8983c-151">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8983c-151">errorDeviceCount</span></span>|<span data-ttu-id="8983c-152">Int32</span><span class="sxs-lookup"><span data-stu-id="8983c-152">Int32</span></span>|<span data-ttu-id="8983c-153">エラー デバイスの数</span><span class="sxs-lookup"><span data-stu-id="8983c-153">Number of error devices</span></span>|
|<span data-ttu-id="8983c-154">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8983c-154">conflictDeviceCount</span></span>|<span data-ttu-id="8983c-155">Int32</span><span class="sxs-lookup"><span data-stu-id="8983c-155">Int32</span></span>|<span data-ttu-id="8983c-156">競合デバイスの数</span><span class="sxs-lookup"><span data-stu-id="8983c-156">Number of conflict devices</span></span>|
|<span data-ttu-id="8983c-157">notAssignedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8983c-157">notAssignedDeviceCount</span></span>|<span data-ttu-id="8983c-158">Int32</span><span class="sxs-lookup"><span data-stu-id="8983c-158">Int32</span></span>|<span data-ttu-id="8983c-159">割り当てられていないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="8983c-159">Number of not assigned devices</span></span>|



## <a name="response"></a><span data-ttu-id="8983c-160">応答</span><span class="sxs-lookup"><span data-stu-id="8983c-160">Response</span></span>
<span data-ttu-id="8983c-161">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="8983c-161">If successful, this method returns a `200 OK` response code and an updated [advancedThreatProtectionOnboardingStateSummary](../resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8983c-162">例</span><span class="sxs-lookup"><span data-stu-id="8983c-162">Example</span></span>
### <a name="request"></a><span data-ttu-id="8983c-163">要求</span><span class="sxs-lookup"><span data-stu-id="8983c-163">Request</span></span>
<span data-ttu-id="8983c-164">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8983c-164">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/advancedThreatProtectionOnboardingStateSummary
Content-type: application/json
Content-length: 246

{
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

### <a name="response"></a><span data-ttu-id="8983c-165">応答</span><span class="sxs-lookup"><span data-stu-id="8983c-165">Response</span></span>
<span data-ttu-id="8983c-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8983c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





