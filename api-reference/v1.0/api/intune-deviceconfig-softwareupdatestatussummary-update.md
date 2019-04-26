---
title: softwareUpdateStatusSummary の更新
description: softwareUpdateStatusSummary オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9ea208150ac85aefb4fb3e34b4d081d02089bdee
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568125"
---
# <a name="update-softwareupdatestatussummary"></a><span data-ttu-id="a36a0-103">softwareUpdateStatusSummary の更新</span><span class="sxs-lookup"><span data-stu-id="a36a0-103">Update softwareUpdateStatusSummary</span></span>

> <span data-ttu-id="a36a0-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a36a0-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a36a0-105">[softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="a36a0-105">Update the properties of a [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a36a0-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="a36a0-106">Prerequisites</span></span>
<span data-ttu-id="a36a0-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a36a0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a36a0-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a36a0-109">Permission type</span></span>|<span data-ttu-id="a36a0-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="a36a0-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a36a0-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a36a0-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a36a0-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a36a0-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a36a0-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a36a0-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a36a0-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a36a0-114">Not supported.</span></span>|
|<span data-ttu-id="a36a0-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a36a0-115">Application</span></span>|<span data-ttu-id="a36a0-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a36a0-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a36a0-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a36a0-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/softwareUpdateStatusSummary
```

## <a name="request-headers"></a><span data-ttu-id="a36a0-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a36a0-118">Request headers</span></span>
|<span data-ttu-id="a36a0-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a36a0-119">Header</span></span>|<span data-ttu-id="a36a0-120">値</span><span class="sxs-lookup"><span data-stu-id="a36a0-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a36a0-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a36a0-121">Authorization</span></span>|<span data-ttu-id="a36a0-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="a36a0-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a36a0-123">承諾</span><span class="sxs-lookup"><span data-stu-id="a36a0-123">Accept</span></span>|<span data-ttu-id="a36a0-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a36a0-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a36a0-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="a36a0-125">Request body</span></span>
<span data-ttu-id="a36a0-126">要求本文で、[softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="a36a0-126">In the request body, supply a JSON representation for the [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object.</span></span>

<span data-ttu-id="a36a0-127">次の表に、[softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="a36a0-127">The following table shows the properties that are required when you create the [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md).</span></span>

|<span data-ttu-id="a36a0-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a36a0-128">Property</span></span>|<span data-ttu-id="a36a0-129">型</span><span class="sxs-lookup"><span data-stu-id="a36a0-129">Type</span></span>|<span data-ttu-id="a36a0-130">説明</span><span class="sxs-lookup"><span data-stu-id="a36a0-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a36a0-131">id</span><span class="sxs-lookup"><span data-stu-id="a36a0-131">id</span></span>|<span data-ttu-id="a36a0-132">String</span><span class="sxs-lookup"><span data-stu-id="a36a0-132">String</span></span>|<span data-ttu-id="a36a0-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="a36a0-133">Key of the entity.</span></span>|
|<span data-ttu-id="a36a0-134">displayName</span><span class="sxs-lookup"><span data-stu-id="a36a0-134">displayName</span></span>|<span data-ttu-id="a36a0-135">String</span><span class="sxs-lookup"><span data-stu-id="a36a0-135">String</span></span>|<span data-ttu-id="a36a0-136">ポリシーの名前。</span><span class="sxs-lookup"><span data-stu-id="a36a0-136">The name of the policy.</span></span>|
|<span data-ttu-id="a36a0-137">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a36a0-137">compliantDeviceCount</span></span>|<span data-ttu-id="a36a0-138">Int32</span><span class="sxs-lookup"><span data-stu-id="a36a0-138">Int32</span></span>|<span data-ttu-id="a36a0-139">準拠デバイスの数。</span><span class="sxs-lookup"><span data-stu-id="a36a0-139">Number of compliant devices.</span></span>|
|<span data-ttu-id="a36a0-140">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a36a0-140">nonCompliantDeviceCount</span></span>|<span data-ttu-id="a36a0-141">Int32</span><span class="sxs-lookup"><span data-stu-id="a36a0-141">Int32</span></span>|<span data-ttu-id="a36a0-142">準拠していないデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="a36a0-142">Number of non compliant devices.</span></span>|
|<span data-ttu-id="a36a0-143">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a36a0-143">remediatedDeviceCount</span></span>|<span data-ttu-id="a36a0-144">Int32</span><span class="sxs-lookup"><span data-stu-id="a36a0-144">Int32</span></span>|<span data-ttu-id="a36a0-145">修復済みデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="a36a0-145">Number of remediated devices.</span></span>|
|<span data-ttu-id="a36a0-146">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a36a0-146">errorDeviceCount</span></span>|<span data-ttu-id="a36a0-147">Int32</span><span class="sxs-lookup"><span data-stu-id="a36a0-147">Int32</span></span>|<span data-ttu-id="a36a0-148">エラーが発生したデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="a36a0-148">Number of devices had error.</span></span>|
|<span data-ttu-id="a36a0-149">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a36a0-149">unknownDeviceCount</span></span>|<span data-ttu-id="a36a0-150">Int32</span><span class="sxs-lookup"><span data-stu-id="a36a0-150">Int32</span></span>|<span data-ttu-id="a36a0-151">不明なデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="a36a0-151">Number of unknown devices.</span></span>|
|<span data-ttu-id="a36a0-152">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a36a0-152">conflictDeviceCount</span></span>|<span data-ttu-id="a36a0-153">Int32</span><span class="sxs-lookup"><span data-stu-id="a36a0-153">Int32</span></span>|<span data-ttu-id="a36a0-154">競合デバイスの数。</span><span class="sxs-lookup"><span data-stu-id="a36a0-154">Number of conflict devices.</span></span>|
|<span data-ttu-id="a36a0-155">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a36a0-155">notApplicableDeviceCount</span></span>|<span data-ttu-id="a36a0-156">Int32</span><span class="sxs-lookup"><span data-stu-id="a36a0-156">Int32</span></span>|<span data-ttu-id="a36a0-157">該当しないデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="a36a0-157">Number of not applicable devices.</span></span>|
|<span data-ttu-id="a36a0-158">compliantUserCount</span><span class="sxs-lookup"><span data-stu-id="a36a0-158">compliantUserCount</span></span>|<span data-ttu-id="a36a0-159">Int32</span><span class="sxs-lookup"><span data-stu-id="a36a0-159">Int32</span></span>|<span data-ttu-id="a36a0-160">準拠ユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="a36a0-160">Number of compliant users.</span></span>|
|<span data-ttu-id="a36a0-161">nonCompliantUserCount</span><span class="sxs-lookup"><span data-stu-id="a36a0-161">nonCompliantUserCount</span></span>|<span data-ttu-id="a36a0-162">Int32</span><span class="sxs-lookup"><span data-stu-id="a36a0-162">Int32</span></span>|<span data-ttu-id="a36a0-163">準拠していないユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="a36a0-163">Number of non compliant users.</span></span>|
|<span data-ttu-id="a36a0-164">remediatedUserCount</span><span class="sxs-lookup"><span data-stu-id="a36a0-164">remediatedUserCount</span></span>|<span data-ttu-id="a36a0-165">Int32</span><span class="sxs-lookup"><span data-stu-id="a36a0-165">Int32</span></span>|<span data-ttu-id="a36a0-166">修復済みユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="a36a0-166">Number of remediated users.</span></span>|
|<span data-ttu-id="a36a0-167">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="a36a0-167">errorUserCount</span></span>|<span data-ttu-id="a36a0-168">Int32</span><span class="sxs-lookup"><span data-stu-id="a36a0-168">Int32</span></span>|<span data-ttu-id="a36a0-169">エラーが発生したユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="a36a0-169">Number of users had error.</span></span>|
|<span data-ttu-id="a36a0-170">unknownUserCount</span><span class="sxs-lookup"><span data-stu-id="a36a0-170">unknownUserCount</span></span>|<span data-ttu-id="a36a0-171">Int32</span><span class="sxs-lookup"><span data-stu-id="a36a0-171">Int32</span></span>|<span data-ttu-id="a36a0-172">不明なユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="a36a0-172">Number of unknown users.</span></span>|
|<span data-ttu-id="a36a0-173">conflictUserCount</span><span class="sxs-lookup"><span data-stu-id="a36a0-173">conflictUserCount</span></span>|<span data-ttu-id="a36a0-174">Int32</span><span class="sxs-lookup"><span data-stu-id="a36a0-174">Int32</span></span>|<span data-ttu-id="a36a0-175">競合ユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="a36a0-175">Number of conflict users.</span></span>|
|<span data-ttu-id="a36a0-176">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="a36a0-176">notApplicableUserCount</span></span>|<span data-ttu-id="a36a0-177">Int32</span><span class="sxs-lookup"><span data-stu-id="a36a0-177">Int32</span></span>|<span data-ttu-id="a36a0-178">該当しないユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="a36a0-178">Number of not applicable users.</span></span>|



## <a name="response"></a><span data-ttu-id="a36a0-179">応答</span><span class="sxs-lookup"><span data-stu-id="a36a0-179">Response</span></span>
<span data-ttu-id="a36a0-180">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="a36a0-180">If successful, this method returns a `200 OK` response code and an updated [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a36a0-181">例</span><span class="sxs-lookup"><span data-stu-id="a36a0-181">Example</span></span>

### <a name="request"></a><span data-ttu-id="a36a0-182">要求</span><span class="sxs-lookup"><span data-stu-id="a36a0-182">Request</span></span>
<span data-ttu-id="a36a0-183">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a36a0-183">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a36a0-184">応答</span><span class="sxs-lookup"><span data-stu-id="a36a0-184">Response</span></span>
<span data-ttu-id="a36a0-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a36a0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



