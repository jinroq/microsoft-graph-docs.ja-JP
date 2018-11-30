---
title: ManagementConditionStatement を更新します。
description: ManagementConditionStatement オブジェクトのプロパティを更新します。
ms.openlocfilehash: a4fd1ae650f0523a0e56498949c3feafd08b8a25
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073704"
---
# <a name="update-managementconditionstatement"></a><span data-ttu-id="9b9a4-103">ManagementConditionStatement を更新します。</span><span class="sxs-lookup"><span data-stu-id="9b9a4-103">Update managementConditionStatement</span></span>

> <span data-ttu-id="9b9a4-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="9b9a4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9b9a4-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9b9a4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9b9a4-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="9b9a4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9b9a4-107">[ManagementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="9b9a4-107">Update the properties of a [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9b9a4-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="9b9a4-108">Prerequisites</span></span>
<span data-ttu-id="9b9a4-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9b9a4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9b9a4-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9b9a4-111">Permission type</span></span>|<span data-ttu-id="9b9a4-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="9b9a4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9b9a4-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9b9a4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9b9a4-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9b9a4-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9b9a4-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9b9a4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9b9a4-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9b9a4-116">Not supported.</span></span>|
|<span data-ttu-id="9b9a4-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9b9a4-117">Application</span></span>|<span data-ttu-id="9b9a4-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9b9a4-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9b9a4-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9b9a4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managementConditionStatements/{managementConditionStatementId}
PATCH /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}
```

## <a name="request-headers"></a><span data-ttu-id="9b9a4-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9b9a4-120">Request headers</span></span>
|<span data-ttu-id="9b9a4-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9b9a4-121">Header</span></span>|<span data-ttu-id="9b9a4-122">値</span><span class="sxs-lookup"><span data-stu-id="9b9a4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9b9a4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9b9a4-123">Authorization</span></span>|<span data-ttu-id="9b9a4-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="9b9a4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9b9a4-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9b9a4-125">Accept</span></span>|<span data-ttu-id="9b9a4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9b9a4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9b9a4-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="9b9a4-127">Request body</span></span>
<span data-ttu-id="9b9a4-128">要求の本文に[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="9b9a4-128">In the request body, supply a JSON representation for the [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object.</span></span>

<span data-ttu-id="9b9a4-129">[ManagementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="9b9a4-129">The following table shows the properties that are required when you create the [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md).</span></span>

|<span data-ttu-id="9b9a4-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9b9a4-130">Property</span></span>|<span data-ttu-id="9b9a4-131">型</span><span class="sxs-lookup"><span data-stu-id="9b9a4-131">Type</span></span>|<span data-ttu-id="9b9a4-132">説明</span><span class="sxs-lookup"><span data-stu-id="9b9a4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9b9a4-133">id</span><span class="sxs-lookup"><span data-stu-id="9b9a4-133">id</span></span>|<span data-ttu-id="9b9a4-134">String</span><span class="sxs-lookup"><span data-stu-id="9b9a4-134">String</span></span>|<span data-ttu-id="9b9a4-135">管理条件付きステートメントの一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="9b9a4-135">Unique identifier for the management condition statement.</span></span> <span data-ttu-id="9b9a4-136">システムでは、作成時に割り当てられた値が生成されます。</span><span class="sxs-lookup"><span data-stu-id="9b9a4-136">System generated value assigned when created.</span></span>|
|<span data-ttu-id="9b9a4-137">displayName</span><span class="sxs-lookup"><span data-stu-id="9b9a4-137">displayName</span></span>|<span data-ttu-id="9b9a4-138">String</span><span class="sxs-lookup"><span data-stu-id="9b9a4-138">String</span></span>|<span data-ttu-id="9b9a4-139">管理者は、管理条件ステートメントの名前を定義します。</span><span class="sxs-lookup"><span data-stu-id="9b9a4-139">The admin defined name of the management condition statement.</span></span>|
|<span data-ttu-id="9b9a4-140">説明</span><span class="sxs-lookup"><span data-stu-id="9b9a4-140">description</span></span>|<span data-ttu-id="9b9a4-141">String</span><span class="sxs-lookup"><span data-stu-id="9b9a4-141">String</span></span>|<span data-ttu-id="9b9a4-142">管理者は、管理条件付きステートメントの説明を定義します。</span><span class="sxs-lookup"><span data-stu-id="9b9a4-142">The admin defined description of the management condition statement.</span></span>|
|<span data-ttu-id="9b9a4-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9b9a4-143">createdDateTime</span></span>|<span data-ttu-id="9b9a4-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9b9a4-144">DateTimeOffset</span></span>|<span data-ttu-id="9b9a4-145">管理条件付きステートメントが作成された時刻。</span><span class="sxs-lookup"><span data-stu-id="9b9a4-145">The time the management condition statement was created.</span></span> <span data-ttu-id="9b9a4-146">サービス側が生成されます。</span><span class="sxs-lookup"><span data-stu-id="9b9a4-146">Generated service side.</span></span>|
|<span data-ttu-id="9b9a4-147">変更された日時</span><span class="sxs-lookup"><span data-stu-id="9b9a4-147">modifiedDateTime</span></span>|<span data-ttu-id="9b9a4-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9b9a4-148">DateTimeOffset</span></span>|<span data-ttu-id="9b9a4-149">管理条件付きステートメントが最後に修正された時間です。</span><span class="sxs-lookup"><span data-stu-id="9b9a4-149">The time the management condition statement was last modified.</span></span> <span data-ttu-id="9b9a4-150">サービス側を更新します。</span><span class="sxs-lookup"><span data-stu-id="9b9a4-150">Updated service side.</span></span>|
|<span data-ttu-id="9b9a4-151">式</span><span class="sxs-lookup"><span data-stu-id="9b9a4-151">expression</span></span>|[<span data-ttu-id="9b9a4-152">managementConditionExpression</span><span class="sxs-lookup"><span data-stu-id="9b9a4-152">managementConditionExpression</span></span>](../resources/intune-fencing-managementconditionexpression.md)|<span data-ttu-id="9b9a4-153">場合は、管理条件ステートメントを評価するために使用、管理条件ステートメントの式は、アクティブ/非アクティブでした。</span><span class="sxs-lookup"><span data-stu-id="9b9a4-153">The management condition statement expression used to evaluate if a management condition statement was activated/deactivated.</span></span>|
|<span data-ttu-id="9b9a4-154">eTag</span><span class="sxs-lookup"><span data-stu-id="9b9a4-154">eTag</span></span>|<span data-ttu-id="9b9a4-155">String</span><span class="sxs-lookup"><span data-stu-id="9b9a4-155">String</span></span>|<span data-ttu-id="9b9a4-156">管理条件付きステートメントの ETag。</span><span class="sxs-lookup"><span data-stu-id="9b9a4-156">ETag of the management condition statement.</span></span> <span data-ttu-id="9b9a4-157">サービス側を更新します。</span><span class="sxs-lookup"><span data-stu-id="9b9a4-157">Updated service side.</span></span>|
|<span data-ttu-id="9b9a4-158">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="9b9a4-158">applicablePlatforms</span></span>|<span data-ttu-id="9b9a4-159">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="9b9a4-159">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="9b9a4-160">この管理条件ステートメントに適用可能なプラットフォームです。</span><span class="sxs-lookup"><span data-stu-id="9b9a4-160">The applicable platforms for this management condition statement.</span></span>
<span data-ttu-id="9b9a4-161">管理に関連付けられている管理の条件を見てからこの計算は、ステートメントと該当するプラットフォームの交点の検出の条件です。</span><span class="sxs-lookup"><span data-stu-id="9b9a4-161">This is calculated from looking the management conditions associated to the management condition statement and finding the intersection of applicable platforms.</span></span> <span data-ttu-id="9b9a4-162">可能な値は、`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile` です。</span><span class="sxs-lookup"><span data-stu-id="9b9a4-162">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.</span></span>|



## <a name="response"></a><span data-ttu-id="9b9a4-163">応答</span><span class="sxs-lookup"><span data-stu-id="9b9a4-163">Response</span></span>
<span data-ttu-id="9b9a4-164">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="9b9a4-164">If successful, this method returns a `200 OK` response code and an updated [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9b9a4-165">例</span><span class="sxs-lookup"><span data-stu-id="9b9a4-165">Example</span></span>
### <a name="request"></a><span data-ttu-id="9b9a4-166">要求</span><span class="sxs-lookup"><span data-stu-id="9b9a4-166">Request</span></span>
<span data-ttu-id="9b9a4-167">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="9b9a4-167">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/managementConditionStatements/{managementConditionStatementId}
Content-type: application/json
Content-length: 256

{
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

### <a name="response"></a><span data-ttu-id="9b9a4-168">応答</span><span class="sxs-lookup"><span data-stu-id="9b9a4-168">Response</span></span>
<span data-ttu-id="9b9a4-p108">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="9b9a4-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





