---
title: DeviceAppManagementTask の更新
description: DeviceAppManagementTask オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c79868e1c618dfd3aaec3dfd9a47e2e572fca280
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "35002302"
---
# <a name="update-deviceappmanagementtask"></a><span data-ttu-id="13585-103">DeviceAppManagementTask の更新</span><span class="sxs-lookup"><span data-stu-id="13585-103">Update deviceAppManagementTask</span></span>

> <span data-ttu-id="13585-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="13585-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="13585-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="13585-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="13585-106">[Deviceappmanagementtask](../resources/intune-partnerintegration-deviceappmanagementtask.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="13585-106">Update the properties of a [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="13585-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="13585-107">Prerequisites</span></span>
<span data-ttu-id="13585-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="13585-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="13585-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="13585-110">Permission type</span></span>|<span data-ttu-id="13585-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="13585-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="13585-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="13585-112">Delegated (work or school account)</span></span>|<span data-ttu-id="13585-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13585-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="13585-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="13585-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="13585-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="13585-115">Not supported.</span></span>|
|<span data-ttu-id="13585-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="13585-116">Application</span></span>|<span data-ttu-id="13585-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="13585-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="13585-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="13585-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/deviceAppManagementTasks/{deviceAppManagementTaskId}
```

## <a name="request-headers"></a><span data-ttu-id="13585-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="13585-119">Request headers</span></span>
|<span data-ttu-id="13585-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="13585-120">Header</span></span>|<span data-ttu-id="13585-121">値</span><span class="sxs-lookup"><span data-stu-id="13585-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="13585-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="13585-122">Authorization</span></span>|<span data-ttu-id="13585-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="13585-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="13585-124">承諾</span><span class="sxs-lookup"><span data-stu-id="13585-124">Accept</span></span>|<span data-ttu-id="13585-125">application/json</span><span class="sxs-lookup"><span data-stu-id="13585-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="13585-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="13585-126">Request body</span></span>
<span data-ttu-id="13585-127">要求本文で、 [Deviceappmanagementtask](../resources/intune-partnerintegration-deviceappmanagementtask.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="13585-127">In the request body, supply a JSON representation for the [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md) object.</span></span>

<span data-ttu-id="13585-128">次の表に、 [Deviceappmanagementtask](../resources/intune-partnerintegration-deviceappmanagementtask.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="13585-128">The following table shows the properties that are required when you create the [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md).</span></span>

|<span data-ttu-id="13585-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="13585-129">Property</span></span>|<span data-ttu-id="13585-130">型</span><span class="sxs-lookup"><span data-stu-id="13585-130">Type</span></span>|<span data-ttu-id="13585-131">説明</span><span class="sxs-lookup"><span data-stu-id="13585-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="13585-132">id</span><span class="sxs-lookup"><span data-stu-id="13585-132">id</span></span>|<span data-ttu-id="13585-133">文字列</span><span class="sxs-lookup"><span data-stu-id="13585-133">String</span></span>|<span data-ttu-id="13585-134">エンティティキー。</span><span class="sxs-lookup"><span data-stu-id="13585-134">The entity key.</span></span>|
|<span data-ttu-id="13585-135">displayName</span><span class="sxs-lookup"><span data-stu-id="13585-135">displayName</span></span>|<span data-ttu-id="13585-136">文字列</span><span class="sxs-lookup"><span data-stu-id="13585-136">String</span></span>|<span data-ttu-id="13585-137">名前を指定します。</span><span class="sxs-lookup"><span data-stu-id="13585-137">The name.</span></span>|
|<span data-ttu-id="13585-138">description</span><span class="sxs-lookup"><span data-stu-id="13585-138">description</span></span>|<span data-ttu-id="13585-139">String</span><span class="sxs-lookup"><span data-stu-id="13585-139">String</span></span>|<span data-ttu-id="13585-140">説明。</span><span class="sxs-lookup"><span data-stu-id="13585-140">The description.</span></span>|
|<span data-ttu-id="13585-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="13585-141">createdDateTime</span></span>|<span data-ttu-id="13585-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="13585-142">DateTimeOffset</span></span>|<span data-ttu-id="13585-143">作成日を指定します。</span><span class="sxs-lookup"><span data-stu-id="13585-143">The created date.</span></span>|
|<span data-ttu-id="13585-144">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="13585-144">dueDateTime</span></span>|<span data-ttu-id="13585-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="13585-145">DateTimeOffset</span></span>|<span data-ttu-id="13585-146">期限を指定します。</span><span class="sxs-lookup"><span data-stu-id="13585-146">The due date.</span></span>|
|<span data-ttu-id="13585-147">category</span><span class="sxs-lookup"><span data-stu-id="13585-147">category</span></span>|[<span data-ttu-id="13585-148">deviceAppManagementTaskCategory</span><span class="sxs-lookup"><span data-stu-id="13585-148">deviceAppManagementTaskCategory</span></span>](../resources/intune-partnerintegration-deviceappmanagementtaskcategory.md)|<span data-ttu-id="13585-149">カテゴリ。</span><span class="sxs-lookup"><span data-stu-id="13585-149">The category.</span></span> <span data-ttu-id="13585-150">可能な値は、`unknown`、`advancedThreatProtection` です。</span><span class="sxs-lookup"><span data-stu-id="13585-150">Possible values are: `unknown`, `advancedThreatProtection`.</span></span>|
|<span data-ttu-id="13585-151">priority</span><span class="sxs-lookup"><span data-stu-id="13585-151">priority</span></span>|[<span data-ttu-id="13585-152">deviceAppManagementTaskPriority</span><span class="sxs-lookup"><span data-stu-id="13585-152">deviceAppManagementTaskPriority</span></span>](../resources/intune-partnerintegration-deviceappmanagementtaskpriority.md)|<span data-ttu-id="13585-153">優先度。</span><span class="sxs-lookup"><span data-stu-id="13585-153">The priority.</span></span> <span data-ttu-id="13585-154">可能な値は、`none`、`high`、`low` です。</span><span class="sxs-lookup"><span data-stu-id="13585-154">Possible values are: `none`, `high`, `low`.</span></span>|
|<span data-ttu-id="13585-155">作成者</span><span class="sxs-lookup"><span data-stu-id="13585-155">creator</span></span>|<span data-ttu-id="13585-156">String</span><span class="sxs-lookup"><span data-stu-id="13585-156">String</span></span>|<span data-ttu-id="13585-157">作成者の電子メールアドレス。</span><span class="sxs-lookup"><span data-stu-id="13585-157">The email address of the creator.</span></span>|
|<span data-ttu-id="13585-158">creatorNotes</span><span class="sxs-lookup"><span data-stu-id="13585-158">creatorNotes</span></span>|<span data-ttu-id="13585-159">String</span><span class="sxs-lookup"><span data-stu-id="13585-159">String</span></span>|<span data-ttu-id="13585-160">作成者からのメモ。</span><span class="sxs-lookup"><span data-stu-id="13585-160">Notes from the creator.</span></span>|
|<span data-ttu-id="13585-161">assignedTo</span><span class="sxs-lookup"><span data-stu-id="13585-161">assignedTo</span></span>|<span data-ttu-id="13585-162">String</span><span class="sxs-lookup"><span data-stu-id="13585-162">String</span></span>|<span data-ttu-id="13585-163">このタスクが割り当てられている管理者の名前または電子メール。</span><span class="sxs-lookup"><span data-stu-id="13585-163">The name or email of the admin this task is assigned to.</span></span>|
|<span data-ttu-id="13585-164">status</span><span class="sxs-lookup"><span data-stu-id="13585-164">status</span></span>|[<span data-ttu-id="13585-165">deviceAppManagementTaskStatus</span><span class="sxs-lookup"><span data-stu-id="13585-165">deviceAppManagementTaskStatus</span></span>](../resources/intune-partnerintegration-deviceappmanagementtaskstatus.md)|<span data-ttu-id="13585-166">ステータス。</span><span class="sxs-lookup"><span data-stu-id="13585-166">The status.</span></span> <span data-ttu-id="13585-167">可能な値は、`unknown`、`pending`、`active`、`completed`、`rejected` です。</span><span class="sxs-lookup"><span data-stu-id="13585-167">Possible values are: `unknown`, `pending`, `active`, `completed`, `rejected`.</span></span>|



## <a name="response"></a><span data-ttu-id="13585-168">応答</span><span class="sxs-lookup"><span data-stu-id="13585-168">Response</span></span>
<span data-ttu-id="13585-169">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[Deviceappmanagementtask](../resources/intune-partnerintegration-deviceappmanagementtask.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="13585-169">If successful, this method returns a `200 OK` response code and an updated [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="13585-170">例</span><span class="sxs-lookup"><span data-stu-id="13585-170">Example</span></span>

### <a name="request"></a><span data-ttu-id="13585-171">要求</span><span class="sxs-lookup"><span data-stu-id="13585-171">Request</span></span>
<span data-ttu-id="13585-172">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="13585-172">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/deviceAppManagementTasks/{deviceAppManagementTaskId}
Content-type: application/json
Content-length: 400

{
  "@odata.type": "#microsoft.graph.deviceAppManagementTask",
  "displayName": "Display Name value",
  "description": "Description value",
  "dueDateTime": "2017-01-01T00:02:18.1994089-08:00",
  "category": "advancedThreatProtection",
  "priority": "high",
  "creator": "Creator value",
  "creatorNotes": "Creator Notes value",
  "assignedTo": "Assigned To value",
  "status": "pending"
}
```

### <a name="response"></a><span data-ttu-id="13585-173">応答</span><span class="sxs-lookup"><span data-stu-id="13585-173">Response</span></span>
<span data-ttu-id="13585-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="13585-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 508

{
  "@odata.type": "#microsoft.graph.deviceAppManagementTask",
  "id": "814545cc-45cc-8145-cc45-4581cc454581",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "dueDateTime": "2017-01-01T00:02:18.1994089-08:00",
  "category": "advancedThreatProtection",
  "priority": "high",
  "creator": "Creator value",
  "creatorNotes": "Creator Notes value",
  "assignedTo": "Assigned To value",
  "status": "pending"
}
```





