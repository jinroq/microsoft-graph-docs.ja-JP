---
title: CircularGeofenceManagementCondition の更新
description: CircularGeofenceManagementCondition オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6f32e1416bf956b34dd5ca0b7c31d31ed552b933
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35990408"
---
# <a name="update-circulargeofencemanagementcondition"></a><span data-ttu-id="b992f-103">CircularGeofenceManagementCondition の更新</span><span class="sxs-lookup"><span data-stu-id="b992f-103">Update circularGeofenceManagementCondition</span></span>

> <span data-ttu-id="b992f-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b992f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b992f-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b992f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b992f-106">[CircularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="b992f-106">Update the properties of a [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b992f-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="b992f-107">Prerequisites</span></span>
<span data-ttu-id="b992f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b992f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b992f-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b992f-110">Permission type</span></span>|<span data-ttu-id="b992f-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="b992f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b992f-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b992f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b992f-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b992f-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b992f-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b992f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b992f-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b992f-115">Not supported.</span></span>|
|<span data-ttu-id="b992f-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b992f-116">Application</span></span>|<span data-ttu-id="b992f-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b992f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b992f-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b992f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managementConditions/{managementConditionId}
PATCH /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions/{managementConditionId}
```

## <a name="request-headers"></a><span data-ttu-id="b992f-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b992f-119">Request headers</span></span>
|<span data-ttu-id="b992f-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b992f-120">Header</span></span>|<span data-ttu-id="b992f-121">値</span><span class="sxs-lookup"><span data-stu-id="b992f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b992f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b992f-122">Authorization</span></span>|<span data-ttu-id="b992f-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="b992f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b992f-124">承諾</span><span class="sxs-lookup"><span data-stu-id="b992f-124">Accept</span></span>|<span data-ttu-id="b992f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b992f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b992f-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="b992f-126">Request body</span></span>
<span data-ttu-id="b992f-127">要求本文で、 [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="b992f-127">In the request body, supply a JSON representation for the [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) object.</span></span>

<span data-ttu-id="b992f-128">次の表に、 [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="b992f-128">The following table shows the properties that are required when you create the [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md).</span></span>

|<span data-ttu-id="b992f-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b992f-129">Property</span></span>|<span data-ttu-id="b992f-130">型</span><span class="sxs-lookup"><span data-stu-id="b992f-130">Type</span></span>|<span data-ttu-id="b992f-131">説明</span><span class="sxs-lookup"><span data-stu-id="b992f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b992f-132">id</span><span class="sxs-lookup"><span data-stu-id="b992f-132">id</span></span>|<span data-ttu-id="b992f-133">文字列</span><span class="sxs-lookup"><span data-stu-id="b992f-133">String</span></span>|<span data-ttu-id="b992f-134">管理条件の一意識別子。</span><span class="sxs-lookup"><span data-stu-id="b992f-134">Unique identifier for the management condition.</span></span> <span data-ttu-id="b992f-135">作成時に割り当てられたシステム生成値。</span><span class="sxs-lookup"><span data-stu-id="b992f-135">System generated value assigned when created.</span></span> <span data-ttu-id="b992f-136">[Managementcondition](../resources/intune-fencing-managementcondition.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="b992f-136">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="b992f-137">uniqueName</span><span class="sxs-lookup"><span data-stu-id="b992f-137">uniqueName</span></span>|<span data-ttu-id="b992f-138">String</span><span class="sxs-lookup"><span data-stu-id="b992f-138">String</span></span>|<span data-ttu-id="b992f-139">管理条件の一意の名前。</span><span class="sxs-lookup"><span data-stu-id="b992f-139">Unique name for the management condition.</span></span> <span data-ttu-id="b992f-140">管理条件式で使用されます。</span><span class="sxs-lookup"><span data-stu-id="b992f-140">Used in management condition expressions.</span></span> <span data-ttu-id="b992f-141">[Managementcondition](../resources/intune-fencing-managementcondition.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="b992f-141">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="b992f-142">displayName</span><span class="sxs-lookup"><span data-stu-id="b992f-142">displayName</span></span>|<span data-ttu-id="b992f-143">String</span><span class="sxs-lookup"><span data-stu-id="b992f-143">String</span></span>|<span data-ttu-id="b992f-144">管理条件の管理者定義の名前。</span><span class="sxs-lookup"><span data-stu-id="b992f-144">The admin defined name of the management condition.</span></span> <span data-ttu-id="b992f-145">[Managementcondition](../resources/intune-fencing-managementcondition.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="b992f-145">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="b992f-146">description</span><span class="sxs-lookup"><span data-stu-id="b992f-146">description</span></span>|<span data-ttu-id="b992f-147">String</span><span class="sxs-lookup"><span data-stu-id="b992f-147">String</span></span>|<span data-ttu-id="b992f-148">管理条件の管理者定義の説明。</span><span class="sxs-lookup"><span data-stu-id="b992f-148">The admin defined description of the management condition.</span></span> <span data-ttu-id="b992f-149">[Managementcondition](../resources/intune-fencing-managementcondition.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="b992f-149">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="b992f-150">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b992f-150">createdDateTime</span></span>|<span data-ttu-id="b992f-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b992f-151">DateTimeOffset</span></span>|<span data-ttu-id="b992f-152">管理条件が作成された時刻。</span><span class="sxs-lookup"><span data-stu-id="b992f-152">The time the management condition was created.</span></span> <span data-ttu-id="b992f-153">サービス側を生成しました。</span><span class="sxs-lookup"><span data-stu-id="b992f-153">Generated service side.</span></span> <span data-ttu-id="b992f-154">[Managementcondition](../resources/intune-fencing-managementcondition.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="b992f-154">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="b992f-155">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b992f-155">modifiedDateTime</span></span>|<span data-ttu-id="b992f-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b992f-156">DateTimeOffset</span></span>|<span data-ttu-id="b992f-157">管理条件が最後に変更された時刻。</span><span class="sxs-lookup"><span data-stu-id="b992f-157">The time the management condition was last modified.</span></span> <span data-ttu-id="b992f-158">サービス側を更新しました。</span><span class="sxs-lookup"><span data-stu-id="b992f-158">Updated service side.</span></span> <span data-ttu-id="b992f-159">[Managementcondition](../resources/intune-fencing-managementcondition.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="b992f-159">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="b992f-160">eTag</span><span class="sxs-lookup"><span data-stu-id="b992f-160">eTag</span></span>|<span data-ttu-id="b992f-161">String</span><span class="sxs-lookup"><span data-stu-id="b992f-161">String</span></span>|<span data-ttu-id="b992f-162">管理条件の ETag。</span><span class="sxs-lookup"><span data-stu-id="b992f-162">ETag of the management condition.</span></span> <span data-ttu-id="b992f-163">サービス側を更新しました。</span><span class="sxs-lookup"><span data-stu-id="b992f-163">Updated service side.</span></span> <span data-ttu-id="b992f-164">[Managementcondition](../resources/intune-fencing-managementcondition.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="b992f-164">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="b992f-165">アプリケーションのプラットフォーム</span><span class="sxs-lookup"><span data-stu-id="b992f-165">applicablePlatforms</span></span>|<span data-ttu-id="b992f-166">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="b992f-166">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="b992f-167">この管理条件の適用可能なプラットフォーム。</span><span class="sxs-lookup"><span data-stu-id="b992f-167">The applicable platforms for this management condition.</span></span> <span data-ttu-id="b992f-168">[Managementcondition](../resources/intune-fencing-managementcondition.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="b992f-168">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md).</span></span> <span data-ttu-id="b992f-169">可能な値は、`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`unknown` です。</span><span class="sxs-lookup"><span data-stu-id="b992f-169">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span></span>|
|<span data-ttu-id="b992f-170">latitude</span><span class="sxs-lookup"><span data-stu-id="b992f-170">latitude</span></span>|<span data-ttu-id="b992f-171">2 行分</span><span class="sxs-lookup"><span data-stu-id="b992f-171">Double</span></span>|<span data-ttu-id="b992f-172">緯度 (度は-90 と + 90 を含む)。</span><span class="sxs-lookup"><span data-stu-id="b992f-172">Latitude in degrees, between -90 and +90 inclusive.</span></span>|
|<span data-ttu-id="b992f-173">longitude</span><span class="sxs-lookup"><span data-stu-id="b992f-173">longitude</span></span>|<span data-ttu-id="b992f-174">Double</span><span class="sxs-lookup"><span data-stu-id="b992f-174">Double</span></span>|<span data-ttu-id="b992f-175">角度 (単位は-180 と + 180 を含む)。</span><span class="sxs-lookup"><span data-stu-id="b992f-175">Longitude in degrees, between -180 and +180 inclusive.</span></span>|
|<span data-ttu-id="b992f-176">radiusInMeters</span><span class="sxs-lookup"><span data-stu-id="b992f-176">radiusInMeters</span></span>|<span data-ttu-id="b992f-177">1 行</span><span class="sxs-lookup"><span data-stu-id="b992f-177">Single</span></span>|<span data-ttu-id="b992f-178">半径 (メートル単位)。</span><span class="sxs-lookup"><span data-stu-id="b992f-178">Radius in meters.</span></span>|



## <a name="response"></a><span data-ttu-id="b992f-179">応答</span><span class="sxs-lookup"><span data-stu-id="b992f-179">Response</span></span>
<span data-ttu-id="b992f-180">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="b992f-180">If successful, this method returns a `200 OK` response code and an updated [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b992f-181">例</span><span class="sxs-lookup"><span data-stu-id="b992f-181">Example</span></span>

### <a name="request"></a><span data-ttu-id="b992f-182">要求</span><span class="sxs-lookup"><span data-stu-id="b992f-182">Request</span></span>
<span data-ttu-id="b992f-183">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b992f-183">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/managementConditions/{managementConditionId}
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

### <a name="response"></a><span data-ttu-id="b992f-184">応答</span><span class="sxs-lookup"><span data-stu-id="b992f-184">Response</span></span>
<span data-ttu-id="b992f-p110">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b992f-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





