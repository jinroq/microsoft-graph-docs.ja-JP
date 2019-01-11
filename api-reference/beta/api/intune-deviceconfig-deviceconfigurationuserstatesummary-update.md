---
title: DeviceConfigurationUserStateSummary を更新します。
description: DeviceConfigurationUserStateSummary オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 36d9065e906a7a4da9f61b30cc4588e494389401
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27812755"
---
# <a name="update-deviceconfigurationuserstatesummary"></a><span data-ttu-id="c89c1-103">DeviceConfigurationUserStateSummary を更新します。</span><span class="sxs-lookup"><span data-stu-id="c89c1-103">Update deviceConfigurationUserStateSummary</span></span>

> <span data-ttu-id="c89c1-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c89c1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c89c1-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c89c1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c89c1-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="c89c1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c89c1-107">[DeviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="c89c1-107">Update the properties of a [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c89c1-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="c89c1-108">Prerequisites</span></span>
<span data-ttu-id="c89c1-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c89c1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c89c1-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c89c1-111">Permission type</span></span>|<span data-ttu-id="c89c1-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="c89c1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c89c1-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c89c1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c89c1-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c89c1-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c89c1-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c89c1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c89c1-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c89c1-116">Not supported.</span></span>|
|<span data-ttu-id="c89c1-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c89c1-117">Application</span></span>|<span data-ttu-id="c89c1-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c89c1-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c89c1-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c89c1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationUserStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="c89c1-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c89c1-120">Request headers</span></span>
|<span data-ttu-id="c89c1-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c89c1-121">Header</span></span>|<span data-ttu-id="c89c1-122">値</span><span class="sxs-lookup"><span data-stu-id="c89c1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c89c1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c89c1-123">Authorization</span></span>|<span data-ttu-id="c89c1-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="c89c1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c89c1-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c89c1-125">Accept</span></span>|<span data-ttu-id="c89c1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c89c1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c89c1-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="c89c1-127">Request body</span></span>
<span data-ttu-id="c89c1-128">要求の本文に[deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="c89c1-128">In the request body, supply a JSON representation for the [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) object.</span></span>

<span data-ttu-id="c89c1-129">[DeviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="c89c1-129">The following table shows the properties that are required when you create the [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md).</span></span>

|<span data-ttu-id="c89c1-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c89c1-130">Property</span></span>|<span data-ttu-id="c89c1-131">種類</span><span class="sxs-lookup"><span data-stu-id="c89c1-131">Type</span></span>|<span data-ttu-id="c89c1-132">説明</span><span class="sxs-lookup"><span data-stu-id="c89c1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c89c1-133">ID</span><span class="sxs-lookup"><span data-stu-id="c89c1-133">id</span></span>|<span data-ttu-id="c89c1-134">String</span><span class="sxs-lookup"><span data-stu-id="c89c1-134">String</span></span>|<span data-ttu-id="c89c1-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="c89c1-135">Key of the entity.</span></span>|
|<span data-ttu-id="c89c1-136">unknownUserCount</span><span class="sxs-lookup"><span data-stu-id="c89c1-136">unknownUserCount</span></span>|<span data-ttu-id="c89c1-137">Int32</span><span class="sxs-lookup"><span data-stu-id="c89c1-137">Int32</span></span>|<span data-ttu-id="c89c1-138">不明なユーザーの数</span><span class="sxs-lookup"><span data-stu-id="c89c1-138">Number of unknown users</span></span>|
|<span data-ttu-id="c89c1-139">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="c89c1-139">notApplicableUserCount</span></span>|<span data-ttu-id="c89c1-140">Int32</span><span class="sxs-lookup"><span data-stu-id="c89c1-140">Int32</span></span>|<span data-ttu-id="c89c1-141">適用されないユーザーの数</span><span class="sxs-lookup"><span data-stu-id="c89c1-141">Number of not applicable users</span></span>|
|<span data-ttu-id="c89c1-142">compliantUserCount</span><span class="sxs-lookup"><span data-stu-id="c89c1-142">compliantUserCount</span></span>|<span data-ttu-id="c89c1-143">Int32</span><span class="sxs-lookup"><span data-stu-id="c89c1-143">Int32</span></span>|<span data-ttu-id="c89c1-144">準拠のユーザーの数</span><span class="sxs-lookup"><span data-stu-id="c89c1-144">Number of compliant users</span></span>|
|<span data-ttu-id="c89c1-145">remediatedUserCount</span><span class="sxs-lookup"><span data-stu-id="c89c1-145">remediatedUserCount</span></span>|<span data-ttu-id="c89c1-146">Int32</span><span class="sxs-lookup"><span data-stu-id="c89c1-146">Int32</span></span>|<span data-ttu-id="c89c1-147">修正されたユーザーの数</span><span class="sxs-lookup"><span data-stu-id="c89c1-147">Number of remediated users</span></span>|
|<span data-ttu-id="c89c1-148">nonCompliantUserCount</span><span class="sxs-lookup"><span data-stu-id="c89c1-148">nonCompliantUserCount</span></span>|<span data-ttu-id="c89c1-149">Int32</span><span class="sxs-lookup"><span data-stu-id="c89c1-149">Int32</span></span>|<span data-ttu-id="c89c1-150">準拠していないユーザーの数</span><span class="sxs-lookup"><span data-stu-id="c89c1-150">Number of NonCompliant users</span></span>|
|<span data-ttu-id="c89c1-151">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="c89c1-151">errorUserCount</span></span>|<span data-ttu-id="c89c1-152">Int32</span><span class="sxs-lookup"><span data-stu-id="c89c1-152">Int32</span></span>|<span data-ttu-id="c89c1-153">エラー ユーザーの数</span><span class="sxs-lookup"><span data-stu-id="c89c1-153">Number of error users</span></span>|
|<span data-ttu-id="c89c1-154">conflictUserCount</span><span class="sxs-lookup"><span data-stu-id="c89c1-154">conflictUserCount</span></span>|<span data-ttu-id="c89c1-155">Int32</span><span class="sxs-lookup"><span data-stu-id="c89c1-155">Int32</span></span>|<span data-ttu-id="c89c1-156">競合ユーザーの数</span><span class="sxs-lookup"><span data-stu-id="c89c1-156">Number of conflict users</span></span>|



## <a name="response"></a><span data-ttu-id="c89c1-157">応答</span><span class="sxs-lookup"><span data-stu-id="c89c1-157">Response</span></span>
<span data-ttu-id="c89c1-158">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="c89c1-158">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c89c1-159">例</span><span class="sxs-lookup"><span data-stu-id="c89c1-159">Example</span></span>
### <a name="request"></a><span data-ttu-id="c89c1-160">要求</span><span class="sxs-lookup"><span data-stu-id="c89c1-160">Request</span></span>
<span data-ttu-id="c89c1-161">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c89c1-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationUserStateSummaries
Content-type: application/json
Content-length: 201

{
  "unknownUserCount": 0,
  "notApplicableUserCount": 6,
  "compliantUserCount": 2,
  "remediatedUserCount": 3,
  "nonCompliantUserCount": 5,
  "errorUserCount": 14,
  "conflictUserCount": 1
}
```

### <a name="response"></a><span data-ttu-id="c89c1-162">応答</span><span class="sxs-lookup"><span data-stu-id="c89c1-162">Response</span></span>
<span data-ttu-id="c89c1-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c89c1-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





