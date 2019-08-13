---
title: ManagementConditionStatement の作成
description: 新しい managementConditionStatement オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 48f636aa83b73aa7d5c4eee38bb0d9e9c02656f0
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36355609"
---
# <a name="create-managementconditionstatement"></a><span data-ttu-id="f642d-103">ManagementConditionStatement の作成</span><span class="sxs-lookup"><span data-stu-id="f642d-103">Create managementConditionStatement</span></span>

> <span data-ttu-id="f642d-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f642d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f642d-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f642d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f642d-106">新しい[Managementconditionstatement](../resources/intune-fencing-managementconditionstatement.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="f642d-106">Create a new [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f642d-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="f642d-107">Prerequisites</span></span>
<span data-ttu-id="f642d-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f642d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f642d-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f642d-110">Permission type</span></span>|<span data-ttu-id="f642d-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="f642d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f642d-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f642d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f642d-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f642d-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f642d-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f642d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f642d-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f642d-115">Not supported.</span></span>|
|<span data-ttu-id="f642d-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f642d-116">Application</span></span>|<span data-ttu-id="f642d-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f642d-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f642d-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f642d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managementConditionStatements
POST /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements
```

## <a name="request-headers"></a><span data-ttu-id="f642d-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f642d-119">Request headers</span></span>
|<span data-ttu-id="f642d-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f642d-120">Header</span></span>|<span data-ttu-id="f642d-121">値</span><span class="sxs-lookup"><span data-stu-id="f642d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f642d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f642d-122">Authorization</span></span>|<span data-ttu-id="f642d-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="f642d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f642d-124">承諾</span><span class="sxs-lookup"><span data-stu-id="f642d-124">Accept</span></span>|<span data-ttu-id="f642d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f642d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f642d-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="f642d-126">Request body</span></span>
<span data-ttu-id="f642d-127">要求本文で、managementConditionStatement オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="f642d-127">In the request body, supply a JSON representation for the managementConditionStatement object.</span></span>

<span data-ttu-id="f642d-128">次の表に、managementConditionStatement の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="f642d-128">The following table shows the properties that are required when you create the managementConditionStatement.</span></span>

|<span data-ttu-id="f642d-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f642d-129">Property</span></span>|<span data-ttu-id="f642d-130">型</span><span class="sxs-lookup"><span data-stu-id="f642d-130">Type</span></span>|<span data-ttu-id="f642d-131">説明</span><span class="sxs-lookup"><span data-stu-id="f642d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f642d-132">id</span><span class="sxs-lookup"><span data-stu-id="f642d-132">id</span></span>|<span data-ttu-id="f642d-133">文字列</span><span class="sxs-lookup"><span data-stu-id="f642d-133">String</span></span>|<span data-ttu-id="f642d-134">管理条件ステートメントの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="f642d-134">Unique identifier for the management condition statement.</span></span> <span data-ttu-id="f642d-135">作成時に割り当てられたシステム生成値。</span><span class="sxs-lookup"><span data-stu-id="f642d-135">System generated value assigned when created.</span></span>|
|<span data-ttu-id="f642d-136">displayName</span><span class="sxs-lookup"><span data-stu-id="f642d-136">displayName</span></span>|<span data-ttu-id="f642d-137">String</span><span class="sxs-lookup"><span data-stu-id="f642d-137">String</span></span>|<span data-ttu-id="f642d-138">管理条件ステートメントの管理者定義の名前。</span><span class="sxs-lookup"><span data-stu-id="f642d-138">The admin defined name of the management condition statement.</span></span>|
|<span data-ttu-id="f642d-139">description</span><span class="sxs-lookup"><span data-stu-id="f642d-139">description</span></span>|<span data-ttu-id="f642d-140">String</span><span class="sxs-lookup"><span data-stu-id="f642d-140">String</span></span>|<span data-ttu-id="f642d-141">管理条件ステートメントの管理者定義の説明。</span><span class="sxs-lookup"><span data-stu-id="f642d-141">The admin defined description of the management condition statement.</span></span>|
|<span data-ttu-id="f642d-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f642d-142">createdDateTime</span></span>|<span data-ttu-id="f642d-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f642d-143">DateTimeOffset</span></span>|<span data-ttu-id="f642d-144">管理条件ステートメントが作成された時刻。</span><span class="sxs-lookup"><span data-stu-id="f642d-144">The time the management condition statement was created.</span></span> <span data-ttu-id="f642d-145">サービス側を生成しました。</span><span class="sxs-lookup"><span data-stu-id="f642d-145">Generated service side.</span></span>|
|<span data-ttu-id="f642d-146">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f642d-146">modifiedDateTime</span></span>|<span data-ttu-id="f642d-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f642d-147">DateTimeOffset</span></span>|<span data-ttu-id="f642d-148">管理条件ステートメントが最後に変更された時刻。</span><span class="sxs-lookup"><span data-stu-id="f642d-148">The time the management condition statement was last modified.</span></span> <span data-ttu-id="f642d-149">サービス側を更新しました。</span><span class="sxs-lookup"><span data-stu-id="f642d-149">Updated service side.</span></span>|
|<span data-ttu-id="f642d-150">式</span><span class="sxs-lookup"><span data-stu-id="f642d-150">expression</span></span>|[<span data-ttu-id="f642d-151">managementConditionExpression</span><span class="sxs-lookup"><span data-stu-id="f642d-151">managementConditionExpression</span></span>](../resources/intune-fencing-managementconditionexpression.md)|<span data-ttu-id="f642d-152">管理条件ステートメントがアクティブ化/非アクティブ化されたかどうかを評価するために使用される管理条件ステートメント式。</span><span class="sxs-lookup"><span data-stu-id="f642d-152">The management condition statement expression used to evaluate if a management condition statement was activated/deactivated.</span></span>|
|<span data-ttu-id="f642d-153">eTag</span><span class="sxs-lookup"><span data-stu-id="f642d-153">eTag</span></span>|<span data-ttu-id="f642d-154">String</span><span class="sxs-lookup"><span data-stu-id="f642d-154">String</span></span>|<span data-ttu-id="f642d-155">管理条件ステートメントの ETag。</span><span class="sxs-lookup"><span data-stu-id="f642d-155">ETag of the management condition statement.</span></span> <span data-ttu-id="f642d-156">サービス側を更新しました。</span><span class="sxs-lookup"><span data-stu-id="f642d-156">Updated service side.</span></span>|
|<span data-ttu-id="f642d-157">アプリケーションのプラットフォーム</span><span class="sxs-lookup"><span data-stu-id="f642d-157">applicablePlatforms</span></span>|<span data-ttu-id="f642d-158">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="f642d-158">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="f642d-159">この管理条件ステートメントの適用可能なプラットフォーム。</span><span class="sxs-lookup"><span data-stu-id="f642d-159">The applicable platforms for this management condition statement.</span></span>
<span data-ttu-id="f642d-160">これは、管理条件ステートメントに関連付けられている管理条件を参照して、適用可能なプラットフォームの共通部分を検索することによって計算されます。</span><span class="sxs-lookup"><span data-stu-id="f642d-160">This is calculated from looking the management conditions associated to the management condition statement and finding the intersection of applicable platforms.</span></span> <span data-ttu-id="f642d-161">可能な値は、`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`unknown` です。</span><span class="sxs-lookup"><span data-stu-id="f642d-161">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span></span>|



## <a name="response"></a><span data-ttu-id="f642d-162">応答</span><span class="sxs-lookup"><span data-stu-id="f642d-162">Response</span></span>
<span data-ttu-id="f642d-163">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[managementconditionstatement](../resources/intune-fencing-managementconditionstatement.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f642d-163">If successful, this method returns a `201 Created` response code and a [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f642d-164">例</span><span class="sxs-lookup"><span data-stu-id="f642d-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="f642d-165">要求</span><span class="sxs-lookup"><span data-stu-id="f642d-165">Request</span></span>
<span data-ttu-id="f642d-166">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f642d-166">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f642d-167">応答</span><span class="sxs-lookup"><span data-stu-id="f642d-167">Response</span></span>
<span data-ttu-id="f642d-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f642d-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






