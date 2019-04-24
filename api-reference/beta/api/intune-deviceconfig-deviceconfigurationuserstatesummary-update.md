---
title: deviceConfigurationUserStateSummary の更新
description: deviceConfigurationUserStateSummary オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b03f366ba494e351e5dab898ec10e259db250521
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32467907"
---
# <a name="update-deviceconfigurationuserstatesummary"></a><span data-ttu-id="76de1-103">deviceConfigurationUserStateSummary の更新</span><span class="sxs-lookup"><span data-stu-id="76de1-103">Update deviceConfigurationUserStateSummary</span></span>

> <span data-ttu-id="76de1-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="76de1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="76de1-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="76de1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="76de1-106">[deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="76de1-106">Update the properties of a [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="76de1-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="76de1-107">Prerequisites</span></span>
<span data-ttu-id="76de1-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="76de1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="76de1-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="76de1-110">Permission type</span></span>|<span data-ttu-id="76de1-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="76de1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="76de1-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="76de1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="76de1-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="76de1-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="76de1-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="76de1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="76de1-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="76de1-115">Not supported.</span></span>|
|<span data-ttu-id="76de1-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="76de1-116">Application</span></span>|<span data-ttu-id="76de1-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="76de1-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="76de1-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="76de1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationUserStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="76de1-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="76de1-119">Request headers</span></span>
|<span data-ttu-id="76de1-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="76de1-120">Header</span></span>|<span data-ttu-id="76de1-121">値</span><span class="sxs-lookup"><span data-stu-id="76de1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="76de1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="76de1-122">Authorization</span></span>|<span data-ttu-id="76de1-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="76de1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="76de1-124">承諾</span><span class="sxs-lookup"><span data-stu-id="76de1-124">Accept</span></span>|<span data-ttu-id="76de1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="76de1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="76de1-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="76de1-126">Request body</span></span>
<span data-ttu-id="76de1-127">要求本文で、 [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="76de1-127">In the request body, supply a JSON representation for the [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) object.</span></span>

<span data-ttu-id="76de1-128">次の表に、 [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="76de1-128">The following table shows the properties that are required when you create the [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md).</span></span>

|<span data-ttu-id="76de1-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="76de1-129">Property</span></span>|<span data-ttu-id="76de1-130">型</span><span class="sxs-lookup"><span data-stu-id="76de1-130">Type</span></span>|<span data-ttu-id="76de1-131">説明</span><span class="sxs-lookup"><span data-stu-id="76de1-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="76de1-132">id</span><span class="sxs-lookup"><span data-stu-id="76de1-132">id</span></span>|<span data-ttu-id="76de1-133">String</span><span class="sxs-lookup"><span data-stu-id="76de1-133">String</span></span>|<span data-ttu-id="76de1-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="76de1-134">Key of the entity.</span></span>|
|<span data-ttu-id="76de1-135">unknownUserCount</span><span class="sxs-lookup"><span data-stu-id="76de1-135">unknownUserCount</span></span>|<span data-ttu-id="76de1-136">Int32</span><span class="sxs-lookup"><span data-stu-id="76de1-136">Int32</span></span>|<span data-ttu-id="76de1-137">不明なユーザーの数</span><span class="sxs-lookup"><span data-stu-id="76de1-137">Number of unknown users</span></span>|
|<span data-ttu-id="76de1-138">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="76de1-138">notApplicableUserCount</span></span>|<span data-ttu-id="76de1-139">Int32</span><span class="sxs-lookup"><span data-stu-id="76de1-139">Int32</span></span>|<span data-ttu-id="76de1-140">該当しないユーザーの数</span><span class="sxs-lookup"><span data-stu-id="76de1-140">Number of not applicable users</span></span>|
|<span data-ttu-id="76de1-141">compliantUserCount</span><span class="sxs-lookup"><span data-stu-id="76de1-141">compliantUserCount</span></span>|<span data-ttu-id="76de1-142">Int32</span><span class="sxs-lookup"><span data-stu-id="76de1-142">Int32</span></span>|<span data-ttu-id="76de1-143">準拠しているユーザーの数</span><span class="sxs-lookup"><span data-stu-id="76de1-143">Number of compliant users</span></span>|
|<span data-ttu-id="76de1-144">remediatedUserCount</span><span class="sxs-lookup"><span data-stu-id="76de1-144">remediatedUserCount</span></span>|<span data-ttu-id="76de1-145">Int32</span><span class="sxs-lookup"><span data-stu-id="76de1-145">Int32</span></span>|<span data-ttu-id="76de1-146">修復したユーザーの数</span><span class="sxs-lookup"><span data-stu-id="76de1-146">Number of remediated users</span></span>|
|<span data-ttu-id="76de1-147">nonCompliantUserCount</span><span class="sxs-lookup"><span data-stu-id="76de1-147">nonCompliantUserCount</span></span>|<span data-ttu-id="76de1-148">Int32</span><span class="sxs-lookup"><span data-stu-id="76de1-148">Int32</span></span>|<span data-ttu-id="76de1-149">準拠していないユーザーの数</span><span class="sxs-lookup"><span data-stu-id="76de1-149">Number of NonCompliant users</span></span>|
|<span data-ttu-id="76de1-150">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="76de1-150">errorUserCount</span></span>|<span data-ttu-id="76de1-151">Int32</span><span class="sxs-lookup"><span data-stu-id="76de1-151">Int32</span></span>|<span data-ttu-id="76de1-152">エラーが発生したユーザーの数</span><span class="sxs-lookup"><span data-stu-id="76de1-152">Number of error users</span></span>|
|<span data-ttu-id="76de1-153">conflictUserCount</span><span class="sxs-lookup"><span data-stu-id="76de1-153">conflictUserCount</span></span>|<span data-ttu-id="76de1-154">Int32</span><span class="sxs-lookup"><span data-stu-id="76de1-154">Int32</span></span>|<span data-ttu-id="76de1-155">競合ユーザーの数</span><span class="sxs-lookup"><span data-stu-id="76de1-155">Number of conflict users</span></span>|



## <a name="response"></a><span data-ttu-id="76de1-156">応答</span><span class="sxs-lookup"><span data-stu-id="76de1-156">Response</span></span>
<span data-ttu-id="76de1-157">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="76de1-157">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="76de1-158">例</span><span class="sxs-lookup"><span data-stu-id="76de1-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="76de1-159">要求</span><span class="sxs-lookup"><span data-stu-id="76de1-159">Request</span></span>
<span data-ttu-id="76de1-160">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="76de1-160">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="76de1-161">応答</span><span class="sxs-lookup"><span data-stu-id="76de1-161">Response</span></span>
<span data-ttu-id="76de1-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="76de1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





