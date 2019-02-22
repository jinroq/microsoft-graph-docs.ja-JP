---
title: softwareUpdateStatusSummary の更新
description: softwareUpdateStatusSummary オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 76475402e0bb240606cfff0ed25b4502b2feb206
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30145095"
---
# <a name="update-softwareupdatestatussummary"></a><span data-ttu-id="45f60-103">softwareUpdateStatusSummary の更新</span><span class="sxs-lookup"><span data-stu-id="45f60-103">Update softwareUpdateStatusSummary</span></span>

> <span data-ttu-id="45f60-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="45f60-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="45f60-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="45f60-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="45f60-106">[softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="45f60-106">Update the properties of a [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="45f60-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="45f60-107">Prerequisites</span></span>
<span data-ttu-id="45f60-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="45f60-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="45f60-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="45f60-110">Permission type</span></span>|<span data-ttu-id="45f60-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="45f60-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="45f60-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="45f60-112">Delegated (work or school account)</span></span>|<span data-ttu-id="45f60-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45f60-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="45f60-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="45f60-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="45f60-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="45f60-115">Not supported.</span></span>|
|<span data-ttu-id="45f60-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="45f60-116">Application</span></span>|<span data-ttu-id="45f60-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="45f60-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="45f60-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="45f60-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/softwareUpdateStatusSummary
```

## <a name="request-headers"></a><span data-ttu-id="45f60-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="45f60-119">Request headers</span></span>
|<span data-ttu-id="45f60-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="45f60-120">Header</span></span>|<span data-ttu-id="45f60-121">値</span><span class="sxs-lookup"><span data-stu-id="45f60-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="45f60-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="45f60-122">Authorization</span></span>|<span data-ttu-id="45f60-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="45f60-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="45f60-124">承諾</span><span class="sxs-lookup"><span data-stu-id="45f60-124">Accept</span></span>|<span data-ttu-id="45f60-125">application/json</span><span class="sxs-lookup"><span data-stu-id="45f60-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="45f60-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="45f60-126">Request body</span></span>
<span data-ttu-id="45f60-127">要求本文で、[softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="45f60-127">In the request body, supply a JSON representation for the [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object.</span></span>

<span data-ttu-id="45f60-128">次の表に、[softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="45f60-128">The following table shows the properties that are required when you create the [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md).</span></span>

|<span data-ttu-id="45f60-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="45f60-129">Property</span></span>|<span data-ttu-id="45f60-130">型</span><span class="sxs-lookup"><span data-stu-id="45f60-130">Type</span></span>|<span data-ttu-id="45f60-131">説明</span><span class="sxs-lookup"><span data-stu-id="45f60-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="45f60-132">id</span><span class="sxs-lookup"><span data-stu-id="45f60-132">id</span></span>|<span data-ttu-id="45f60-133">String</span><span class="sxs-lookup"><span data-stu-id="45f60-133">String</span></span>|<span data-ttu-id="45f60-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="45f60-134">Key of the entity.</span></span>|
|<span data-ttu-id="45f60-135">displayName</span><span class="sxs-lookup"><span data-stu-id="45f60-135">displayName</span></span>|<span data-ttu-id="45f60-136">String</span><span class="sxs-lookup"><span data-stu-id="45f60-136">String</span></span>|<span data-ttu-id="45f60-137">ポリシーの名前。</span><span class="sxs-lookup"><span data-stu-id="45f60-137">The name of the policy.</span></span>|
|<span data-ttu-id="45f60-138">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="45f60-138">compliantDeviceCount</span></span>|<span data-ttu-id="45f60-139">Int32</span><span class="sxs-lookup"><span data-stu-id="45f60-139">Int32</span></span>|<span data-ttu-id="45f60-140">準拠デバイスの数。</span><span class="sxs-lookup"><span data-stu-id="45f60-140">Number of compliant devices.</span></span>|
|<span data-ttu-id="45f60-141">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="45f60-141">nonCompliantDeviceCount</span></span>|<span data-ttu-id="45f60-142">Int32</span><span class="sxs-lookup"><span data-stu-id="45f60-142">Int32</span></span>|<span data-ttu-id="45f60-143">準拠していないデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="45f60-143">Number of non compliant devices.</span></span>|
|<span data-ttu-id="45f60-144">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="45f60-144">remediatedDeviceCount</span></span>|<span data-ttu-id="45f60-145">Int32</span><span class="sxs-lookup"><span data-stu-id="45f60-145">Int32</span></span>|<span data-ttu-id="45f60-146">修復済みデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="45f60-146">Number of remediated devices.</span></span>|
|<span data-ttu-id="45f60-147">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="45f60-147">errorDeviceCount</span></span>|<span data-ttu-id="45f60-148">Int32</span><span class="sxs-lookup"><span data-stu-id="45f60-148">Int32</span></span>|<span data-ttu-id="45f60-149">エラーが発生したデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="45f60-149">Number of devices had error.</span></span>|
|<span data-ttu-id="45f60-150">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="45f60-150">unknownDeviceCount</span></span>|<span data-ttu-id="45f60-151">Int32</span><span class="sxs-lookup"><span data-stu-id="45f60-151">Int32</span></span>|<span data-ttu-id="45f60-152">不明なデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="45f60-152">Number of unknown devices.</span></span>|
|<span data-ttu-id="45f60-153">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="45f60-153">conflictDeviceCount</span></span>|<span data-ttu-id="45f60-154">Int32</span><span class="sxs-lookup"><span data-stu-id="45f60-154">Int32</span></span>|<span data-ttu-id="45f60-155">競合デバイスの数。</span><span class="sxs-lookup"><span data-stu-id="45f60-155">Number of conflict devices.</span></span>|
|<span data-ttu-id="45f60-156">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="45f60-156">notApplicableDeviceCount</span></span>|<span data-ttu-id="45f60-157">Int32</span><span class="sxs-lookup"><span data-stu-id="45f60-157">Int32</span></span>|<span data-ttu-id="45f60-158">該当しないデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="45f60-158">Number of not applicable devices.</span></span>|
|<span data-ttu-id="45f60-159">compliantUserCount</span><span class="sxs-lookup"><span data-stu-id="45f60-159">compliantUserCount</span></span>|<span data-ttu-id="45f60-160">Int32</span><span class="sxs-lookup"><span data-stu-id="45f60-160">Int32</span></span>|<span data-ttu-id="45f60-161">準拠ユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="45f60-161">Number of compliant users.</span></span>|
|<span data-ttu-id="45f60-162">nonCompliantUserCount</span><span class="sxs-lookup"><span data-stu-id="45f60-162">nonCompliantUserCount</span></span>|<span data-ttu-id="45f60-163">Int32</span><span class="sxs-lookup"><span data-stu-id="45f60-163">Int32</span></span>|<span data-ttu-id="45f60-164">準拠していないユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="45f60-164">Number of non compliant users.</span></span>|
|<span data-ttu-id="45f60-165">remediatedUserCount</span><span class="sxs-lookup"><span data-stu-id="45f60-165">remediatedUserCount</span></span>|<span data-ttu-id="45f60-166">Int32</span><span class="sxs-lookup"><span data-stu-id="45f60-166">Int32</span></span>|<span data-ttu-id="45f60-167">修復済みユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="45f60-167">Number of remediated users.</span></span>|
|<span data-ttu-id="45f60-168">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="45f60-168">errorUserCount</span></span>|<span data-ttu-id="45f60-169">Int32</span><span class="sxs-lookup"><span data-stu-id="45f60-169">Int32</span></span>|<span data-ttu-id="45f60-170">エラーが発生したユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="45f60-170">Number of users had error.</span></span>|
|<span data-ttu-id="45f60-171">unknownUserCount</span><span class="sxs-lookup"><span data-stu-id="45f60-171">unknownUserCount</span></span>|<span data-ttu-id="45f60-172">Int32</span><span class="sxs-lookup"><span data-stu-id="45f60-172">Int32</span></span>|<span data-ttu-id="45f60-173">不明なユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="45f60-173">Number of unknown users.</span></span>|
|<span data-ttu-id="45f60-174">conflictUserCount</span><span class="sxs-lookup"><span data-stu-id="45f60-174">conflictUserCount</span></span>|<span data-ttu-id="45f60-175">Int32</span><span class="sxs-lookup"><span data-stu-id="45f60-175">Int32</span></span>|<span data-ttu-id="45f60-176">競合ユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="45f60-176">Number of conflict users.</span></span>|
|<span data-ttu-id="45f60-177">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="45f60-177">notApplicableUserCount</span></span>|<span data-ttu-id="45f60-178">Int32</span><span class="sxs-lookup"><span data-stu-id="45f60-178">Int32</span></span>|<span data-ttu-id="45f60-179">該当しないユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="45f60-179">Number of not applicable users.</span></span>|



## <a name="response"></a><span data-ttu-id="45f60-180">応答</span><span class="sxs-lookup"><span data-stu-id="45f60-180">Response</span></span>
<span data-ttu-id="45f60-181">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="45f60-181">If successful, this method returns a `200 OK` response code and an updated [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="45f60-182">例</span><span class="sxs-lookup"><span data-stu-id="45f60-182">Example</span></span>

### <a name="request"></a><span data-ttu-id="45f60-183">要求</span><span class="sxs-lookup"><span data-stu-id="45f60-183">Request</span></span>
<span data-ttu-id="45f60-184">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="45f60-184">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/softwareUpdateStatusSummary
Content-type: application/json
Content-length: 518

{
  "@odata.type": "#microsoft.graph.softwareUpdateStatusSummary",
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

### <a name="response"></a><span data-ttu-id="45f60-185">応答</span><span class="sxs-lookup"><span data-stu-id="45f60-185">Response</span></span>
<span data-ttu-id="45f60-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="45f60-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




