---
title: softwareUpdateStatusSummary の更新
description: softwareUpdateStatusSummary オブジェクトのプロパティを更新します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 0140d0035c05182a22264d36bf3c87db18760a19
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29416203"
---
# <a name="update-softwareupdatestatussummary"></a><span data-ttu-id="16c8a-103">softwareUpdateStatusSummary の更新</span><span class="sxs-lookup"><span data-stu-id="16c8a-103">Update softwareUpdateStatusSummary</span></span>

> <span data-ttu-id="16c8a-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="16c8a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="16c8a-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="16c8a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="16c8a-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="16c8a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="16c8a-107">[softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="16c8a-107">Update the properties of a [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="16c8a-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="16c8a-108">Prerequisites</span></span>
<span data-ttu-id="16c8a-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="16c8a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="16c8a-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="16c8a-111">Permission type</span></span>|<span data-ttu-id="16c8a-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="16c8a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="16c8a-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="16c8a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="16c8a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16c8a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="16c8a-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="16c8a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="16c8a-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="16c8a-116">Not supported.</span></span>|
|<span data-ttu-id="16c8a-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="16c8a-117">Application</span></span>|<span data-ttu-id="16c8a-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="16c8a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="16c8a-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="16c8a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/softwareUpdateStatusSummary
```

## <a name="request-headers"></a><span data-ttu-id="16c8a-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="16c8a-120">Request headers</span></span>
|<span data-ttu-id="16c8a-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="16c8a-121">Header</span></span>|<span data-ttu-id="16c8a-122">値</span><span class="sxs-lookup"><span data-stu-id="16c8a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="16c8a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="16c8a-123">Authorization</span></span>|<span data-ttu-id="16c8a-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="16c8a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="16c8a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="16c8a-125">Accept</span></span>|<span data-ttu-id="16c8a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="16c8a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="16c8a-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="16c8a-127">Request body</span></span>
<span data-ttu-id="16c8a-128">要求本文で、[softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="16c8a-128">In the request body, supply a JSON representation for the [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object.</span></span>

<span data-ttu-id="16c8a-129">次の表に、[softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="16c8a-129">The following table shows the properties that are required when you create the [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md).</span></span>

|<span data-ttu-id="16c8a-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="16c8a-130">Property</span></span>|<span data-ttu-id="16c8a-131">型</span><span class="sxs-lookup"><span data-stu-id="16c8a-131">Type</span></span>|<span data-ttu-id="16c8a-132">説明</span><span class="sxs-lookup"><span data-stu-id="16c8a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="16c8a-133">id</span><span class="sxs-lookup"><span data-stu-id="16c8a-133">id</span></span>|<span data-ttu-id="16c8a-134">String</span><span class="sxs-lookup"><span data-stu-id="16c8a-134">String</span></span>|<span data-ttu-id="16c8a-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="16c8a-135">Key of the entity.</span></span>|
|<span data-ttu-id="16c8a-136">displayName</span><span class="sxs-lookup"><span data-stu-id="16c8a-136">displayName</span></span>|<span data-ttu-id="16c8a-137">String</span><span class="sxs-lookup"><span data-stu-id="16c8a-137">String</span></span>|<span data-ttu-id="16c8a-138">ポリシーの名前。</span><span class="sxs-lookup"><span data-stu-id="16c8a-138">The name of the policy.</span></span>|
|<span data-ttu-id="16c8a-139">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="16c8a-139">compliantDeviceCount</span></span>|<span data-ttu-id="16c8a-140">Int32</span><span class="sxs-lookup"><span data-stu-id="16c8a-140">Int32</span></span>|<span data-ttu-id="16c8a-141">準拠デバイスの数。</span><span class="sxs-lookup"><span data-stu-id="16c8a-141">Number of compliant devices.</span></span>|
|<span data-ttu-id="16c8a-142">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="16c8a-142">nonCompliantDeviceCount</span></span>|<span data-ttu-id="16c8a-143">Int32</span><span class="sxs-lookup"><span data-stu-id="16c8a-143">Int32</span></span>|<span data-ttu-id="16c8a-144">準拠していないデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="16c8a-144">Number of non compliant devices.</span></span>|
|<span data-ttu-id="16c8a-145">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="16c8a-145">remediatedDeviceCount</span></span>|<span data-ttu-id="16c8a-146">Int32</span><span class="sxs-lookup"><span data-stu-id="16c8a-146">Int32</span></span>|<span data-ttu-id="16c8a-147">修復済みデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="16c8a-147">Number of remediated devices.</span></span>|
|<span data-ttu-id="16c8a-148">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="16c8a-148">errorDeviceCount</span></span>|<span data-ttu-id="16c8a-149">Int32</span><span class="sxs-lookup"><span data-stu-id="16c8a-149">Int32</span></span>|<span data-ttu-id="16c8a-150">エラーが発生したデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="16c8a-150">Number of devices had error.</span></span>|
|<span data-ttu-id="16c8a-151">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="16c8a-151">unknownDeviceCount</span></span>|<span data-ttu-id="16c8a-152">Int32</span><span class="sxs-lookup"><span data-stu-id="16c8a-152">Int32</span></span>|<span data-ttu-id="16c8a-153">不明なデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="16c8a-153">Number of unknown devices.</span></span>|
|<span data-ttu-id="16c8a-154">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="16c8a-154">conflictDeviceCount</span></span>|<span data-ttu-id="16c8a-155">Int32</span><span class="sxs-lookup"><span data-stu-id="16c8a-155">Int32</span></span>|<span data-ttu-id="16c8a-156">競合デバイスの数。</span><span class="sxs-lookup"><span data-stu-id="16c8a-156">Number of conflict devices.</span></span>|
|<span data-ttu-id="16c8a-157">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="16c8a-157">notApplicableDeviceCount</span></span>|<span data-ttu-id="16c8a-158">Int32</span><span class="sxs-lookup"><span data-stu-id="16c8a-158">Int32</span></span>|<span data-ttu-id="16c8a-159">該当しないデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="16c8a-159">Number of not applicable devices.</span></span>|
|<span data-ttu-id="16c8a-160">compliantUserCount</span><span class="sxs-lookup"><span data-stu-id="16c8a-160">compliantUserCount</span></span>|<span data-ttu-id="16c8a-161">Int32</span><span class="sxs-lookup"><span data-stu-id="16c8a-161">Int32</span></span>|<span data-ttu-id="16c8a-162">準拠ユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="16c8a-162">Number of compliant users.</span></span>|
|<span data-ttu-id="16c8a-163">nonCompliantUserCount</span><span class="sxs-lookup"><span data-stu-id="16c8a-163">nonCompliantUserCount</span></span>|<span data-ttu-id="16c8a-164">Int32</span><span class="sxs-lookup"><span data-stu-id="16c8a-164">Int32</span></span>|<span data-ttu-id="16c8a-165">準拠していないユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="16c8a-165">Number of non compliant users.</span></span>|
|<span data-ttu-id="16c8a-166">remediatedUserCount</span><span class="sxs-lookup"><span data-stu-id="16c8a-166">remediatedUserCount</span></span>|<span data-ttu-id="16c8a-167">Int32</span><span class="sxs-lookup"><span data-stu-id="16c8a-167">Int32</span></span>|<span data-ttu-id="16c8a-168">修復済みユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="16c8a-168">Number of remediated users.</span></span>|
|<span data-ttu-id="16c8a-169">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="16c8a-169">errorUserCount</span></span>|<span data-ttu-id="16c8a-170">Int32</span><span class="sxs-lookup"><span data-stu-id="16c8a-170">Int32</span></span>|<span data-ttu-id="16c8a-171">エラーが発生したユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="16c8a-171">Number of users had error.</span></span>|
|<span data-ttu-id="16c8a-172">unknownUserCount</span><span class="sxs-lookup"><span data-stu-id="16c8a-172">unknownUserCount</span></span>|<span data-ttu-id="16c8a-173">Int32</span><span class="sxs-lookup"><span data-stu-id="16c8a-173">Int32</span></span>|<span data-ttu-id="16c8a-174">不明なユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="16c8a-174">Number of unknown users.</span></span>|
|<span data-ttu-id="16c8a-175">conflictUserCount</span><span class="sxs-lookup"><span data-stu-id="16c8a-175">conflictUserCount</span></span>|<span data-ttu-id="16c8a-176">Int32</span><span class="sxs-lookup"><span data-stu-id="16c8a-176">Int32</span></span>|<span data-ttu-id="16c8a-177">競合ユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="16c8a-177">Number of conflict users.</span></span>|
|<span data-ttu-id="16c8a-178">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="16c8a-178">notApplicableUserCount</span></span>|<span data-ttu-id="16c8a-179">Int32</span><span class="sxs-lookup"><span data-stu-id="16c8a-179">Int32</span></span>|<span data-ttu-id="16c8a-180">該当しないユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="16c8a-180">Number of not applicable users.</span></span>|



## <a name="response"></a><span data-ttu-id="16c8a-181">応答</span><span class="sxs-lookup"><span data-stu-id="16c8a-181">Response</span></span>
<span data-ttu-id="16c8a-182">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="16c8a-182">If successful, this method returns a `200 OK` response code and an updated [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="16c8a-183">例</span><span class="sxs-lookup"><span data-stu-id="16c8a-183">Example</span></span>

### <a name="request"></a><span data-ttu-id="16c8a-184">要求</span><span class="sxs-lookup"><span data-stu-id="16c8a-184">Request</span></span>
<span data-ttu-id="16c8a-185">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="16c8a-185">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="16c8a-186">応答</span><span class="sxs-lookup"><span data-stu-id="16c8a-186">Response</span></span>
<span data-ttu-id="16c8a-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="16c8a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




