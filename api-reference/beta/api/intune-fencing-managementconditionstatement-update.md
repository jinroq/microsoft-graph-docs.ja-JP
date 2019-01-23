---
title: ManagementConditionStatement を更新します。
description: ManagementConditionStatement オブジェクトのプロパティを更新します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 02d5301ca81bf5b1479454f65a6c9e9630a8f284
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29417043"
---
# <a name="update-managementconditionstatement"></a><span data-ttu-id="b45cc-103">ManagementConditionStatement を更新します。</span><span class="sxs-lookup"><span data-stu-id="b45cc-103">Update managementConditionStatement</span></span>

> <span data-ttu-id="b45cc-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b45cc-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b45cc-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b45cc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b45cc-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b45cc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b45cc-107">[ManagementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="b45cc-107">Update the properties of a [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b45cc-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="b45cc-108">Prerequisites</span></span>
<span data-ttu-id="b45cc-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b45cc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b45cc-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b45cc-111">Permission type</span></span>|<span data-ttu-id="b45cc-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="b45cc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b45cc-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b45cc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b45cc-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b45cc-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b45cc-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b45cc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b45cc-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b45cc-116">Not supported.</span></span>|
|<span data-ttu-id="b45cc-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b45cc-117">Application</span></span>|<span data-ttu-id="b45cc-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b45cc-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b45cc-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b45cc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managementConditionStatements/{managementConditionStatementId}
PATCH /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}
```

## <a name="request-headers"></a><span data-ttu-id="b45cc-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b45cc-120">Request headers</span></span>
|<span data-ttu-id="b45cc-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b45cc-121">Header</span></span>|<span data-ttu-id="b45cc-122">値</span><span class="sxs-lookup"><span data-stu-id="b45cc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b45cc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b45cc-123">Authorization</span></span>|<span data-ttu-id="b45cc-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="b45cc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b45cc-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b45cc-125">Accept</span></span>|<span data-ttu-id="b45cc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b45cc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b45cc-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="b45cc-127">Request body</span></span>
<span data-ttu-id="b45cc-128">要求の本文に[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="b45cc-128">In the request body, supply a JSON representation for the [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object.</span></span>

<span data-ttu-id="b45cc-129">[ManagementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="b45cc-129">The following table shows the properties that are required when you create the [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md).</span></span>

|<span data-ttu-id="b45cc-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b45cc-130">Property</span></span>|<span data-ttu-id="b45cc-131">型</span><span class="sxs-lookup"><span data-stu-id="b45cc-131">Type</span></span>|<span data-ttu-id="b45cc-132">説明</span><span class="sxs-lookup"><span data-stu-id="b45cc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b45cc-133">id</span><span class="sxs-lookup"><span data-stu-id="b45cc-133">id</span></span>|<span data-ttu-id="b45cc-134">String</span><span class="sxs-lookup"><span data-stu-id="b45cc-134">String</span></span>|<span data-ttu-id="b45cc-135">管理条件付きステートメントの一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="b45cc-135">Unique identifier for the management condition statement.</span></span> <span data-ttu-id="b45cc-136">システムでは、作成時に割り当てられた値が生成されます。</span><span class="sxs-lookup"><span data-stu-id="b45cc-136">System generated value assigned when created.</span></span>|
|<span data-ttu-id="b45cc-137">displayName</span><span class="sxs-lookup"><span data-stu-id="b45cc-137">displayName</span></span>|<span data-ttu-id="b45cc-138">String</span><span class="sxs-lookup"><span data-stu-id="b45cc-138">String</span></span>|<span data-ttu-id="b45cc-139">管理者は、管理条件ステートメントの名前を定義します。</span><span class="sxs-lookup"><span data-stu-id="b45cc-139">The admin defined name of the management condition statement.</span></span>|
|<span data-ttu-id="b45cc-140">説明</span><span class="sxs-lookup"><span data-stu-id="b45cc-140">description</span></span>|<span data-ttu-id="b45cc-141">String</span><span class="sxs-lookup"><span data-stu-id="b45cc-141">String</span></span>|<span data-ttu-id="b45cc-142">管理者は、管理条件付きステートメントの説明を定義します。</span><span class="sxs-lookup"><span data-stu-id="b45cc-142">The admin defined description of the management condition statement.</span></span>|
|<span data-ttu-id="b45cc-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b45cc-143">createdDateTime</span></span>|<span data-ttu-id="b45cc-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b45cc-144">DateTimeOffset</span></span>|<span data-ttu-id="b45cc-145">管理条件付きステートメントが作成された時刻。</span><span class="sxs-lookup"><span data-stu-id="b45cc-145">The time the management condition statement was created.</span></span> <span data-ttu-id="b45cc-146">サービス側が生成されます。</span><span class="sxs-lookup"><span data-stu-id="b45cc-146">Generated service side.</span></span>|
|<span data-ttu-id="b45cc-147">変更された日時</span><span class="sxs-lookup"><span data-stu-id="b45cc-147">modifiedDateTime</span></span>|<span data-ttu-id="b45cc-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b45cc-148">DateTimeOffset</span></span>|<span data-ttu-id="b45cc-149">管理条件付きステートメントが最後に修正された時間です。</span><span class="sxs-lookup"><span data-stu-id="b45cc-149">The time the management condition statement was last modified.</span></span> <span data-ttu-id="b45cc-150">サービス側を更新します。</span><span class="sxs-lookup"><span data-stu-id="b45cc-150">Updated service side.</span></span>|
|<span data-ttu-id="b45cc-151">式</span><span class="sxs-lookup"><span data-stu-id="b45cc-151">expression</span></span>|[<span data-ttu-id="b45cc-152">managementConditionExpression</span><span class="sxs-lookup"><span data-stu-id="b45cc-152">managementConditionExpression</span></span>](../resources/intune-fencing-managementconditionexpression.md)|<span data-ttu-id="b45cc-153">場合は、管理条件ステートメントを評価するために使用、管理条件ステートメントの式は、アクティブ/非アクティブでした。</span><span class="sxs-lookup"><span data-stu-id="b45cc-153">The management condition statement expression used to evaluate if a management condition statement was activated/deactivated.</span></span>|
|<span data-ttu-id="b45cc-154">eTag</span><span class="sxs-lookup"><span data-stu-id="b45cc-154">eTag</span></span>|<span data-ttu-id="b45cc-155">String</span><span class="sxs-lookup"><span data-stu-id="b45cc-155">String</span></span>|<span data-ttu-id="b45cc-156">管理条件付きステートメントの ETag。</span><span class="sxs-lookup"><span data-stu-id="b45cc-156">ETag of the management condition statement.</span></span> <span data-ttu-id="b45cc-157">サービス側を更新します。</span><span class="sxs-lookup"><span data-stu-id="b45cc-157">Updated service side.</span></span>|
|<span data-ttu-id="b45cc-158">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="b45cc-158">applicablePlatforms</span></span>|<span data-ttu-id="b45cc-159">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="b45cc-159">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="b45cc-160">この管理条件ステートメントに適用可能なプラットフォームです。</span><span class="sxs-lookup"><span data-stu-id="b45cc-160">The applicable platforms for this management condition statement.</span></span>
<span data-ttu-id="b45cc-161">管理に関連付けられている管理の条件を見てからこの計算は、ステートメントと該当するプラットフォームの交点の検出の条件です。</span><span class="sxs-lookup"><span data-stu-id="b45cc-161">This is calculated from looking the management conditions associated to the management condition statement and finding the intersection of applicable platforms.</span></span> <span data-ttu-id="b45cc-162">可能な値は、`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile` です。</span><span class="sxs-lookup"><span data-stu-id="b45cc-162">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.</span></span>|



## <a name="response"></a><span data-ttu-id="b45cc-163">応答</span><span class="sxs-lookup"><span data-stu-id="b45cc-163">Response</span></span>
<span data-ttu-id="b45cc-164">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="b45cc-164">If successful, this method returns a `200 OK` response code and an updated [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b45cc-165">例</span><span class="sxs-lookup"><span data-stu-id="b45cc-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="b45cc-166">要求</span><span class="sxs-lookup"><span data-stu-id="b45cc-166">Request</span></span>
<span data-ttu-id="b45cc-167">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b45cc-167">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/managementConditionStatements/{managementConditionStatementId}
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

### <a name="response"></a><span data-ttu-id="b45cc-168">応答</span><span class="sxs-lookup"><span data-stu-id="b45cc-168">Response</span></span>
<span data-ttu-id="b45cc-p108">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b45cc-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




