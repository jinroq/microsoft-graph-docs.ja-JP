---
title: deviceConfigurationUserStateSummary の更新
description: deviceConfigurationUserStateSummary オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: efc16035394ec16af3b4334df2160a176332b14a
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30983744"
---
# <a name="update-deviceconfigurationuserstatesummary"></a><span data-ttu-id="29714-103">deviceConfigurationUserStateSummary の更新</span><span class="sxs-lookup"><span data-stu-id="29714-103">Update deviceConfigurationUserStateSummary</span></span>

> <span data-ttu-id="29714-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="29714-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="29714-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="29714-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="29714-106">[deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="29714-106">Update the properties of a [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="29714-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="29714-107">Prerequisites</span></span>
<span data-ttu-id="29714-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="29714-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="29714-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="29714-110">Permission type</span></span>|<span data-ttu-id="29714-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="29714-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="29714-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="29714-112">Delegated (work or school account)</span></span>|<span data-ttu-id="29714-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29714-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="29714-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="29714-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="29714-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="29714-115">Not supported.</span></span>|
|<span data-ttu-id="29714-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="29714-116">Application</span></span>|<span data-ttu-id="29714-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="29714-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="29714-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="29714-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationUserStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="29714-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="29714-119">Request headers</span></span>
|<span data-ttu-id="29714-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="29714-120">Header</span></span>|<span data-ttu-id="29714-121">値</span><span class="sxs-lookup"><span data-stu-id="29714-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="29714-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="29714-122">Authorization</span></span>|<span data-ttu-id="29714-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="29714-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="29714-124">承諾</span><span class="sxs-lookup"><span data-stu-id="29714-124">Accept</span></span>|<span data-ttu-id="29714-125">application/json</span><span class="sxs-lookup"><span data-stu-id="29714-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="29714-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="29714-126">Request body</span></span>
<span data-ttu-id="29714-127">要求本文で、 [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="29714-127">In the request body, supply a JSON representation for the [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) object.</span></span>

<span data-ttu-id="29714-128">次の表に、 [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="29714-128">The following table shows the properties that are required when you create the [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md).</span></span>

|<span data-ttu-id="29714-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="29714-129">Property</span></span>|<span data-ttu-id="29714-130">型</span><span class="sxs-lookup"><span data-stu-id="29714-130">Type</span></span>|<span data-ttu-id="29714-131">説明</span><span class="sxs-lookup"><span data-stu-id="29714-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="29714-132">id</span><span class="sxs-lookup"><span data-stu-id="29714-132">id</span></span>|<span data-ttu-id="29714-133">String</span><span class="sxs-lookup"><span data-stu-id="29714-133">String</span></span>|<span data-ttu-id="29714-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="29714-134">Key of the entity.</span></span>|
|<span data-ttu-id="29714-135">unknownUserCount</span><span class="sxs-lookup"><span data-stu-id="29714-135">unknownUserCount</span></span>|<span data-ttu-id="29714-136">Int32</span><span class="sxs-lookup"><span data-stu-id="29714-136">Int32</span></span>|<span data-ttu-id="29714-137">不明なユーザーの数</span><span class="sxs-lookup"><span data-stu-id="29714-137">Number of unknown users</span></span>|
|<span data-ttu-id="29714-138">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="29714-138">notApplicableUserCount</span></span>|<span data-ttu-id="29714-139">Int32</span><span class="sxs-lookup"><span data-stu-id="29714-139">Int32</span></span>|<span data-ttu-id="29714-140">該当しないユーザーの数</span><span class="sxs-lookup"><span data-stu-id="29714-140">Number of not applicable users</span></span>|
|<span data-ttu-id="29714-141">compliantUserCount</span><span class="sxs-lookup"><span data-stu-id="29714-141">compliantUserCount</span></span>|<span data-ttu-id="29714-142">Int32</span><span class="sxs-lookup"><span data-stu-id="29714-142">Int32</span></span>|<span data-ttu-id="29714-143">準拠しているユーザーの数</span><span class="sxs-lookup"><span data-stu-id="29714-143">Number of compliant users</span></span>|
|<span data-ttu-id="29714-144">remediatedUserCount</span><span class="sxs-lookup"><span data-stu-id="29714-144">remediatedUserCount</span></span>|<span data-ttu-id="29714-145">Int32</span><span class="sxs-lookup"><span data-stu-id="29714-145">Int32</span></span>|<span data-ttu-id="29714-146">修復したユーザーの数</span><span class="sxs-lookup"><span data-stu-id="29714-146">Number of remediated users</span></span>|
|<span data-ttu-id="29714-147">nonCompliantUserCount</span><span class="sxs-lookup"><span data-stu-id="29714-147">nonCompliantUserCount</span></span>|<span data-ttu-id="29714-148">Int32</span><span class="sxs-lookup"><span data-stu-id="29714-148">Int32</span></span>|<span data-ttu-id="29714-149">準拠していないユーザーの数</span><span class="sxs-lookup"><span data-stu-id="29714-149">Number of NonCompliant users</span></span>|
|<span data-ttu-id="29714-150">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="29714-150">errorUserCount</span></span>|<span data-ttu-id="29714-151">Int32</span><span class="sxs-lookup"><span data-stu-id="29714-151">Int32</span></span>|<span data-ttu-id="29714-152">エラーが発生したユーザーの数</span><span class="sxs-lookup"><span data-stu-id="29714-152">Number of error users</span></span>|
|<span data-ttu-id="29714-153">conflictUserCount</span><span class="sxs-lookup"><span data-stu-id="29714-153">conflictUserCount</span></span>|<span data-ttu-id="29714-154">Int32</span><span class="sxs-lookup"><span data-stu-id="29714-154">Int32</span></span>|<span data-ttu-id="29714-155">競合ユーザーの数</span><span class="sxs-lookup"><span data-stu-id="29714-155">Number of conflict users</span></span>|



## <a name="response"></a><span data-ttu-id="29714-156">応答</span><span class="sxs-lookup"><span data-stu-id="29714-156">Response</span></span>
<span data-ttu-id="29714-157">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="29714-157">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="29714-158">例</span><span class="sxs-lookup"><span data-stu-id="29714-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="29714-159">要求</span><span class="sxs-lookup"><span data-stu-id="29714-159">Request</span></span>
<span data-ttu-id="29714-160">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="29714-160">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="29714-161">応答</span><span class="sxs-lookup"><span data-stu-id="29714-161">Response</span></span>
<span data-ttu-id="29714-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="29714-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




