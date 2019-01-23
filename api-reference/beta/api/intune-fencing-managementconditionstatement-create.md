---
title: ManagementConditionStatement を作成します。
description: 新しい managementConditionStatement オブジェクトを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: eba9d3f96d7d3a8b1f855c94b18aab6a6450651f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29417358"
---
# <a name="create-managementconditionstatement"></a><span data-ttu-id="b2399-103">ManagementConditionStatement を作成します。</span><span class="sxs-lookup"><span data-stu-id="b2399-103">Create managementConditionStatement</span></span>

> <span data-ttu-id="b2399-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b2399-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b2399-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b2399-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b2399-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b2399-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b2399-107">新しい[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="b2399-107">Create a new [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b2399-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="b2399-108">Prerequisites</span></span>
<span data-ttu-id="b2399-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b2399-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b2399-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b2399-111">Permission type</span></span>|<span data-ttu-id="b2399-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="b2399-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b2399-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b2399-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b2399-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2399-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b2399-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b2399-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b2399-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b2399-116">Not supported.</span></span>|
|<span data-ttu-id="b2399-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b2399-117">Application</span></span>|<span data-ttu-id="b2399-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b2399-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b2399-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b2399-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managementConditionStatements
POST /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements
```

## <a name="request-headers"></a><span data-ttu-id="b2399-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b2399-120">Request headers</span></span>
|<span data-ttu-id="b2399-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b2399-121">Header</span></span>|<span data-ttu-id="b2399-122">値</span><span class="sxs-lookup"><span data-stu-id="b2399-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b2399-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b2399-123">Authorization</span></span>|<span data-ttu-id="b2399-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="b2399-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b2399-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b2399-125">Accept</span></span>|<span data-ttu-id="b2399-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b2399-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b2399-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="b2399-127">Request body</span></span>
<span data-ttu-id="b2399-128">要求の本文に managementConditionStatement オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="b2399-128">In the request body, supply a JSON representation for the managementConditionStatement object.</span></span>

<span data-ttu-id="b2399-129">次の表は、managementConditionStatement を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="b2399-129">The following table shows the properties that are required when you create the managementConditionStatement.</span></span>

|<span data-ttu-id="b2399-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b2399-130">Property</span></span>|<span data-ttu-id="b2399-131">型</span><span class="sxs-lookup"><span data-stu-id="b2399-131">Type</span></span>|<span data-ttu-id="b2399-132">説明</span><span class="sxs-lookup"><span data-stu-id="b2399-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b2399-133">id</span><span class="sxs-lookup"><span data-stu-id="b2399-133">id</span></span>|<span data-ttu-id="b2399-134">String</span><span class="sxs-lookup"><span data-stu-id="b2399-134">String</span></span>|<span data-ttu-id="b2399-135">管理条件付きステートメントの一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="b2399-135">Unique identifier for the management condition statement.</span></span> <span data-ttu-id="b2399-136">システムでは、作成時に割り当てられた値が生成されます。</span><span class="sxs-lookup"><span data-stu-id="b2399-136">System generated value assigned when created.</span></span>|
|<span data-ttu-id="b2399-137">displayName</span><span class="sxs-lookup"><span data-stu-id="b2399-137">displayName</span></span>|<span data-ttu-id="b2399-138">String</span><span class="sxs-lookup"><span data-stu-id="b2399-138">String</span></span>|<span data-ttu-id="b2399-139">管理者は、管理条件ステートメントの名前を定義します。</span><span class="sxs-lookup"><span data-stu-id="b2399-139">The admin defined name of the management condition statement.</span></span>|
|<span data-ttu-id="b2399-140">説明</span><span class="sxs-lookup"><span data-stu-id="b2399-140">description</span></span>|<span data-ttu-id="b2399-141">String</span><span class="sxs-lookup"><span data-stu-id="b2399-141">String</span></span>|<span data-ttu-id="b2399-142">管理者は、管理条件付きステートメントの説明を定義します。</span><span class="sxs-lookup"><span data-stu-id="b2399-142">The admin defined description of the management condition statement.</span></span>|
|<span data-ttu-id="b2399-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b2399-143">createdDateTime</span></span>|<span data-ttu-id="b2399-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b2399-144">DateTimeOffset</span></span>|<span data-ttu-id="b2399-145">管理条件付きステートメントが作成された時刻。</span><span class="sxs-lookup"><span data-stu-id="b2399-145">The time the management condition statement was created.</span></span> <span data-ttu-id="b2399-146">サービス側が生成されます。</span><span class="sxs-lookup"><span data-stu-id="b2399-146">Generated service side.</span></span>|
|<span data-ttu-id="b2399-147">変更された日時</span><span class="sxs-lookup"><span data-stu-id="b2399-147">modifiedDateTime</span></span>|<span data-ttu-id="b2399-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b2399-148">DateTimeOffset</span></span>|<span data-ttu-id="b2399-149">管理条件付きステートメントが最後に修正された時間です。</span><span class="sxs-lookup"><span data-stu-id="b2399-149">The time the management condition statement was last modified.</span></span> <span data-ttu-id="b2399-150">サービス側を更新します。</span><span class="sxs-lookup"><span data-stu-id="b2399-150">Updated service side.</span></span>|
|<span data-ttu-id="b2399-151">式</span><span class="sxs-lookup"><span data-stu-id="b2399-151">expression</span></span>|[<span data-ttu-id="b2399-152">managementConditionExpression</span><span class="sxs-lookup"><span data-stu-id="b2399-152">managementConditionExpression</span></span>](../resources/intune-fencing-managementconditionexpression.md)|<span data-ttu-id="b2399-153">場合は、管理条件ステートメントを評価するために使用、管理条件ステートメントの式は、アクティブ/非アクティブでした。</span><span class="sxs-lookup"><span data-stu-id="b2399-153">The management condition statement expression used to evaluate if a management condition statement was activated/deactivated.</span></span>|
|<span data-ttu-id="b2399-154">eTag</span><span class="sxs-lookup"><span data-stu-id="b2399-154">eTag</span></span>|<span data-ttu-id="b2399-155">String</span><span class="sxs-lookup"><span data-stu-id="b2399-155">String</span></span>|<span data-ttu-id="b2399-156">管理条件付きステートメントの ETag。</span><span class="sxs-lookup"><span data-stu-id="b2399-156">ETag of the management condition statement.</span></span> <span data-ttu-id="b2399-157">サービス側を更新します。</span><span class="sxs-lookup"><span data-stu-id="b2399-157">Updated service side.</span></span>|
|<span data-ttu-id="b2399-158">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="b2399-158">applicablePlatforms</span></span>|<span data-ttu-id="b2399-159">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="b2399-159">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="b2399-160">この管理条件ステートメントに適用可能なプラットフォームです。</span><span class="sxs-lookup"><span data-stu-id="b2399-160">The applicable platforms for this management condition statement.</span></span>
<span data-ttu-id="b2399-161">管理に関連付けられている管理の条件を見てからこの計算は、ステートメントと該当するプラットフォームの交点の検出の条件です。</span><span class="sxs-lookup"><span data-stu-id="b2399-161">This is calculated from looking the management conditions associated to the management condition statement and finding the intersection of applicable platforms.</span></span> <span data-ttu-id="b2399-162">可能な値は、`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile` です。</span><span class="sxs-lookup"><span data-stu-id="b2399-162">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.</span></span>|



## <a name="response"></a><span data-ttu-id="b2399-163">応答</span><span class="sxs-lookup"><span data-stu-id="b2399-163">Response</span></span>
<span data-ttu-id="b2399-164">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="b2399-164">If successful, this method returns a `201 Created` response code and a [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b2399-165">例</span><span class="sxs-lookup"><span data-stu-id="b2399-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="b2399-166">要求</span><span class="sxs-lookup"><span data-stu-id="b2399-166">Request</span></span>
<span data-ttu-id="b2399-167">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b2399-167">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managementConditionStatements
Content-type: application/json
Content-length: 323

{
  "@odata.type": "#microsoft.graph.managementConditionStatement",
  "displayName": "Display Name value",
  "description": "Description value",
  "expression": {
    "@odata.type": "microsoft.graph.managementConditionExpression"
  },
  "eTag": "ETag value",
  "applicablePlatforms": [
    "androidForWork"
  ]
}
```

### <a name="response"></a><span data-ttu-id="b2399-168">応答</span><span class="sxs-lookup"><span data-stu-id="b2399-168">Response</span></span>
<span data-ttu-id="b2399-p108">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b2399-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 491

{
  "@odata.type": "#microsoft.graph.managementConditionStatement",
  "id": "bedb0c00-0c00-bedb-000c-dbbe000cdbbe",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
  "expression": {
    "@odata.type": "microsoft.graph.managementConditionExpression"
  },
  "eTag": "ETag value",
  "applicablePlatforms": [
    "androidForWork"
  ]
}
```




