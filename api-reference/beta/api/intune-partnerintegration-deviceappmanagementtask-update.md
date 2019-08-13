---
title: DeviceAppManagementTask の更新
description: DeviceAppManagementTask オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5e8315527c5f3737b7c57c57d242436daca42c27
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36351680"
---
# <a name="update-deviceappmanagementtask"></a><span data-ttu-id="2305b-103">DeviceAppManagementTask の更新</span><span class="sxs-lookup"><span data-stu-id="2305b-103">Update deviceAppManagementTask</span></span>

> <span data-ttu-id="2305b-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2305b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2305b-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="2305b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2305b-106">[Deviceappmanagementtask](../resources/intune-partnerintegration-deviceappmanagementtask.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="2305b-106">Update the properties of a [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2305b-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="2305b-107">Prerequisites</span></span>
<span data-ttu-id="2305b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2305b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2305b-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2305b-110">Permission type</span></span>|<span data-ttu-id="2305b-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="2305b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2305b-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2305b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2305b-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2305b-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2305b-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2305b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2305b-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2305b-115">Not supported.</span></span>|
|<span data-ttu-id="2305b-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2305b-116">Application</span></span>|<span data-ttu-id="2305b-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2305b-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2305b-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2305b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/deviceAppManagementTasks/{deviceAppManagementTaskId}
```

## <a name="request-headers"></a><span data-ttu-id="2305b-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2305b-119">Request headers</span></span>
|<span data-ttu-id="2305b-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2305b-120">Header</span></span>|<span data-ttu-id="2305b-121">値</span><span class="sxs-lookup"><span data-stu-id="2305b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2305b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2305b-122">Authorization</span></span>|<span data-ttu-id="2305b-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="2305b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2305b-124">承諾</span><span class="sxs-lookup"><span data-stu-id="2305b-124">Accept</span></span>|<span data-ttu-id="2305b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2305b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2305b-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="2305b-126">Request body</span></span>
<span data-ttu-id="2305b-127">要求本文で、 [Deviceappmanagementtask](../resources/intune-partnerintegration-deviceappmanagementtask.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="2305b-127">In the request body, supply a JSON representation for the [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md) object.</span></span>

<span data-ttu-id="2305b-128">次の表に、 [Deviceappmanagementtask](../resources/intune-partnerintegration-deviceappmanagementtask.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="2305b-128">The following table shows the properties that are required when you create the [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md).</span></span>

|<span data-ttu-id="2305b-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2305b-129">Property</span></span>|<span data-ttu-id="2305b-130">型</span><span class="sxs-lookup"><span data-stu-id="2305b-130">Type</span></span>|<span data-ttu-id="2305b-131">説明</span><span class="sxs-lookup"><span data-stu-id="2305b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2305b-132">id</span><span class="sxs-lookup"><span data-stu-id="2305b-132">id</span></span>|<span data-ttu-id="2305b-133">文字列</span><span class="sxs-lookup"><span data-stu-id="2305b-133">String</span></span>|<span data-ttu-id="2305b-134">エンティティキー。</span><span class="sxs-lookup"><span data-stu-id="2305b-134">The entity key.</span></span>|
|<span data-ttu-id="2305b-135">displayName</span><span class="sxs-lookup"><span data-stu-id="2305b-135">displayName</span></span>|<span data-ttu-id="2305b-136">文字列</span><span class="sxs-lookup"><span data-stu-id="2305b-136">String</span></span>|<span data-ttu-id="2305b-137">名前を指定します。</span><span class="sxs-lookup"><span data-stu-id="2305b-137">The name.</span></span>|
|<span data-ttu-id="2305b-138">description</span><span class="sxs-lookup"><span data-stu-id="2305b-138">description</span></span>|<span data-ttu-id="2305b-139">String</span><span class="sxs-lookup"><span data-stu-id="2305b-139">String</span></span>|<span data-ttu-id="2305b-140">説明。</span><span class="sxs-lookup"><span data-stu-id="2305b-140">The description.</span></span>|
|<span data-ttu-id="2305b-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2305b-141">createdDateTime</span></span>|<span data-ttu-id="2305b-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2305b-142">DateTimeOffset</span></span>|<span data-ttu-id="2305b-143">作成日を指定します。</span><span class="sxs-lookup"><span data-stu-id="2305b-143">The created date.</span></span>|
|<span data-ttu-id="2305b-144">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="2305b-144">dueDateTime</span></span>|<span data-ttu-id="2305b-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2305b-145">DateTimeOffset</span></span>|<span data-ttu-id="2305b-146">期限を指定します。</span><span class="sxs-lookup"><span data-stu-id="2305b-146">The due date.</span></span>|
|<span data-ttu-id="2305b-147">category</span><span class="sxs-lookup"><span data-stu-id="2305b-147">category</span></span>|[<span data-ttu-id="2305b-148">deviceAppManagementTaskCategory</span><span class="sxs-lookup"><span data-stu-id="2305b-148">deviceAppManagementTaskCategory</span></span>](../resources/intune-partnerintegration-deviceappmanagementtaskcategory.md)|<span data-ttu-id="2305b-149">カテゴリ。</span><span class="sxs-lookup"><span data-stu-id="2305b-149">The category.</span></span> <span data-ttu-id="2305b-150">可能な値は、`unknown`、`advancedThreatProtection` です。</span><span class="sxs-lookup"><span data-stu-id="2305b-150">Possible values are: `unknown`, `advancedThreatProtection`.</span></span>|
|<span data-ttu-id="2305b-151">priority</span><span class="sxs-lookup"><span data-stu-id="2305b-151">priority</span></span>|[<span data-ttu-id="2305b-152">deviceAppManagementTaskPriority</span><span class="sxs-lookup"><span data-stu-id="2305b-152">deviceAppManagementTaskPriority</span></span>](../resources/intune-partnerintegration-deviceappmanagementtaskpriority.md)|<span data-ttu-id="2305b-153">優先度。</span><span class="sxs-lookup"><span data-stu-id="2305b-153">The priority.</span></span> <span data-ttu-id="2305b-154">可能な値は、`none`、`high`、`low` です。</span><span class="sxs-lookup"><span data-stu-id="2305b-154">Possible values are: `none`, `high`, `low`.</span></span>|
|<span data-ttu-id="2305b-155">作成者</span><span class="sxs-lookup"><span data-stu-id="2305b-155">creator</span></span>|<span data-ttu-id="2305b-156">String</span><span class="sxs-lookup"><span data-stu-id="2305b-156">String</span></span>|<span data-ttu-id="2305b-157">作成者の電子メールアドレス。</span><span class="sxs-lookup"><span data-stu-id="2305b-157">The email address of the creator.</span></span>|
|<span data-ttu-id="2305b-158">creatorNotes</span><span class="sxs-lookup"><span data-stu-id="2305b-158">creatorNotes</span></span>|<span data-ttu-id="2305b-159">String</span><span class="sxs-lookup"><span data-stu-id="2305b-159">String</span></span>|<span data-ttu-id="2305b-160">作成者からのメモ。</span><span class="sxs-lookup"><span data-stu-id="2305b-160">Notes from the creator.</span></span>|
|<span data-ttu-id="2305b-161">assignedTo</span><span class="sxs-lookup"><span data-stu-id="2305b-161">assignedTo</span></span>|<span data-ttu-id="2305b-162">String</span><span class="sxs-lookup"><span data-stu-id="2305b-162">String</span></span>|<span data-ttu-id="2305b-163">このタスクが割り当てられている管理者の名前または電子メール。</span><span class="sxs-lookup"><span data-stu-id="2305b-163">The name or email of the admin this task is assigned to.</span></span>|
|<span data-ttu-id="2305b-164">status</span><span class="sxs-lookup"><span data-stu-id="2305b-164">status</span></span>|[<span data-ttu-id="2305b-165">deviceAppManagementTaskStatus</span><span class="sxs-lookup"><span data-stu-id="2305b-165">deviceAppManagementTaskStatus</span></span>](../resources/intune-partnerintegration-deviceappmanagementtaskstatus.md)|<span data-ttu-id="2305b-166">ステータス。</span><span class="sxs-lookup"><span data-stu-id="2305b-166">The status.</span></span> <span data-ttu-id="2305b-167">可能な値は、`unknown`、`pending`、`active`、`completed`、`rejected` です。</span><span class="sxs-lookup"><span data-stu-id="2305b-167">Possible values are: `unknown`, `pending`, `active`, `completed`, `rejected`.</span></span>|



## <a name="response"></a><span data-ttu-id="2305b-168">応答</span><span class="sxs-lookup"><span data-stu-id="2305b-168">Response</span></span>
<span data-ttu-id="2305b-169">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[Deviceappmanagementtask](../resources/intune-partnerintegration-deviceappmanagementtask.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="2305b-169">If successful, this method returns a `200 OK` response code and an updated [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2305b-170">例</span><span class="sxs-lookup"><span data-stu-id="2305b-170">Example</span></span>

### <a name="request"></a><span data-ttu-id="2305b-171">要求</span><span class="sxs-lookup"><span data-stu-id="2305b-171">Request</span></span>
<span data-ttu-id="2305b-172">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2305b-172">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2305b-173">応答</span><span class="sxs-lookup"><span data-stu-id="2305b-173">Response</span></span>
<span data-ttu-id="2305b-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="2305b-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






