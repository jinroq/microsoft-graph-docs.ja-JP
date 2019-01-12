---
title: CircularGeofenceManagementCondition を更新します。
description: CircularGeofenceManagementCondition オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 45c6e1d491b652a31ba7e36eac9fb82eef1b235f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27963956"
---
# <a name="update-circulargeofencemanagementcondition"></a><span data-ttu-id="8b1ea-103">CircularGeofenceManagementCondition を更新します。</span><span class="sxs-lookup"><span data-stu-id="8b1ea-103">Update circularGeofenceManagementCondition</span></span>

> <span data-ttu-id="8b1ea-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="8b1ea-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8b1ea-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8b1ea-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8b1ea-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="8b1ea-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8b1ea-107">[CircularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="8b1ea-107">Update the properties of a [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8b1ea-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="8b1ea-108">Prerequisites</span></span>
<span data-ttu-id="8b1ea-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8b1ea-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8b1ea-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8b1ea-111">Permission type</span></span>|<span data-ttu-id="8b1ea-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="8b1ea-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8b1ea-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8b1ea-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8b1ea-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b1ea-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8b1ea-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8b1ea-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8b1ea-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8b1ea-116">Not supported.</span></span>|
|<span data-ttu-id="8b1ea-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8b1ea-117">Application</span></span>|<span data-ttu-id="8b1ea-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8b1ea-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8b1ea-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8b1ea-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managementConditions/{managementConditionId}
PATCH /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions/{managementConditionId}
```

## <a name="request-headers"></a><span data-ttu-id="8b1ea-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8b1ea-120">Request headers</span></span>
|<span data-ttu-id="8b1ea-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8b1ea-121">Header</span></span>|<span data-ttu-id="8b1ea-122">値</span><span class="sxs-lookup"><span data-stu-id="8b1ea-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8b1ea-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8b1ea-123">Authorization</span></span>|<span data-ttu-id="8b1ea-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="8b1ea-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8b1ea-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8b1ea-125">Accept</span></span>|<span data-ttu-id="8b1ea-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8b1ea-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8b1ea-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="8b1ea-127">Request body</span></span>
<span data-ttu-id="8b1ea-128">要求の本文に[circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="8b1ea-128">In the request body, supply a JSON representation for the [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) object.</span></span>

<span data-ttu-id="8b1ea-129">[CircularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="8b1ea-129">The following table shows the properties that are required when you create the [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md).</span></span>

|<span data-ttu-id="8b1ea-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8b1ea-130">Property</span></span>|<span data-ttu-id="8b1ea-131">種類</span><span class="sxs-lookup"><span data-stu-id="8b1ea-131">Type</span></span>|<span data-ttu-id="8b1ea-132">説明</span><span class="sxs-lookup"><span data-stu-id="8b1ea-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8b1ea-133">ID</span><span class="sxs-lookup"><span data-stu-id="8b1ea-133">id</span></span>|<span data-ttu-id="8b1ea-134">String</span><span class="sxs-lookup"><span data-stu-id="8b1ea-134">String</span></span>|<span data-ttu-id="8b1ea-135">管理条件の一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="8b1ea-135">Unique identifier for the management condition.</span></span> <span data-ttu-id="8b1ea-136">システムでは、作成時に割り当てられた値が生成されます。</span><span class="sxs-lookup"><span data-stu-id="8b1ea-136">System generated value assigned when created.</span></span> <span data-ttu-id="8b1ea-137">[ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="8b1ea-137">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="8b1ea-138">一意な名前</span><span class="sxs-lookup"><span data-stu-id="8b1ea-138">uniqueName</span></span>|<span data-ttu-id="8b1ea-139">String</span><span class="sxs-lookup"><span data-stu-id="8b1ea-139">String</span></span>|<span data-ttu-id="8b1ea-140">管理条件の一意の名前です。</span><span class="sxs-lookup"><span data-stu-id="8b1ea-140">Unique name for the management condition.</span></span> <span data-ttu-id="8b1ea-141">管理条件式で使用されます。</span><span class="sxs-lookup"><span data-stu-id="8b1ea-141">Used in management condition expressions.</span></span> <span data-ttu-id="8b1ea-142">[ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="8b1ea-142">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="8b1ea-143">displayName</span><span class="sxs-lookup"><span data-stu-id="8b1ea-143">displayName</span></span>|<span data-ttu-id="8b1ea-144">String</span><span class="sxs-lookup"><span data-stu-id="8b1ea-144">String</span></span>|<span data-ttu-id="8b1ea-145">管理者は、管理の条件の名前を定義します。</span><span class="sxs-lookup"><span data-stu-id="8b1ea-145">The admin defined name of the management condition.</span></span> <span data-ttu-id="8b1ea-146">[ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="8b1ea-146">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="8b1ea-147">説明</span><span class="sxs-lookup"><span data-stu-id="8b1ea-147">description</span></span>|<span data-ttu-id="8b1ea-148">String</span><span class="sxs-lookup"><span data-stu-id="8b1ea-148">String</span></span>|<span data-ttu-id="8b1ea-149">管理者は、管理状態の説明を定義します。</span><span class="sxs-lookup"><span data-stu-id="8b1ea-149">The admin defined description of the management condition.</span></span> <span data-ttu-id="8b1ea-150">[ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="8b1ea-150">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="8b1ea-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8b1ea-151">createdDateTime</span></span>|<span data-ttu-id="8b1ea-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8b1ea-152">DateTimeOffset</span></span>|<span data-ttu-id="8b1ea-153">管理条件が作成された時刻。</span><span class="sxs-lookup"><span data-stu-id="8b1ea-153">The time the management condition was created.</span></span> <span data-ttu-id="8b1ea-154">サービス側が生成されます。</span><span class="sxs-lookup"><span data-stu-id="8b1ea-154">Generated service side.</span></span> <span data-ttu-id="8b1ea-155">[ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="8b1ea-155">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="8b1ea-156">変更された日時</span><span class="sxs-lookup"><span data-stu-id="8b1ea-156">modifiedDateTime</span></span>|<span data-ttu-id="8b1ea-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8b1ea-157">DateTimeOffset</span></span>|<span data-ttu-id="8b1ea-158">管理条件が最後に修正された時間です。</span><span class="sxs-lookup"><span data-stu-id="8b1ea-158">The time the management condition was last modified.</span></span> <span data-ttu-id="8b1ea-159">サービス側を更新します。</span><span class="sxs-lookup"><span data-stu-id="8b1ea-159">Updated service side.</span></span> <span data-ttu-id="8b1ea-160">[ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="8b1ea-160">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="8b1ea-161">eTag</span><span class="sxs-lookup"><span data-stu-id="8b1ea-161">eTag</span></span>|<span data-ttu-id="8b1ea-162">String</span><span class="sxs-lookup"><span data-stu-id="8b1ea-162">String</span></span>|<span data-ttu-id="8b1ea-163">管理条件の ETag。</span><span class="sxs-lookup"><span data-stu-id="8b1ea-163">ETag of the management condition.</span></span> <span data-ttu-id="8b1ea-164">サービス側を更新します。</span><span class="sxs-lookup"><span data-stu-id="8b1ea-164">Updated service side.</span></span> <span data-ttu-id="8b1ea-165">[ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="8b1ea-165">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="8b1ea-166">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="8b1ea-166">applicablePlatforms</span></span>|<span data-ttu-id="8b1ea-167">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="8b1ea-167">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="8b1ea-168">この管理条件に該当するプラットフォームです。</span><span class="sxs-lookup"><span data-stu-id="8b1ea-168">The applicable platforms for this management condition.</span></span> <span data-ttu-id="8b1ea-169">[ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="8b1ea-169">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md).</span></span> <span data-ttu-id="8b1ea-170">可能な値は、`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile` です。</span><span class="sxs-lookup"><span data-stu-id="8b1ea-170">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.</span></span>|
|<span data-ttu-id="8b1ea-171">latitude</span><span class="sxs-lookup"><span data-stu-id="8b1ea-171">latitude</span></span>|<span data-ttu-id="8b1ea-172">倍精度浮動小数点数</span><span class="sxs-lookup"><span data-stu-id="8b1ea-172">Double</span></span>|<span data-ttu-id="8b1ea-173">度、-90 °、および包括的 +90 の間の緯度です。</span><span class="sxs-lookup"><span data-stu-id="8b1ea-173">Latitude in degrees, between -90 and +90 inclusive.</span></span>|
|<span data-ttu-id="8b1ea-174">longitude</span><span class="sxs-lookup"><span data-stu-id="8b1ea-174">longitude</span></span>|<span data-ttu-id="8b1ea-175">倍精度浮動小数点数</span><span class="sxs-lookup"><span data-stu-id="8b1ea-175">Double</span></span>|<span data-ttu-id="8b1ea-176">-180 と包括的な +180 度の経度です。</span><span class="sxs-lookup"><span data-stu-id="8b1ea-176">Longitude in degrees, between -180 and +180 inclusive.</span></span>|
|<span data-ttu-id="8b1ea-177">radiusInMeters</span><span class="sxs-lookup"><span data-stu-id="8b1ea-177">radiusInMeters</span></span>|<span data-ttu-id="8b1ea-178">単精度浮動小数点型 (Single)</span><span class="sxs-lookup"><span data-stu-id="8b1ea-178">Single</span></span>|<span data-ttu-id="8b1ea-179">メートル単位の半径です。</span><span class="sxs-lookup"><span data-stu-id="8b1ea-179">Radius in meters.</span></span>|



## <a name="response"></a><span data-ttu-id="8b1ea-180">応答</span><span class="sxs-lookup"><span data-stu-id="8b1ea-180">Response</span></span>
<span data-ttu-id="8b1ea-181">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="8b1ea-181">If successful, this method returns a `200 OK` response code and an updated [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8b1ea-182">例</span><span class="sxs-lookup"><span data-stu-id="8b1ea-182">Example</span></span>
### <a name="request"></a><span data-ttu-id="8b1ea-183">要求</span><span class="sxs-lookup"><span data-stu-id="8b1ea-183">Request</span></span>
<span data-ttu-id="8b1ea-184">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8b1ea-184">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/managementConditions/{managementConditionId}
Content-type: application/json
Content-length: 370

{
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

### <a name="response"></a><span data-ttu-id="8b1ea-185">応答</span><span class="sxs-lookup"><span data-stu-id="8b1ea-185">Response</span></span>
<span data-ttu-id="8b1ea-p111">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8b1ea-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





