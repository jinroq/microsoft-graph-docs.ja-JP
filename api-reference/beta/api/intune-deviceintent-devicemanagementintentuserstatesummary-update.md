---
title: DeviceManagementIntentUserStateSummary の更新
description: DeviceManagementIntentUserStateSummary オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7eb98c9c77c5bc8cecef7994fd2913111bd913fb
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33915762"
---
# <a name="update-devicemanagementintentuserstatesummary"></a><span data-ttu-id="90aa4-103">DeviceManagementIntentUserStateSummary の更新</span><span class="sxs-lookup"><span data-stu-id="90aa4-103">Update deviceManagementIntentUserStateSummary</span></span>

> <span data-ttu-id="90aa4-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="90aa4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="90aa4-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="90aa4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="90aa4-106">[DeviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="90aa4-106">Update the properties of a [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="90aa4-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="90aa4-107">Prerequisites</span></span>
<span data-ttu-id="90aa4-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="90aa4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="90aa4-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="90aa4-110">Permission type</span></span>|<span data-ttu-id="90aa4-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="90aa4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="90aa4-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="90aa4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="90aa4-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90aa4-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="90aa4-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="90aa4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="90aa4-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="90aa4-115">Not supported.</span></span>|
|<span data-ttu-id="90aa4-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="90aa4-116">Application</span></span>|<span data-ttu-id="90aa4-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="90aa4-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="90aa4-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="90aa4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intents/{deviceManagementIntentId}/userStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="90aa4-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="90aa4-119">Request headers</span></span>
|<span data-ttu-id="90aa4-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="90aa4-120">Header</span></span>|<span data-ttu-id="90aa4-121">値</span><span class="sxs-lookup"><span data-stu-id="90aa4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="90aa4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="90aa4-122">Authorization</span></span>|<span data-ttu-id="90aa4-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="90aa4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="90aa4-124">承諾</span><span class="sxs-lookup"><span data-stu-id="90aa4-124">Accept</span></span>|<span data-ttu-id="90aa4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="90aa4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="90aa4-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="90aa4-126">Request body</span></span>
<span data-ttu-id="90aa4-127">要求本文で、 [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="90aa4-127">In the request body, supply a JSON representation for the [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) object.</span></span>

<span data-ttu-id="90aa4-128">次の表に、 [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="90aa4-128">The following table shows the properties that are required when you create the [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md).</span></span>

|<span data-ttu-id="90aa4-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="90aa4-129">Property</span></span>|<span data-ttu-id="90aa4-130">型</span><span class="sxs-lookup"><span data-stu-id="90aa4-130">Type</span></span>|<span data-ttu-id="90aa4-131">説明</span><span class="sxs-lookup"><span data-stu-id="90aa4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="90aa4-132">id</span><span class="sxs-lookup"><span data-stu-id="90aa4-132">id</span></span>|<span data-ttu-id="90aa4-133">String</span><span class="sxs-lookup"><span data-stu-id="90aa4-133">String</span></span>|<span data-ttu-id="90aa4-134">ID</span><span class="sxs-lookup"><span data-stu-id="90aa4-134">The ID</span></span>|
|<span data-ttu-id="90aa4-135">conflictCount</span><span class="sxs-lookup"><span data-stu-id="90aa4-135">conflictCount</span></span>|<span data-ttu-id="90aa4-136">Int32</span><span class="sxs-lookup"><span data-stu-id="90aa4-136">Int32</span></span>|<span data-ttu-id="90aa4-137">競合しているユーザーの数</span><span class="sxs-lookup"><span data-stu-id="90aa4-137">Number of users in conflict</span></span>|
|<span data-ttu-id="90aa4-138">errorCount</span><span class="sxs-lookup"><span data-stu-id="90aa4-138">errorCount</span></span>|<span data-ttu-id="90aa4-139">Int32</span><span class="sxs-lookup"><span data-stu-id="90aa4-139">Int32</span></span>|<span data-ttu-id="90aa4-140">エラーが発生したユーザーの数</span><span class="sxs-lookup"><span data-stu-id="90aa4-140">Number of error users</span></span>|
|<span data-ttu-id="90aa4-141">failedCount</span><span class="sxs-lookup"><span data-stu-id="90aa4-141">failedCount</span></span>|<span data-ttu-id="90aa4-142">Int32</span><span class="sxs-lookup"><span data-stu-id="90aa4-142">Int32</span></span>|<span data-ttu-id="90aa4-143">失敗したユーザーの数</span><span class="sxs-lookup"><span data-stu-id="90aa4-143">Number of failed users</span></span>|
|<span data-ttu-id="90aa4-144">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="90aa4-144">notApplicableCount</span></span>|<span data-ttu-id="90aa4-145">Int32</span><span class="sxs-lookup"><span data-stu-id="90aa4-145">Int32</span></span>|<span data-ttu-id="90aa4-146">該当しないユーザーの数</span><span class="sxs-lookup"><span data-stu-id="90aa4-146">Number of not applicable users</span></span>|
|<span data-ttu-id="90aa4-147">successCount</span><span class="sxs-lookup"><span data-stu-id="90aa4-147">successCount</span></span>|<span data-ttu-id="90aa4-148">Int32</span><span class="sxs-lookup"><span data-stu-id="90aa4-148">Int32</span></span>|<span data-ttu-id="90aa4-149">成功したユーザーの数</span><span class="sxs-lookup"><span data-stu-id="90aa4-149">Number of succeeded users</span></span>|



## <a name="response"></a><span data-ttu-id="90aa4-150">応答</span><span class="sxs-lookup"><span data-stu-id="90aa4-150">Response</span></span>
<span data-ttu-id="90aa4-151">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="90aa4-151">If successful, this method returns a `200 OK` response code and an updated [deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="90aa4-152">例</span><span class="sxs-lookup"><span data-stu-id="90aa4-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="90aa4-153">要求</span><span class="sxs-lookup"><span data-stu-id="90aa4-153">Request</span></span>
<span data-ttu-id="90aa4-154">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="90aa4-154">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/userStateSummary
Content-type: application/json
Content-length: 198

{
  "@odata.type": "#microsoft.graph.deviceManagementIntentUserStateSummary",
  "conflictCount": 13,
  "errorCount": 10,
  "failedCount": 11,
  "notApplicableCount": 2,
  "successCount": 12
}
```

### <a name="response"></a><span data-ttu-id="90aa4-155">応答</span><span class="sxs-lookup"><span data-stu-id="90aa4-155">Response</span></span>
<span data-ttu-id="90aa4-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="90aa4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 247

{
  "@odata.type": "#microsoft.graph.deviceManagementIntentUserStateSummary",
  "id": "be567e02-7e02-be56-027e-56be027e56be",
  "conflictCount": 13,
  "errorCount": 10,
  "failedCount": 11,
  "notApplicableCount": 2,
  "successCount": 12
}
```




