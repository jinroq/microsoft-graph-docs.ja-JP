---
title: ManagementConditionStatement を作成します。
description: 新しい managementConditionStatement オブジェクトを作成します。
author: tfitzmac
ms.openlocfilehash: 5402faee0c7ace84957f3ff6a2ef65844f5a527e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27327350"
---
# <a name="create-managementconditionstatement"></a><span data-ttu-id="3ce82-103">ManagementConditionStatement を作成します。</span><span class="sxs-lookup"><span data-stu-id="3ce82-103">Create managementConditionStatement</span></span>

> <span data-ttu-id="3ce82-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="3ce82-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3ce82-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3ce82-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3ce82-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="3ce82-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3ce82-107">新しい[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="3ce82-107">Create a new [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3ce82-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="3ce82-108">Prerequisites</span></span>
<span data-ttu-id="3ce82-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3ce82-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3ce82-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3ce82-111">Permission type</span></span>|<span data-ttu-id="3ce82-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="3ce82-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3ce82-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3ce82-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3ce82-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ce82-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3ce82-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3ce82-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3ce82-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3ce82-116">Not supported.</span></span>|
|<span data-ttu-id="3ce82-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3ce82-117">Application</span></span>|<span data-ttu-id="3ce82-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3ce82-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3ce82-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3ce82-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managementConditionStatements
POST /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements
```

## <a name="request-headers"></a><span data-ttu-id="3ce82-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3ce82-120">Request headers</span></span>
|<span data-ttu-id="3ce82-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3ce82-121">Header</span></span>|<span data-ttu-id="3ce82-122">値</span><span class="sxs-lookup"><span data-stu-id="3ce82-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3ce82-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3ce82-123">Authorization</span></span>|<span data-ttu-id="3ce82-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="3ce82-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3ce82-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3ce82-125">Accept</span></span>|<span data-ttu-id="3ce82-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3ce82-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3ce82-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="3ce82-127">Request body</span></span>
<span data-ttu-id="3ce82-128">要求の本文に managementConditionStatement オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="3ce82-128">In the request body, supply a JSON representation for the managementConditionStatement object.</span></span>

<span data-ttu-id="3ce82-129">次の表は、managementConditionStatement を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="3ce82-129">The following table shows the properties that are required when you create the managementConditionStatement.</span></span>

|<span data-ttu-id="3ce82-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3ce82-130">Property</span></span>|<span data-ttu-id="3ce82-131">種類</span><span class="sxs-lookup"><span data-stu-id="3ce82-131">Type</span></span>|<span data-ttu-id="3ce82-132">説明</span><span class="sxs-lookup"><span data-stu-id="3ce82-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3ce82-133">ID</span><span class="sxs-lookup"><span data-stu-id="3ce82-133">id</span></span>|<span data-ttu-id="3ce82-134">String</span><span class="sxs-lookup"><span data-stu-id="3ce82-134">String</span></span>|<span data-ttu-id="3ce82-135">管理条件付きステートメントの一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="3ce82-135">Unique identifier for the management condition statement.</span></span> <span data-ttu-id="3ce82-136">システムでは、作成時に割り当てられた値が生成されます。</span><span class="sxs-lookup"><span data-stu-id="3ce82-136">System generated value assigned when created.</span></span>|
|<span data-ttu-id="3ce82-137">displayName</span><span class="sxs-lookup"><span data-stu-id="3ce82-137">displayName</span></span>|<span data-ttu-id="3ce82-138">String</span><span class="sxs-lookup"><span data-stu-id="3ce82-138">String</span></span>|<span data-ttu-id="3ce82-139">管理者は、管理条件ステートメントの名前を定義します。</span><span class="sxs-lookup"><span data-stu-id="3ce82-139">The admin defined name of the management condition statement.</span></span>|
|<span data-ttu-id="3ce82-140">説明</span><span class="sxs-lookup"><span data-stu-id="3ce82-140">description</span></span>|<span data-ttu-id="3ce82-141">String</span><span class="sxs-lookup"><span data-stu-id="3ce82-141">String</span></span>|<span data-ttu-id="3ce82-142">管理者は、管理条件付きステートメントの説明を定義します。</span><span class="sxs-lookup"><span data-stu-id="3ce82-142">The admin defined description of the management condition statement.</span></span>|
|<span data-ttu-id="3ce82-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3ce82-143">createdDateTime</span></span>|<span data-ttu-id="3ce82-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3ce82-144">DateTimeOffset</span></span>|<span data-ttu-id="3ce82-145">管理条件付きステートメントが作成された時刻。</span><span class="sxs-lookup"><span data-stu-id="3ce82-145">The time the management condition statement was created.</span></span> <span data-ttu-id="3ce82-146">サービス側が生成されます。</span><span class="sxs-lookup"><span data-stu-id="3ce82-146">Generated service side.</span></span>|
|<span data-ttu-id="3ce82-147">変更された日時</span><span class="sxs-lookup"><span data-stu-id="3ce82-147">modifiedDateTime</span></span>|<span data-ttu-id="3ce82-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3ce82-148">DateTimeOffset</span></span>|<span data-ttu-id="3ce82-149">管理条件付きステートメントが最後に修正された時間です。</span><span class="sxs-lookup"><span data-stu-id="3ce82-149">The time the management condition statement was last modified.</span></span> <span data-ttu-id="3ce82-150">サービス側を更新します。</span><span class="sxs-lookup"><span data-stu-id="3ce82-150">Updated service side.</span></span>|
|<span data-ttu-id="3ce82-151">式</span><span class="sxs-lookup"><span data-stu-id="3ce82-151">expression</span></span>|[<span data-ttu-id="3ce82-152">managementConditionExpression</span><span class="sxs-lookup"><span data-stu-id="3ce82-152">managementConditionExpression</span></span>](../resources/intune-fencing-managementconditionexpression.md)|<span data-ttu-id="3ce82-153">場合は、管理条件ステートメントを評価するために使用、管理条件ステートメントの式は、アクティブ/非アクティブでした。</span><span class="sxs-lookup"><span data-stu-id="3ce82-153">The management condition statement expression used to evaluate if a management condition statement was activated/deactivated.</span></span>|
|<span data-ttu-id="3ce82-154">eTag</span><span class="sxs-lookup"><span data-stu-id="3ce82-154">eTag</span></span>|<span data-ttu-id="3ce82-155">String</span><span class="sxs-lookup"><span data-stu-id="3ce82-155">String</span></span>|<span data-ttu-id="3ce82-156">管理条件付きステートメントの ETag。</span><span class="sxs-lookup"><span data-stu-id="3ce82-156">ETag of the management condition statement.</span></span> <span data-ttu-id="3ce82-157">サービス側を更新します。</span><span class="sxs-lookup"><span data-stu-id="3ce82-157">Updated service side.</span></span>|
|<span data-ttu-id="3ce82-158">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="3ce82-158">applicablePlatforms</span></span>|<span data-ttu-id="3ce82-159">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="3ce82-159">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="3ce82-160">この管理条件ステートメントに適用可能なプラットフォームです。</span><span class="sxs-lookup"><span data-stu-id="3ce82-160">The applicable platforms for this management condition statement.</span></span>
<span data-ttu-id="3ce82-161">管理に関連付けられている管理の条件を見てからこの計算は、ステートメントと該当するプラットフォームの交点の検出の条件です。</span><span class="sxs-lookup"><span data-stu-id="3ce82-161">This is calculated from looking the management conditions associated to the management condition statement and finding the intersection of applicable platforms.</span></span> <span data-ttu-id="3ce82-162">可能な値は、`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile` です。</span><span class="sxs-lookup"><span data-stu-id="3ce82-162">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.</span></span>|



## <a name="response"></a><span data-ttu-id="3ce82-163">応答</span><span class="sxs-lookup"><span data-stu-id="3ce82-163">Response</span></span>
<span data-ttu-id="3ce82-164">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="3ce82-164">If successful, this method returns a `201 Created` response code and a [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3ce82-165">例</span><span class="sxs-lookup"><span data-stu-id="3ce82-165">Example</span></span>
### <a name="request"></a><span data-ttu-id="3ce82-166">要求</span><span class="sxs-lookup"><span data-stu-id="3ce82-166">Request</span></span>
<span data-ttu-id="3ce82-167">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="3ce82-167">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="3ce82-168">応答</span><span class="sxs-lookup"><span data-stu-id="3ce82-168">Response</span></span>
<span data-ttu-id="3ce82-p108">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="3ce82-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




