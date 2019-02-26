---
title: grouppolicydefinition の更新
description: grouppolicydefinition オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3439c14463118f616847dd5e7f71970fa3d6a8c7
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30157254"
---
# <a name="update-grouppolicydefinition"></a><span data-ttu-id="87e7f-103">grouppolicydefinition の更新</span><span class="sxs-lookup"><span data-stu-id="87e7f-103">Update groupPolicyDefinition</span></span>

> <span data-ttu-id="87e7f-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="87e7f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="87e7f-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="87e7f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="87e7f-106">[grouppolicydefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="87e7f-106">Update the properties of a [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="87e7f-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="87e7f-107">Prerequisites</span></span>
<span data-ttu-id="87e7f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="87e7f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="87e7f-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="87e7f-110">Permission type</span></span>|<span data-ttu-id="87e7f-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="87e7f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="87e7f-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="87e7f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="87e7f-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87e7f-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="87e7f-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="87e7f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="87e7f-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="87e7f-115">Not supported.</span></span>|
|<span data-ttu-id="87e7f-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="87e7f-116">Application</span></span>|<span data-ttu-id="87e7f-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="87e7f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="87e7f-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="87e7f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyDefinitions/{groupPolicyDefinitionId}
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/definition
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/definitionFile/definitions/{groupPolicyDefinitionId}
```

## <a name="request-headers"></a><span data-ttu-id="87e7f-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="87e7f-119">Request headers</span></span>
|<span data-ttu-id="87e7f-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="87e7f-120">Header</span></span>|<span data-ttu-id="87e7f-121">値</span><span class="sxs-lookup"><span data-stu-id="87e7f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="87e7f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="87e7f-122">Authorization</span></span>|<span data-ttu-id="87e7f-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="87e7f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="87e7f-124">承諾</span><span class="sxs-lookup"><span data-stu-id="87e7f-124">Accept</span></span>|<span data-ttu-id="87e7f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="87e7f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="87e7f-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="87e7f-126">Request body</span></span>
<span data-ttu-id="87e7f-127">要求本文で、 [grouppolicydefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="87e7f-127">In the request body, supply a JSON representation for the [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object.</span></span>

<span data-ttu-id="87e7f-128">次の表に、 [grouppolicydefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="87e7f-128">The following table shows the properties that are required when you create the [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md).</span></span>

|<span data-ttu-id="87e7f-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="87e7f-129">Property</span></span>|<span data-ttu-id="87e7f-130">型</span><span class="sxs-lookup"><span data-stu-id="87e7f-130">Type</span></span>|<span data-ttu-id="87e7f-131">説明</span><span class="sxs-lookup"><span data-stu-id="87e7f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="87e7f-132">classType</span><span class="sxs-lookup"><span data-stu-id="87e7f-132">classType</span></span>|[<span data-ttu-id="87e7f-133">grouppolicydefinitionclasstype</span><span class="sxs-lookup"><span data-stu-id="87e7f-133">groupPolicyDefinitionClassType</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionclasstype.md)|<span data-ttu-id="87e7f-134">ポリシーを適用できるグループの種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="87e7f-134">Identifies the type of groups the policy can be applied to.</span></span> <span data-ttu-id="87e7f-135">可能な値は `user`、`machine`、`both` です。</span><span class="sxs-lookup"><span data-stu-id="87e7f-135">Possible values are: `user`, `machine`, `both`.</span></span>|
|<span data-ttu-id="87e7f-136">displayName</span><span class="sxs-lookup"><span data-stu-id="87e7f-136">displayName</span></span>|<span data-ttu-id="87e7f-137">String</span><span class="sxs-lookup"><span data-stu-id="87e7f-137">String</span></span>|<span data-ttu-id="87e7f-138">ローカライズされたポリシー名。</span><span class="sxs-lookup"><span data-stu-id="87e7f-138">The localized policy name.</span></span>|
|<span data-ttu-id="87e7f-139">explainText</span><span class="sxs-lookup"><span data-stu-id="87e7f-139">explainText</span></span>|<span data-ttu-id="87e7f-140">String</span><span class="sxs-lookup"><span data-stu-id="87e7f-140">String</span></span>|<span data-ttu-id="87e7f-141">ポリシーに関連付けられたローカライズされた説明またはヘルプテキスト。</span><span class="sxs-lookup"><span data-stu-id="87e7f-141">The localized explanation or help text associated with the policy.</span></span> <span data-ttu-id="87e7f-142">既定値は empty です。</span><span class="sxs-lookup"><span data-stu-id="87e7f-142">The default value is empty.</span></span>|
|<span data-ttu-id="87e7f-143">categoryPath</span><span class="sxs-lookup"><span data-stu-id="87e7f-143">categoryPath</span></span>|<span data-ttu-id="87e7f-144">String</span><span class="sxs-lookup"><span data-stu-id="87e7f-144">String</span></span>|<span data-ttu-id="87e7f-145">ポリシーのローカライズされた完全なカテゴリのパス。</span><span class="sxs-lookup"><span data-stu-id="87e7f-145">The localized full category path for the policy.</span></span>|
|<span data-ttu-id="87e7f-146">supportedOn</span><span class="sxs-lookup"><span data-stu-id="87e7f-146">supportedOn</span></span>|<span data-ttu-id="87e7f-147">String</span><span class="sxs-lookup"><span data-stu-id="87e7f-147">String</span></span>|<span data-ttu-id="87e7f-148">ポリシーによって影響を受けるオペレーティングシステムまたはアプリケーションのバージョンを指定するために使用されるローカライズされた文字列。</span><span class="sxs-lookup"><span data-stu-id="87e7f-148">Localized string used to specify what operating system or application version is affected by the policy.</span></span>|
|<span data-ttu-id="87e7f-149">msrtcsip-policytype</span><span class="sxs-lookup"><span data-stu-id="87e7f-149">policyType</span></span>|[<span data-ttu-id="87e7f-150">groupPolicyType</span><span class="sxs-lookup"><span data-stu-id="87e7f-150">groupPolicyType</span></span>](../resources/intune-grouppolicy-grouppolicytype.md)|<span data-ttu-id="87e7f-151">グループポリシーの種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="87e7f-151">Specifies the type of group policy.</span></span> <span data-ttu-id="87e7f-152">使用可能な値は、`admxBacked`、`admxIngested` です。</span><span class="sxs-lookup"><span data-stu-id="87e7f-152">Possible values are: `admxBacked`, `admxIngested`.</span></span>|
|<span data-ttu-id="87e7f-153">id</span><span class="sxs-lookup"><span data-stu-id="87e7f-153">id</span></span>|<span data-ttu-id="87e7f-154">String</span><span class="sxs-lookup"><span data-stu-id="87e7f-154">String</span></span>|<span data-ttu-id="87e7f-155">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="87e7f-155">Key of the entity.</span></span>|
|<span data-ttu-id="87e7f-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="87e7f-156">lastModifiedDateTime</span></span>|<span data-ttu-id="87e7f-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="87e7f-157">DateTimeOffset</span></span>|<span data-ttu-id="87e7f-158">エンティティが最後に変更された日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="87e7f-158">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="87e7f-159">応答</span><span class="sxs-lookup"><span data-stu-id="87e7f-159">Response</span></span>
<span data-ttu-id="87e7f-160">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[grouppolicydefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="87e7f-160">If successful, this method returns a `200 OK` response code and an updated [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="87e7f-161">例</span><span class="sxs-lookup"><span data-stu-id="87e7f-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="87e7f-162">要求</span><span class="sxs-lookup"><span data-stu-id="87e7f-162">Request</span></span>
<span data-ttu-id="87e7f-163">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="87e7f-163">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyDefinitions/{groupPolicyDefinitionId}
Content-type: application/json
Content-length: 285

{
  "@odata.type": "#microsoft.graph.groupPolicyDefinition",
  "classType": "machine",
  "displayName": "Display Name value",
  "explainText": "Explain Text value",
  "categoryPath": "Category Path value",
  "supportedOn": "Supported On value",
  "policyType": "admxIngested"
}
```

### <a name="response"></a><span data-ttu-id="87e7f-164">応答</span><span class="sxs-lookup"><span data-stu-id="87e7f-164">Response</span></span>
<span data-ttu-id="87e7f-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="87e7f-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 398

{
  "@odata.type": "#microsoft.graph.groupPolicyDefinition",
  "classType": "machine",
  "displayName": "Display Name value",
  "explainText": "Explain Text value",
  "categoryPath": "Category Path value",
  "supportedOn": "Supported On value",
  "policyType": "admxIngested",
  "id": "f9607947-7947-f960-4779-60f9477960f9",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```




