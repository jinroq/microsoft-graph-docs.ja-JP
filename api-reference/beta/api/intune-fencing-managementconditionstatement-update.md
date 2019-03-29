---
title: managementconditionstatement の更新
description: managementconditionstatement オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1c2211d202ddc875a0da24d9f0d5bbe959f092ae
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30969408"
---
# <a name="update-managementconditionstatement"></a><span data-ttu-id="0fec5-103">managementconditionstatement の更新</span><span class="sxs-lookup"><span data-stu-id="0fec5-103">Update managementConditionStatement</span></span>

> <span data-ttu-id="0fec5-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0fec5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0fec5-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0fec5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0fec5-106">[managementconditionstatement](../resources/intune-fencing-managementconditionstatement.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="0fec5-106">Update the properties of a [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0fec5-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="0fec5-107">Prerequisites</span></span>
<span data-ttu-id="0fec5-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0fec5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0fec5-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0fec5-110">Permission type</span></span>|<span data-ttu-id="0fec5-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="0fec5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0fec5-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0fec5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0fec5-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0fec5-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0fec5-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0fec5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0fec5-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0fec5-115">Not supported.</span></span>|
|<span data-ttu-id="0fec5-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0fec5-116">Application</span></span>|<span data-ttu-id="0fec5-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0fec5-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0fec5-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0fec5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managementConditionStatements/{managementConditionStatementId}
PATCH /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}
```

## <a name="request-headers"></a><span data-ttu-id="0fec5-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0fec5-119">Request headers</span></span>
|<span data-ttu-id="0fec5-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0fec5-120">Header</span></span>|<span data-ttu-id="0fec5-121">値</span><span class="sxs-lookup"><span data-stu-id="0fec5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0fec5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0fec5-122">Authorization</span></span>|<span data-ttu-id="0fec5-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="0fec5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0fec5-124">承諾</span><span class="sxs-lookup"><span data-stu-id="0fec5-124">Accept</span></span>|<span data-ttu-id="0fec5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0fec5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0fec5-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="0fec5-126">Request body</span></span>
<span data-ttu-id="0fec5-127">要求本文で、 [managementconditionstatement](../resources/intune-fencing-managementconditionstatement.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="0fec5-127">In the request body, supply a JSON representation for the [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object.</span></span>

<span data-ttu-id="0fec5-128">次の表に、 [managementconditionstatement](../resources/intune-fencing-managementconditionstatement.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="0fec5-128">The following table shows the properties that are required when you create the [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md).</span></span>

|<span data-ttu-id="0fec5-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0fec5-129">Property</span></span>|<span data-ttu-id="0fec5-130">型</span><span class="sxs-lookup"><span data-stu-id="0fec5-130">Type</span></span>|<span data-ttu-id="0fec5-131">説明</span><span class="sxs-lookup"><span data-stu-id="0fec5-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0fec5-132">id</span><span class="sxs-lookup"><span data-stu-id="0fec5-132">id</span></span>|<span data-ttu-id="0fec5-133">String</span><span class="sxs-lookup"><span data-stu-id="0fec5-133">String</span></span>|<span data-ttu-id="0fec5-134">管理条件ステートメントの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="0fec5-134">Unique identifier for the management condition statement.</span></span> <span data-ttu-id="0fec5-135">作成時に割り当てられたシステム生成値。</span><span class="sxs-lookup"><span data-stu-id="0fec5-135">System generated value assigned when created.</span></span>|
|<span data-ttu-id="0fec5-136">displayName</span><span class="sxs-lookup"><span data-stu-id="0fec5-136">displayName</span></span>|<span data-ttu-id="0fec5-137">String</span><span class="sxs-lookup"><span data-stu-id="0fec5-137">String</span></span>|<span data-ttu-id="0fec5-138">管理条件ステートメントの管理者定義の名前。</span><span class="sxs-lookup"><span data-stu-id="0fec5-138">The admin defined name of the management condition statement.</span></span>|
|<span data-ttu-id="0fec5-139">description</span><span class="sxs-lookup"><span data-stu-id="0fec5-139">description</span></span>|<span data-ttu-id="0fec5-140">String</span><span class="sxs-lookup"><span data-stu-id="0fec5-140">String</span></span>|<span data-ttu-id="0fec5-141">管理条件ステートメントの管理者定義の説明。</span><span class="sxs-lookup"><span data-stu-id="0fec5-141">The admin defined description of the management condition statement.</span></span>|
|<span data-ttu-id="0fec5-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0fec5-142">createdDateTime</span></span>|<span data-ttu-id="0fec5-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0fec5-143">DateTimeOffset</span></span>|<span data-ttu-id="0fec5-144">管理条件ステートメントが作成された時刻。</span><span class="sxs-lookup"><span data-stu-id="0fec5-144">The time the management condition statement was created.</span></span> <span data-ttu-id="0fec5-145">サービス側を生成しました。</span><span class="sxs-lookup"><span data-stu-id="0fec5-145">Generated service side.</span></span>|
|<span data-ttu-id="0fec5-146">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0fec5-146">modifiedDateTime</span></span>|<span data-ttu-id="0fec5-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0fec5-147">DateTimeOffset</span></span>|<span data-ttu-id="0fec5-148">管理条件ステートメントが最後に変更された時刻。</span><span class="sxs-lookup"><span data-stu-id="0fec5-148">The time the management condition statement was last modified.</span></span> <span data-ttu-id="0fec5-149">サービス側を更新しました。</span><span class="sxs-lookup"><span data-stu-id="0fec5-149">Updated service side.</span></span>|
|<span data-ttu-id="0fec5-150">式</span><span class="sxs-lookup"><span data-stu-id="0fec5-150">expression</span></span>|[<span data-ttu-id="0fec5-151">managementconditionexpression</span><span class="sxs-lookup"><span data-stu-id="0fec5-151">managementConditionExpression</span></span>](../resources/intune-fencing-managementconditionexpression.md)|<span data-ttu-id="0fec5-152">管理条件ステートメントがアクティブ化/非アクティブ化されたかどうかを評価するために使用される管理条件ステートメント式。</span><span class="sxs-lookup"><span data-stu-id="0fec5-152">The management condition statement expression used to evaluate if a management condition statement was activated/deactivated.</span></span>|
|<span data-ttu-id="0fec5-153">eTag</span><span class="sxs-lookup"><span data-stu-id="0fec5-153">eTag</span></span>|<span data-ttu-id="0fec5-154">String</span><span class="sxs-lookup"><span data-stu-id="0fec5-154">String</span></span>|<span data-ttu-id="0fec5-155">管理条件ステートメントの ETag。</span><span class="sxs-lookup"><span data-stu-id="0fec5-155">ETag of the management condition statement.</span></span> <span data-ttu-id="0fec5-156">サービス側を更新しました。</span><span class="sxs-lookup"><span data-stu-id="0fec5-156">Updated service side.</span></span>|
|<span data-ttu-id="0fec5-157">アプリケーションのプラットフォーム</span><span class="sxs-lookup"><span data-stu-id="0fec5-157">applicablePlatforms</span></span>|<span data-ttu-id="0fec5-158">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="0fec5-158">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="0fec5-159">この管理条件ステートメントの適用可能なプラットフォーム。</span><span class="sxs-lookup"><span data-stu-id="0fec5-159">The applicable platforms for this management condition statement.</span></span>
<span data-ttu-id="0fec5-160">これは、管理条件ステートメントに関連付けられている管理条件を参照して、適用可能なプラットフォームの共通部分を検索することによって計算されます。</span><span class="sxs-lookup"><span data-stu-id="0fec5-160">This is calculated from looking the management conditions associated to the management condition statement and finding the intersection of applicable platforms.</span></span> <span data-ttu-id="0fec5-161">可能な値は、`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile` です。</span><span class="sxs-lookup"><span data-stu-id="0fec5-161">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.</span></span>|



## <a name="response"></a><span data-ttu-id="0fec5-162">応答</span><span class="sxs-lookup"><span data-stu-id="0fec5-162">Response</span></span>
<span data-ttu-id="0fec5-163">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[managementconditionstatement](../resources/intune-fencing-managementconditionstatement.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="0fec5-163">If successful, this method returns a `200 OK` response code and an updated [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0fec5-164">例</span><span class="sxs-lookup"><span data-stu-id="0fec5-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="0fec5-165">要求</span><span class="sxs-lookup"><span data-stu-id="0fec5-165">Request</span></span>
<span data-ttu-id="0fec5-166">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0fec5-166">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0fec5-167">応答</span><span class="sxs-lookup"><span data-stu-id="0fec5-167">Response</span></span>
<span data-ttu-id="0fec5-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0fec5-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




