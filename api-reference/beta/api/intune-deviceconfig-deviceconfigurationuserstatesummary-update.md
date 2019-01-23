---
title: DeviceConfigurationUserStateSummary を更新します。
description: DeviceConfigurationUserStateSummary オブジェクトのプロパティを更新します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 425ac4f2697363f92f61bdd627172fd074bf94b6
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29420662"
---
# <a name="update-deviceconfigurationuserstatesummary"></a><span data-ttu-id="18b80-103">DeviceConfigurationUserStateSummary を更新します。</span><span class="sxs-lookup"><span data-stu-id="18b80-103">Update deviceConfigurationUserStateSummary</span></span>

> <span data-ttu-id="18b80-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="18b80-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="18b80-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="18b80-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="18b80-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="18b80-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="18b80-107">[DeviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="18b80-107">Update the properties of a [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="18b80-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="18b80-108">Prerequisites</span></span>
<span data-ttu-id="18b80-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="18b80-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="18b80-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="18b80-111">Permission type</span></span>|<span data-ttu-id="18b80-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="18b80-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="18b80-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="18b80-113">Delegated (work or school account)</span></span>|<span data-ttu-id="18b80-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18b80-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="18b80-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="18b80-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="18b80-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="18b80-116">Not supported.</span></span>|
|<span data-ttu-id="18b80-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="18b80-117">Application</span></span>|<span data-ttu-id="18b80-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="18b80-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="18b80-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="18b80-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationUserStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="18b80-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="18b80-120">Request headers</span></span>
|<span data-ttu-id="18b80-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="18b80-121">Header</span></span>|<span data-ttu-id="18b80-122">値</span><span class="sxs-lookup"><span data-stu-id="18b80-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="18b80-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="18b80-123">Authorization</span></span>|<span data-ttu-id="18b80-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="18b80-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="18b80-125">Accept</span><span class="sxs-lookup"><span data-stu-id="18b80-125">Accept</span></span>|<span data-ttu-id="18b80-126">application/json</span><span class="sxs-lookup"><span data-stu-id="18b80-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="18b80-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="18b80-127">Request body</span></span>
<span data-ttu-id="18b80-128">要求の本文に[deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="18b80-128">In the request body, supply a JSON representation for the [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) object.</span></span>

<span data-ttu-id="18b80-129">[DeviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="18b80-129">The following table shows the properties that are required when you create the [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md).</span></span>

|<span data-ttu-id="18b80-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="18b80-130">Property</span></span>|<span data-ttu-id="18b80-131">型</span><span class="sxs-lookup"><span data-stu-id="18b80-131">Type</span></span>|<span data-ttu-id="18b80-132">説明</span><span class="sxs-lookup"><span data-stu-id="18b80-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="18b80-133">id</span><span class="sxs-lookup"><span data-stu-id="18b80-133">id</span></span>|<span data-ttu-id="18b80-134">String</span><span class="sxs-lookup"><span data-stu-id="18b80-134">String</span></span>|<span data-ttu-id="18b80-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="18b80-135">Key of the entity.</span></span>|
|<span data-ttu-id="18b80-136">unknownUserCount</span><span class="sxs-lookup"><span data-stu-id="18b80-136">unknownUserCount</span></span>|<span data-ttu-id="18b80-137">Int32</span><span class="sxs-lookup"><span data-stu-id="18b80-137">Int32</span></span>|<span data-ttu-id="18b80-138">不明なユーザーの数</span><span class="sxs-lookup"><span data-stu-id="18b80-138">Number of unknown users</span></span>|
|<span data-ttu-id="18b80-139">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="18b80-139">notApplicableUserCount</span></span>|<span data-ttu-id="18b80-140">Int32</span><span class="sxs-lookup"><span data-stu-id="18b80-140">Int32</span></span>|<span data-ttu-id="18b80-141">適用されないユーザーの数</span><span class="sxs-lookup"><span data-stu-id="18b80-141">Number of not applicable users</span></span>|
|<span data-ttu-id="18b80-142">compliantUserCount</span><span class="sxs-lookup"><span data-stu-id="18b80-142">compliantUserCount</span></span>|<span data-ttu-id="18b80-143">Int32</span><span class="sxs-lookup"><span data-stu-id="18b80-143">Int32</span></span>|<span data-ttu-id="18b80-144">準拠のユーザーの数</span><span class="sxs-lookup"><span data-stu-id="18b80-144">Number of compliant users</span></span>|
|<span data-ttu-id="18b80-145">remediatedUserCount</span><span class="sxs-lookup"><span data-stu-id="18b80-145">remediatedUserCount</span></span>|<span data-ttu-id="18b80-146">Int32</span><span class="sxs-lookup"><span data-stu-id="18b80-146">Int32</span></span>|<span data-ttu-id="18b80-147">修正されたユーザーの数</span><span class="sxs-lookup"><span data-stu-id="18b80-147">Number of remediated users</span></span>|
|<span data-ttu-id="18b80-148">nonCompliantUserCount</span><span class="sxs-lookup"><span data-stu-id="18b80-148">nonCompliantUserCount</span></span>|<span data-ttu-id="18b80-149">Int32</span><span class="sxs-lookup"><span data-stu-id="18b80-149">Int32</span></span>|<span data-ttu-id="18b80-150">準拠していないユーザーの数</span><span class="sxs-lookup"><span data-stu-id="18b80-150">Number of NonCompliant users</span></span>|
|<span data-ttu-id="18b80-151">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="18b80-151">errorUserCount</span></span>|<span data-ttu-id="18b80-152">Int32</span><span class="sxs-lookup"><span data-stu-id="18b80-152">Int32</span></span>|<span data-ttu-id="18b80-153">エラー ユーザーの数</span><span class="sxs-lookup"><span data-stu-id="18b80-153">Number of error users</span></span>|
|<span data-ttu-id="18b80-154">conflictUserCount</span><span class="sxs-lookup"><span data-stu-id="18b80-154">conflictUserCount</span></span>|<span data-ttu-id="18b80-155">Int32</span><span class="sxs-lookup"><span data-stu-id="18b80-155">Int32</span></span>|<span data-ttu-id="18b80-156">競合ユーザーの数</span><span class="sxs-lookup"><span data-stu-id="18b80-156">Number of conflict users</span></span>|



## <a name="response"></a><span data-ttu-id="18b80-157">応答</span><span class="sxs-lookup"><span data-stu-id="18b80-157">Response</span></span>
<span data-ttu-id="18b80-158">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="18b80-158">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="18b80-159">例</span><span class="sxs-lookup"><span data-stu-id="18b80-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="18b80-160">要求</span><span class="sxs-lookup"><span data-stu-id="18b80-160">Request</span></span>
<span data-ttu-id="18b80-161">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="18b80-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationUserStateSummaries
Content-type: application/json
Content-length: 275

{
  "@odata.type": "#microsoft.graph.deviceConfigurationUserStateSummary",
  "unknownUserCount": 0,
  "notApplicableUserCount": 6,
  "compliantUserCount": 2,
  "remediatedUserCount": 3,
  "nonCompliantUserCount": 5,
  "errorUserCount": 14,
  "conflictUserCount": 1
}
```

### <a name="response"></a><span data-ttu-id="18b80-162">応答</span><span class="sxs-lookup"><span data-stu-id="18b80-162">Response</span></span>
<span data-ttu-id="18b80-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="18b80-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 324

{
  "@odata.type": "#microsoft.graph.deviceConfigurationUserStateSummary",
  "id": "e8957887-7887-e895-8778-95e8877895e8",
  "unknownUserCount": 0,
  "notApplicableUserCount": 6,
  "compliantUserCount": 2,
  "remediatedUserCount": 3,
  "nonCompliantUserCount": 5,
  "errorUserCount": 14,
  "conflictUserCount": 1
}
```




