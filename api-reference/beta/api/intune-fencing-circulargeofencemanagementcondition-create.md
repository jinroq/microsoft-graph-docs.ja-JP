---
title: CircularGeofenceManagementCondition を作成する
description: 新しい circularGeofenceManagementCondition オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 05c9d99d0b9b27e462a1b0e9a0579b40ccb2aab4
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36355690"
---
# <a name="create-circulargeofencemanagementcondition"></a><span data-ttu-id="43ead-103">CircularGeofenceManagementCondition を作成する</span><span class="sxs-lookup"><span data-stu-id="43ead-103">Create circularGeofenceManagementCondition</span></span>

> <span data-ttu-id="43ead-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="43ead-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="43ead-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="43ead-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="43ead-106">新しい[circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="43ead-106">Create a new [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="43ead-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="43ead-107">Prerequisites</span></span>
<span data-ttu-id="43ead-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="43ead-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="43ead-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="43ead-110">Permission type</span></span>|<span data-ttu-id="43ead-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="43ead-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="43ead-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="43ead-112">Delegated (work or school account)</span></span>|<span data-ttu-id="43ead-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43ead-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="43ead-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="43ead-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="43ead-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="43ead-115">Not supported.</span></span>|
|<span data-ttu-id="43ead-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="43ead-116">Application</span></span>|<span data-ttu-id="43ead-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43ead-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="43ead-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="43ead-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managementConditions
POST /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions
```

## <a name="request-headers"></a><span data-ttu-id="43ead-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="43ead-119">Request headers</span></span>
|<span data-ttu-id="43ead-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="43ead-120">Header</span></span>|<span data-ttu-id="43ead-121">値</span><span class="sxs-lookup"><span data-stu-id="43ead-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="43ead-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="43ead-122">Authorization</span></span>|<span data-ttu-id="43ead-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="43ead-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="43ead-124">承諾</span><span class="sxs-lookup"><span data-stu-id="43ead-124">Accept</span></span>|<span data-ttu-id="43ead-125">application/json</span><span class="sxs-lookup"><span data-stu-id="43ead-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="43ead-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="43ead-126">Request body</span></span>
<span data-ttu-id="43ead-127">要求本文で、circularGeofenceManagementCondition オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="43ead-127">In the request body, supply a JSON representation for the circularGeofenceManagementCondition object.</span></span>

<span data-ttu-id="43ead-128">次の表に、circularGeofenceManagementCondition の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="43ead-128">The following table shows the properties that are required when you create the circularGeofenceManagementCondition.</span></span>

|<span data-ttu-id="43ead-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="43ead-129">Property</span></span>|<span data-ttu-id="43ead-130">型</span><span class="sxs-lookup"><span data-stu-id="43ead-130">Type</span></span>|<span data-ttu-id="43ead-131">説明</span><span class="sxs-lookup"><span data-stu-id="43ead-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="43ead-132">id</span><span class="sxs-lookup"><span data-stu-id="43ead-132">id</span></span>|<span data-ttu-id="43ead-133">文字列</span><span class="sxs-lookup"><span data-stu-id="43ead-133">String</span></span>|<span data-ttu-id="43ead-134">管理条件の一意識別子。</span><span class="sxs-lookup"><span data-stu-id="43ead-134">Unique identifier for the management condition.</span></span> <span data-ttu-id="43ead-135">作成時に割り当てられたシステム生成値。</span><span class="sxs-lookup"><span data-stu-id="43ead-135">System generated value assigned when created.</span></span> <span data-ttu-id="43ead-136">[Managementcondition](../resources/intune-fencing-managementcondition.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="43ead-136">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="43ead-137">uniqueName</span><span class="sxs-lookup"><span data-stu-id="43ead-137">uniqueName</span></span>|<span data-ttu-id="43ead-138">String</span><span class="sxs-lookup"><span data-stu-id="43ead-138">String</span></span>|<span data-ttu-id="43ead-139">管理条件の一意の名前。</span><span class="sxs-lookup"><span data-stu-id="43ead-139">Unique name for the management condition.</span></span> <span data-ttu-id="43ead-140">管理条件式で使用されます。</span><span class="sxs-lookup"><span data-stu-id="43ead-140">Used in management condition expressions.</span></span> <span data-ttu-id="43ead-141">[Managementcondition](../resources/intune-fencing-managementcondition.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="43ead-141">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="43ead-142">displayName</span><span class="sxs-lookup"><span data-stu-id="43ead-142">displayName</span></span>|<span data-ttu-id="43ead-143">String</span><span class="sxs-lookup"><span data-stu-id="43ead-143">String</span></span>|<span data-ttu-id="43ead-144">管理条件の管理者定義の名前。</span><span class="sxs-lookup"><span data-stu-id="43ead-144">The admin defined name of the management condition.</span></span> <span data-ttu-id="43ead-145">[Managementcondition](../resources/intune-fencing-managementcondition.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="43ead-145">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="43ead-146">description</span><span class="sxs-lookup"><span data-stu-id="43ead-146">description</span></span>|<span data-ttu-id="43ead-147">String</span><span class="sxs-lookup"><span data-stu-id="43ead-147">String</span></span>|<span data-ttu-id="43ead-148">管理条件の管理者定義の説明。</span><span class="sxs-lookup"><span data-stu-id="43ead-148">The admin defined description of the management condition.</span></span> <span data-ttu-id="43ead-149">[Managementcondition](../resources/intune-fencing-managementcondition.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="43ead-149">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="43ead-150">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="43ead-150">createdDateTime</span></span>|<span data-ttu-id="43ead-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="43ead-151">DateTimeOffset</span></span>|<span data-ttu-id="43ead-152">管理条件が作成された時刻。</span><span class="sxs-lookup"><span data-stu-id="43ead-152">The time the management condition was created.</span></span> <span data-ttu-id="43ead-153">サービス側を生成しました。</span><span class="sxs-lookup"><span data-stu-id="43ead-153">Generated service side.</span></span> <span data-ttu-id="43ead-154">[Managementcondition](../resources/intune-fencing-managementcondition.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="43ead-154">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="43ead-155">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="43ead-155">modifiedDateTime</span></span>|<span data-ttu-id="43ead-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="43ead-156">DateTimeOffset</span></span>|<span data-ttu-id="43ead-157">管理条件が最後に変更された時刻。</span><span class="sxs-lookup"><span data-stu-id="43ead-157">The time the management condition was last modified.</span></span> <span data-ttu-id="43ead-158">サービス側を更新しました。</span><span class="sxs-lookup"><span data-stu-id="43ead-158">Updated service side.</span></span> <span data-ttu-id="43ead-159">[Managementcondition](../resources/intune-fencing-managementcondition.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="43ead-159">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="43ead-160">eTag</span><span class="sxs-lookup"><span data-stu-id="43ead-160">eTag</span></span>|<span data-ttu-id="43ead-161">String</span><span class="sxs-lookup"><span data-stu-id="43ead-161">String</span></span>|<span data-ttu-id="43ead-162">管理条件の ETag。</span><span class="sxs-lookup"><span data-stu-id="43ead-162">ETag of the management condition.</span></span> <span data-ttu-id="43ead-163">サービス側を更新しました。</span><span class="sxs-lookup"><span data-stu-id="43ead-163">Updated service side.</span></span> <span data-ttu-id="43ead-164">[Managementcondition](../resources/intune-fencing-managementcondition.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="43ead-164">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="43ead-165">アプリケーションのプラットフォーム</span><span class="sxs-lookup"><span data-stu-id="43ead-165">applicablePlatforms</span></span>|<span data-ttu-id="43ead-166">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="43ead-166">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="43ead-167">この管理条件の適用可能なプラットフォーム。</span><span class="sxs-lookup"><span data-stu-id="43ead-167">The applicable platforms for this management condition.</span></span> <span data-ttu-id="43ead-168">[Managementcondition](../resources/intune-fencing-managementcondition.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="43ead-168">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md).</span></span> <span data-ttu-id="43ead-169">可能な値は、`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`unknown` です。</span><span class="sxs-lookup"><span data-stu-id="43ead-169">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span></span>|
|<span data-ttu-id="43ead-170">latitude</span><span class="sxs-lookup"><span data-stu-id="43ead-170">latitude</span></span>|<span data-ttu-id="43ead-171">2 行分</span><span class="sxs-lookup"><span data-stu-id="43ead-171">Double</span></span>|<span data-ttu-id="43ead-172">緯度 (度は-90 と + 90 を含む)。</span><span class="sxs-lookup"><span data-stu-id="43ead-172">Latitude in degrees, between -90 and +90 inclusive.</span></span>|
|<span data-ttu-id="43ead-173">longitude</span><span class="sxs-lookup"><span data-stu-id="43ead-173">longitude</span></span>|<span data-ttu-id="43ead-174">Double</span><span class="sxs-lookup"><span data-stu-id="43ead-174">Double</span></span>|<span data-ttu-id="43ead-175">角度 (単位は-180 と + 180 を含む)。</span><span class="sxs-lookup"><span data-stu-id="43ead-175">Longitude in degrees, between -180 and +180 inclusive.</span></span>|
|<span data-ttu-id="43ead-176">radiusInMeters</span><span class="sxs-lookup"><span data-stu-id="43ead-176">radiusInMeters</span></span>|<span data-ttu-id="43ead-177">1 行</span><span class="sxs-lookup"><span data-stu-id="43ead-177">Single</span></span>|<span data-ttu-id="43ead-178">半径 (メートル単位)。</span><span class="sxs-lookup"><span data-stu-id="43ead-178">Radius in meters.</span></span>|



## <a name="response"></a><span data-ttu-id="43ead-179">応答</span><span class="sxs-lookup"><span data-stu-id="43ead-179">Response</span></span>
<span data-ttu-id="43ead-180">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="43ead-180">If successful, this method returns a `201 Created` response code and a [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="43ead-181">例</span><span class="sxs-lookup"><span data-stu-id="43ead-181">Example</span></span>

### <a name="request"></a><span data-ttu-id="43ead-182">要求</span><span class="sxs-lookup"><span data-stu-id="43ead-182">Request</span></span>
<span data-ttu-id="43ead-183">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="43ead-183">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managementConditions
Content-type: application/json
Content-length: 444

{
  "@odata.type": "#microsoft.graph.circularGeofenceManagementCondition",
  "uniqueName": "Unique Name value",
  "displayName": "Display Name value",
  "description": "Description value",
  "eTag": "ETag value",
  "applicablePlatforms": [
    "androidForWork"
  ],
  "latitude": "<Unknown Primitive Type Edm.Double>",
  "longitude": "<Unknown Primitive Type Edm.Double>",
  "radiusInMeters": "<Unknown Primitive Type Edm.Single>"
}
```

### <a name="response"></a><span data-ttu-id="43ead-184">応答</span><span class="sxs-lookup"><span data-stu-id="43ead-184">Response</span></span>
<span data-ttu-id="43ead-p110">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="43ead-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 612

{
  "@odata.type": "#microsoft.graph.circularGeofenceManagementCondition",
  "id": "30ee27b6-27b6-30ee-b627-ee30b627ee30",
  "uniqueName": "Unique Name value",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
  "eTag": "ETag value",
  "applicablePlatforms": [
    "androidForWork"
  ],
  "latitude": "<Unknown Primitive Type Edm.Double>",
  "longitude": "<Unknown Primitive Type Edm.Double>",
  "radiusInMeters": "<Unknown Primitive Type Edm.Single>"
}
```






