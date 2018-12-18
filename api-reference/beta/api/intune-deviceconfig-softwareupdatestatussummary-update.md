---
title: softwareUpdateStatusSummary の更新
description: softwareUpdateStatusSummary オブジェクトのプロパティを更新します。
author: tfitzmac
ms.openlocfilehash: 6cb95a9bfb28e0488148d1f8773c87209c585b70
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27302283"
---
# <a name="update-softwareupdatestatussummary"></a><span data-ttu-id="21b4f-103">softwareUpdateStatusSummary の更新</span><span class="sxs-lookup"><span data-stu-id="21b4f-103">Update softwareUpdateStatusSummary</span></span>

> <span data-ttu-id="21b4f-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="21b4f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="21b4f-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="21b4f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="21b4f-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="21b4f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="21b4f-107">[softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="21b4f-107">Update the properties of a [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="21b4f-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="21b4f-108">Prerequisites</span></span>
<span data-ttu-id="21b4f-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="21b4f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="21b4f-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="21b4f-111">Permission type</span></span>|<span data-ttu-id="21b4f-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="21b4f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="21b4f-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="21b4f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="21b4f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="21b4f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="21b4f-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="21b4f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="21b4f-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="21b4f-116">Not supported.</span></span>|
|<span data-ttu-id="21b4f-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="21b4f-117">Application</span></span>|<span data-ttu-id="21b4f-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="21b4f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="21b4f-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="21b4f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/softwareUpdateStatusSummary
```

## <a name="request-headers"></a><span data-ttu-id="21b4f-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="21b4f-120">Request headers</span></span>
|<span data-ttu-id="21b4f-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="21b4f-121">Header</span></span>|<span data-ttu-id="21b4f-122">値</span><span class="sxs-lookup"><span data-stu-id="21b4f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="21b4f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="21b4f-123">Authorization</span></span>|<span data-ttu-id="21b4f-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="21b4f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="21b4f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="21b4f-125">Accept</span></span>|<span data-ttu-id="21b4f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="21b4f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="21b4f-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="21b4f-127">Request body</span></span>
<span data-ttu-id="21b4f-128">要求本文で、[softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="21b4f-128">In the request body, supply a JSON representation for the [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object.</span></span>

<span data-ttu-id="21b4f-129">次の表に、[softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="21b4f-129">The following table shows the properties that are required when you create the [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md).</span></span>

|<span data-ttu-id="21b4f-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="21b4f-130">Property</span></span>|<span data-ttu-id="21b4f-131">種類</span><span class="sxs-lookup"><span data-stu-id="21b4f-131">Type</span></span>|<span data-ttu-id="21b4f-132">説明</span><span class="sxs-lookup"><span data-stu-id="21b4f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="21b4f-133">ID</span><span class="sxs-lookup"><span data-stu-id="21b4f-133">id</span></span>|<span data-ttu-id="21b4f-134">String</span><span class="sxs-lookup"><span data-stu-id="21b4f-134">String</span></span>|<span data-ttu-id="21b4f-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="21b4f-135">Key of the entity.</span></span>|
|<span data-ttu-id="21b4f-136">displayName</span><span class="sxs-lookup"><span data-stu-id="21b4f-136">displayName</span></span>|<span data-ttu-id="21b4f-137">String</span><span class="sxs-lookup"><span data-stu-id="21b4f-137">String</span></span>|<span data-ttu-id="21b4f-138">ポリシーの名前。</span><span class="sxs-lookup"><span data-stu-id="21b4f-138">The name of the policy.</span></span>|
|<span data-ttu-id="21b4f-139">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="21b4f-139">compliantDeviceCount</span></span>|<span data-ttu-id="21b4f-140">Int32</span><span class="sxs-lookup"><span data-stu-id="21b4f-140">Int32</span></span>|<span data-ttu-id="21b4f-141">準拠デバイスの数。</span><span class="sxs-lookup"><span data-stu-id="21b4f-141">Number of compliant devices.</span></span>|
|<span data-ttu-id="21b4f-142">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="21b4f-142">nonCompliantDeviceCount</span></span>|<span data-ttu-id="21b4f-143">Int32</span><span class="sxs-lookup"><span data-stu-id="21b4f-143">Int32</span></span>|<span data-ttu-id="21b4f-144">準拠していないデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="21b4f-144">Number of non compliant devices.</span></span>|
|<span data-ttu-id="21b4f-145">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="21b4f-145">remediatedDeviceCount</span></span>|<span data-ttu-id="21b4f-146">Int32</span><span class="sxs-lookup"><span data-stu-id="21b4f-146">Int32</span></span>|<span data-ttu-id="21b4f-147">修復済みデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="21b4f-147">Number of remediated devices.</span></span>|
|<span data-ttu-id="21b4f-148">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="21b4f-148">errorDeviceCount</span></span>|<span data-ttu-id="21b4f-149">Int32</span><span class="sxs-lookup"><span data-stu-id="21b4f-149">Int32</span></span>|<span data-ttu-id="21b4f-150">エラーが発生したデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="21b4f-150">Number of devices had error.</span></span>|
|<span data-ttu-id="21b4f-151">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="21b4f-151">unknownDeviceCount</span></span>|<span data-ttu-id="21b4f-152">Int32</span><span class="sxs-lookup"><span data-stu-id="21b4f-152">Int32</span></span>|<span data-ttu-id="21b4f-153">不明なデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="21b4f-153">Number of unknown devices.</span></span>|
|<span data-ttu-id="21b4f-154">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="21b4f-154">conflictDeviceCount</span></span>|<span data-ttu-id="21b4f-155">Int32</span><span class="sxs-lookup"><span data-stu-id="21b4f-155">Int32</span></span>|<span data-ttu-id="21b4f-156">競合デバイスの数。</span><span class="sxs-lookup"><span data-stu-id="21b4f-156">Number of conflict devices.</span></span>|
|<span data-ttu-id="21b4f-157">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="21b4f-157">notApplicableDeviceCount</span></span>|<span data-ttu-id="21b4f-158">Int32</span><span class="sxs-lookup"><span data-stu-id="21b4f-158">Int32</span></span>|<span data-ttu-id="21b4f-159">該当しないデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="21b4f-159">Number of not applicable devices.</span></span>|
|<span data-ttu-id="21b4f-160">compliantUserCount</span><span class="sxs-lookup"><span data-stu-id="21b4f-160">compliantUserCount</span></span>|<span data-ttu-id="21b4f-161">Int32</span><span class="sxs-lookup"><span data-stu-id="21b4f-161">Int32</span></span>|<span data-ttu-id="21b4f-162">準拠ユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="21b4f-162">Number of compliant users.</span></span>|
|<span data-ttu-id="21b4f-163">nonCompliantUserCount</span><span class="sxs-lookup"><span data-stu-id="21b4f-163">nonCompliantUserCount</span></span>|<span data-ttu-id="21b4f-164">Int32</span><span class="sxs-lookup"><span data-stu-id="21b4f-164">Int32</span></span>|<span data-ttu-id="21b4f-165">準拠していないユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="21b4f-165">Number of non compliant users.</span></span>|
|<span data-ttu-id="21b4f-166">remediatedUserCount</span><span class="sxs-lookup"><span data-stu-id="21b4f-166">remediatedUserCount</span></span>|<span data-ttu-id="21b4f-167">Int32</span><span class="sxs-lookup"><span data-stu-id="21b4f-167">Int32</span></span>|<span data-ttu-id="21b4f-168">修復済みユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="21b4f-168">Number of remediated users.</span></span>|
|<span data-ttu-id="21b4f-169">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="21b4f-169">errorUserCount</span></span>|<span data-ttu-id="21b4f-170">Int32</span><span class="sxs-lookup"><span data-stu-id="21b4f-170">Int32</span></span>|<span data-ttu-id="21b4f-171">エラーが発生したユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="21b4f-171">Number of users had error.</span></span>|
|<span data-ttu-id="21b4f-172">unknownUserCount</span><span class="sxs-lookup"><span data-stu-id="21b4f-172">unknownUserCount</span></span>|<span data-ttu-id="21b4f-173">Int32</span><span class="sxs-lookup"><span data-stu-id="21b4f-173">Int32</span></span>|<span data-ttu-id="21b4f-174">不明なユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="21b4f-174">Number of unknown users.</span></span>|
|<span data-ttu-id="21b4f-175">conflictUserCount</span><span class="sxs-lookup"><span data-stu-id="21b4f-175">conflictUserCount</span></span>|<span data-ttu-id="21b4f-176">Int32</span><span class="sxs-lookup"><span data-stu-id="21b4f-176">Int32</span></span>|<span data-ttu-id="21b4f-177">競合ユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="21b4f-177">Number of conflict users.</span></span>|
|<span data-ttu-id="21b4f-178">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="21b4f-178">notApplicableUserCount</span></span>|<span data-ttu-id="21b4f-179">Int32</span><span class="sxs-lookup"><span data-stu-id="21b4f-179">Int32</span></span>|<span data-ttu-id="21b4f-180">該当しないユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="21b4f-180">Number of not applicable users.</span></span>|



## <a name="response"></a><span data-ttu-id="21b4f-181">応答</span><span class="sxs-lookup"><span data-stu-id="21b4f-181">Response</span></span>
<span data-ttu-id="21b4f-182">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="21b4f-182">If successful, this method returns a `200 OK` response code and an updated [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="21b4f-183">例</span><span class="sxs-lookup"><span data-stu-id="21b4f-183">Example</span></span>
### <a name="request"></a><span data-ttu-id="21b4f-184">要求</span><span class="sxs-lookup"><span data-stu-id="21b4f-184">Request</span></span>
<span data-ttu-id="21b4f-185">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="21b4f-185">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/softwareUpdateStatusSummary
Content-type: application/json
Content-length: 452

{
  "displayName": "Display Name value",
  "compliantDeviceCount": 4,
  "nonCompliantDeviceCount": 7,
  "remediatedDeviceCount": 5,
  "errorDeviceCount": 0,
  "unknownDeviceCount": 2,
  "conflictDeviceCount": 3,
  "notApplicableDeviceCount": 8,
  "compliantUserCount": 2,
  "nonCompliantUserCount": 5,
  "remediatedUserCount": 3,
  "errorUserCount": 14,
  "unknownUserCount": 0,
  "conflictUserCount": 1,
  "notApplicableUserCount": 6
}
```

### <a name="response"></a><span data-ttu-id="21b4f-186">応答</span><span class="sxs-lookup"><span data-stu-id="21b4f-186">Response</span></span>
<span data-ttu-id="21b4f-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="21b4f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 567

{
  "@odata.type": "#microsoft.graph.softwareUpdateStatusSummary",
  "id": "4f71421f-421f-4f71-1f42-714f1f42714f",
  "displayName": "Display Name value",
  "compliantDeviceCount": 4,
  "nonCompliantDeviceCount": 7,
  "remediatedDeviceCount": 5,
  "errorDeviceCount": 0,
  "unknownDeviceCount": 2,
  "conflictDeviceCount": 3,
  "notApplicableDeviceCount": 8,
  "compliantUserCount": 2,
  "nonCompliantUserCount": 5,
  "remediatedUserCount": 3,
  "errorUserCount": 14,
  "unknownUserCount": 0,
  "conflictUserCount": 1,
  "notApplicableUserCount": 6
}
```





