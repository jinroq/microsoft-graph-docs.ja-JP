---
title: softwareUpdateStatusSummary の更新
description: softwareUpdateStatusSummary オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 230d850e5bb747bf2c5c1b471daf33590642de61
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30260439"
---
# <a name="update-softwareupdatestatussummary"></a><span data-ttu-id="a0130-103">softwareUpdateStatusSummary の更新</span><span class="sxs-lookup"><span data-stu-id="a0130-103">Update softwareUpdateStatusSummary</span></span>

> <span data-ttu-id="a0130-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a0130-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a0130-105">[softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="a0130-105">Update the properties of a [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a0130-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="a0130-106">Prerequisites</span></span>
<span data-ttu-id="a0130-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a0130-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a0130-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a0130-109">Permission type</span></span>|<span data-ttu-id="a0130-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="a0130-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a0130-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a0130-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a0130-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0130-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a0130-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a0130-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a0130-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a0130-114">Not supported.</span></span>|
|<span data-ttu-id="a0130-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a0130-115">Application</span></span>|<span data-ttu-id="a0130-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a0130-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a0130-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a0130-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/softwareUpdateStatusSummary
```

## <a name="request-headers"></a><span data-ttu-id="a0130-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a0130-118">Request headers</span></span>
|<span data-ttu-id="a0130-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a0130-119">Header</span></span>|<span data-ttu-id="a0130-120">値</span><span class="sxs-lookup"><span data-stu-id="a0130-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a0130-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a0130-121">Authorization</span></span>|<span data-ttu-id="a0130-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="a0130-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a0130-123">承諾</span><span class="sxs-lookup"><span data-stu-id="a0130-123">Accept</span></span>|<span data-ttu-id="a0130-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a0130-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a0130-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="a0130-125">Request body</span></span>
<span data-ttu-id="a0130-126">要求本文で、[softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="a0130-126">In the request body, supply a JSON representation for the [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object.</span></span>

<span data-ttu-id="a0130-127">次の表に、[softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="a0130-127">The following table shows the properties that are required when you create the [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md).</span></span>

|<span data-ttu-id="a0130-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a0130-128">Property</span></span>|<span data-ttu-id="a0130-129">型</span><span class="sxs-lookup"><span data-stu-id="a0130-129">Type</span></span>|<span data-ttu-id="a0130-130">説明</span><span class="sxs-lookup"><span data-stu-id="a0130-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a0130-131">id</span><span class="sxs-lookup"><span data-stu-id="a0130-131">id</span></span>|<span data-ttu-id="a0130-132">String</span><span class="sxs-lookup"><span data-stu-id="a0130-132">String</span></span>|<span data-ttu-id="a0130-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="a0130-133">Key of the entity.</span></span>|
|<span data-ttu-id="a0130-134">displayName</span><span class="sxs-lookup"><span data-stu-id="a0130-134">displayName</span></span>|<span data-ttu-id="a0130-135">String</span><span class="sxs-lookup"><span data-stu-id="a0130-135">String</span></span>|<span data-ttu-id="a0130-136">ポリシーの名前。</span><span class="sxs-lookup"><span data-stu-id="a0130-136">The name of the policy.</span></span>|
|<span data-ttu-id="a0130-137">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a0130-137">compliantDeviceCount</span></span>|<span data-ttu-id="a0130-138">Int32</span><span class="sxs-lookup"><span data-stu-id="a0130-138">Int32</span></span>|<span data-ttu-id="a0130-139">準拠デバイスの数。</span><span class="sxs-lookup"><span data-stu-id="a0130-139">Number of compliant devices.</span></span>|
|<span data-ttu-id="a0130-140">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a0130-140">nonCompliantDeviceCount</span></span>|<span data-ttu-id="a0130-141">Int32</span><span class="sxs-lookup"><span data-stu-id="a0130-141">Int32</span></span>|<span data-ttu-id="a0130-142">準拠していないデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="a0130-142">Number of non compliant devices.</span></span>|
|<span data-ttu-id="a0130-143">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a0130-143">remediatedDeviceCount</span></span>|<span data-ttu-id="a0130-144">Int32</span><span class="sxs-lookup"><span data-stu-id="a0130-144">Int32</span></span>|<span data-ttu-id="a0130-145">修復済みデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="a0130-145">Number of remediated devices.</span></span>|
|<span data-ttu-id="a0130-146">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a0130-146">errorDeviceCount</span></span>|<span data-ttu-id="a0130-147">Int32</span><span class="sxs-lookup"><span data-stu-id="a0130-147">Int32</span></span>|<span data-ttu-id="a0130-148">エラーが発生したデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="a0130-148">Number of devices had error.</span></span>|
|<span data-ttu-id="a0130-149">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a0130-149">unknownDeviceCount</span></span>|<span data-ttu-id="a0130-150">Int32</span><span class="sxs-lookup"><span data-stu-id="a0130-150">Int32</span></span>|<span data-ttu-id="a0130-151">不明なデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="a0130-151">Number of unknown devices.</span></span>|
|<span data-ttu-id="a0130-152">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a0130-152">conflictDeviceCount</span></span>|<span data-ttu-id="a0130-153">Int32</span><span class="sxs-lookup"><span data-stu-id="a0130-153">Int32</span></span>|<span data-ttu-id="a0130-154">競合デバイスの数。</span><span class="sxs-lookup"><span data-stu-id="a0130-154">Number of conflict devices.</span></span>|
|<span data-ttu-id="a0130-155">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a0130-155">notApplicableDeviceCount</span></span>|<span data-ttu-id="a0130-156">Int32</span><span class="sxs-lookup"><span data-stu-id="a0130-156">Int32</span></span>|<span data-ttu-id="a0130-157">該当しないデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="a0130-157">Number of not applicable devices.</span></span>|
|<span data-ttu-id="a0130-158">compliantUserCount</span><span class="sxs-lookup"><span data-stu-id="a0130-158">compliantUserCount</span></span>|<span data-ttu-id="a0130-159">Int32</span><span class="sxs-lookup"><span data-stu-id="a0130-159">Int32</span></span>|<span data-ttu-id="a0130-160">準拠ユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="a0130-160">Number of compliant users.</span></span>|
|<span data-ttu-id="a0130-161">nonCompliantUserCount</span><span class="sxs-lookup"><span data-stu-id="a0130-161">nonCompliantUserCount</span></span>|<span data-ttu-id="a0130-162">Int32</span><span class="sxs-lookup"><span data-stu-id="a0130-162">Int32</span></span>|<span data-ttu-id="a0130-163">準拠していないユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="a0130-163">Number of non compliant users.</span></span>|
|<span data-ttu-id="a0130-164">remediatedUserCount</span><span class="sxs-lookup"><span data-stu-id="a0130-164">remediatedUserCount</span></span>|<span data-ttu-id="a0130-165">Int32</span><span class="sxs-lookup"><span data-stu-id="a0130-165">Int32</span></span>|<span data-ttu-id="a0130-166">修復済みユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="a0130-166">Number of remediated users.</span></span>|
|<span data-ttu-id="a0130-167">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="a0130-167">errorUserCount</span></span>|<span data-ttu-id="a0130-168">Int32</span><span class="sxs-lookup"><span data-stu-id="a0130-168">Int32</span></span>|<span data-ttu-id="a0130-169">エラーが発生したユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="a0130-169">Number of users had error.</span></span>|
|<span data-ttu-id="a0130-170">unknownUserCount</span><span class="sxs-lookup"><span data-stu-id="a0130-170">unknownUserCount</span></span>|<span data-ttu-id="a0130-171">Int32</span><span class="sxs-lookup"><span data-stu-id="a0130-171">Int32</span></span>|<span data-ttu-id="a0130-172">不明なユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="a0130-172">Number of unknown users.</span></span>|
|<span data-ttu-id="a0130-173">conflictUserCount</span><span class="sxs-lookup"><span data-stu-id="a0130-173">conflictUserCount</span></span>|<span data-ttu-id="a0130-174">Int32</span><span class="sxs-lookup"><span data-stu-id="a0130-174">Int32</span></span>|<span data-ttu-id="a0130-175">競合ユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="a0130-175">Number of conflict users.</span></span>|
|<span data-ttu-id="a0130-176">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="a0130-176">notApplicableUserCount</span></span>|<span data-ttu-id="a0130-177">Int32</span><span class="sxs-lookup"><span data-stu-id="a0130-177">Int32</span></span>|<span data-ttu-id="a0130-178">該当しないユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="a0130-178">Number of not applicable users.</span></span>|



## <a name="response"></a><span data-ttu-id="a0130-179">応答</span><span class="sxs-lookup"><span data-stu-id="a0130-179">Response</span></span>
<span data-ttu-id="a0130-180">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="a0130-180">If successful, this method returns a `200 OK` response code and an updated [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a0130-181">例</span><span class="sxs-lookup"><span data-stu-id="a0130-181">Example</span></span>

### <a name="request"></a><span data-ttu-id="a0130-182">要求</span><span class="sxs-lookup"><span data-stu-id="a0130-182">Request</span></span>
<span data-ttu-id="a0130-183">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a0130-183">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/softwareUpdateStatusSummary
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

### <a name="response"></a><span data-ttu-id="a0130-184">応答</span><span class="sxs-lookup"><span data-stu-id="a0130-184">Response</span></span>
<span data-ttu-id="a0130-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a0130-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



