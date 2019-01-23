---
title: GroupPolicyDefinition を更新します。
description: GroupPolicyDefinition オブジェクトのプロパティを更新します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: eeb3e32f1870eac8491989426081df2ae41e4d42
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430315"
---
# <a name="update-grouppolicydefinition"></a><span data-ttu-id="7c67a-103">GroupPolicyDefinition を更新します。</span><span class="sxs-lookup"><span data-stu-id="7c67a-103">Update groupPolicyDefinition</span></span>

> <span data-ttu-id="7c67a-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="7c67a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="7c67a-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7c67a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7c67a-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="7c67a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7c67a-107">[GroupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="7c67a-107">Update the properties of a [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7c67a-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="7c67a-108">Prerequisites</span></span>
<span data-ttu-id="7c67a-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7c67a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="7c67a-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7c67a-111">Permission type</span></span>|<span data-ttu-id="7c67a-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="7c67a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7c67a-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7c67a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7c67a-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c67a-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="7c67a-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7c67a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7c67a-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7c67a-116">Not supported.</span></span>|
|<span data-ttu-id="7c67a-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7c67a-117">Application</span></span>|<span data-ttu-id="7c67a-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7c67a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7c67a-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7c67a-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="7c67a-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7c67a-120">Request headers</span></span>
|<span data-ttu-id="7c67a-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7c67a-121">Header</span></span>|<span data-ttu-id="7c67a-122">値</span><span class="sxs-lookup"><span data-stu-id="7c67a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7c67a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7c67a-123">Authorization</span></span>|<span data-ttu-id="7c67a-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="7c67a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7c67a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7c67a-125">Accept</span></span>|<span data-ttu-id="7c67a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7c67a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7c67a-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="7c67a-127">Request body</span></span>
<span data-ttu-id="7c67a-128">要求の本文に[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="7c67a-128">In the request body, supply a JSON representation for the [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object.</span></span>

<span data-ttu-id="7c67a-129">[GroupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="7c67a-129">The following table shows the properties that are required when you create the [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md).</span></span>

|<span data-ttu-id="7c67a-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7c67a-130">Property</span></span>|<span data-ttu-id="7c67a-131">型</span><span class="sxs-lookup"><span data-stu-id="7c67a-131">Type</span></span>|<span data-ttu-id="7c67a-132">説明</span><span class="sxs-lookup"><span data-stu-id="7c67a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7c67a-133">classType</span><span class="sxs-lookup"><span data-stu-id="7c67a-133">classType</span></span>|[<span data-ttu-id="7c67a-134">groupPolicyDefinitionClassType</span><span class="sxs-lookup"><span data-stu-id="7c67a-134">groupPolicyDefinitionClassType</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionclasstype.md)|<span data-ttu-id="7c67a-135">ポリシーを適用できるグループの種類を識別します。</span><span class="sxs-lookup"><span data-stu-id="7c67a-135">Identifies the type of groups the policy can be applied to.</span></span> <span data-ttu-id="7c67a-136">可能な値は、`user`、`machine`、`both` です。</span><span class="sxs-lookup"><span data-stu-id="7c67a-136">Possible values are: `user`, `machine`, `both`.</span></span>|
|<span data-ttu-id="7c67a-137">displayName</span><span class="sxs-lookup"><span data-stu-id="7c67a-137">displayName</span></span>|<span data-ttu-id="7c67a-138">String</span><span class="sxs-lookup"><span data-stu-id="7c67a-138">String</span></span>|<span data-ttu-id="7c67a-139">ローカライズされたポリシーの名前です。</span><span class="sxs-lookup"><span data-stu-id="7c67a-139">The localized policy name.</span></span>|
|<span data-ttu-id="7c67a-140">説明</span><span class="sxs-lookup"><span data-stu-id="7c67a-140">explainText</span></span>|<span data-ttu-id="7c67a-141">String</span><span class="sxs-lookup"><span data-stu-id="7c67a-141">String</span></span>|<span data-ttu-id="7c67a-142">ローカライズされた説明またはヘルプ テキスト、ポリシーに関連付けられています。</span><span class="sxs-lookup"><span data-stu-id="7c67a-142">The localized explanation or help text associated with the policy.</span></span> <span data-ttu-id="7c67a-143">既定値は空です。</span><span class="sxs-lookup"><span data-stu-id="7c67a-143">The default value is empty.</span></span>|
|<span data-ttu-id="7c67a-144">categoryPath</span><span class="sxs-lookup"><span data-stu-id="7c67a-144">categoryPath</span></span>|<span data-ttu-id="7c67a-145">String</span><span class="sxs-lookup"><span data-stu-id="7c67a-145">String</span></span>|<span data-ttu-id="7c67a-146">ポリシーのすべてのローカライズされたカテゴリのパスです。</span><span class="sxs-lookup"><span data-stu-id="7c67a-146">The localized full category path for the policy.</span></span>|
|<span data-ttu-id="7c67a-147">supportedOn</span><span class="sxs-lookup"><span data-stu-id="7c67a-147">supportedOn</span></span>|<span data-ttu-id="7c67a-148">String</span><span class="sxs-lookup"><span data-stu-id="7c67a-148">String</span></span>|<span data-ttu-id="7c67a-149">どのようなオペレーティング システムまたはアプリケーションのバージョンを指定するために使用するローカライズされた文字列は、ポリシーの影響を受けます。</span><span class="sxs-lookup"><span data-stu-id="7c67a-149">Localized string used to specify what operating system or application version is affected by the policy.</span></span>|
|<span data-ttu-id="7c67a-150">policyType</span><span class="sxs-lookup"><span data-stu-id="7c67a-150">policyType</span></span>|[<span data-ttu-id="7c67a-151">groupPolicyType</span><span class="sxs-lookup"><span data-stu-id="7c67a-151">groupPolicyType</span></span>](../resources/intune-grouppolicy-grouppolicytype.md)|<span data-ttu-id="7c67a-152">グループ ポリシーの種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="7c67a-152">Specifies the type of group policy.</span></span> <span data-ttu-id="7c67a-153">使用可能な値は、`admxBacked`、`admxIngested` です。</span><span class="sxs-lookup"><span data-stu-id="7c67a-153">Possible values are: `admxBacked`, `admxIngested`.</span></span>|
|<span data-ttu-id="7c67a-154">id</span><span class="sxs-lookup"><span data-stu-id="7c67a-154">id</span></span>|<span data-ttu-id="7c67a-155">String</span><span class="sxs-lookup"><span data-stu-id="7c67a-155">String</span></span>|<span data-ttu-id="7c67a-156">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="7c67a-156">Key of the entity.</span></span>|
|<span data-ttu-id="7c67a-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7c67a-157">lastModifiedDateTime</span></span>|<span data-ttu-id="7c67a-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7c67a-158">DateTimeOffset</span></span>|<span data-ttu-id="7c67a-159">日付と時刻、エンティティが最後に修正されました。</span><span class="sxs-lookup"><span data-stu-id="7c67a-159">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="7c67a-160">応答</span><span class="sxs-lookup"><span data-stu-id="7c67a-160">Response</span></span>
<span data-ttu-id="7c67a-161">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="7c67a-161">If successful, this method returns a `200 OK` response code and an updated [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7c67a-162">例</span><span class="sxs-lookup"><span data-stu-id="7c67a-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="7c67a-163">要求</span><span class="sxs-lookup"><span data-stu-id="7c67a-163">Request</span></span>
<span data-ttu-id="7c67a-164">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7c67a-164">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7c67a-165">応答</span><span class="sxs-lookup"><span data-stu-id="7c67a-165">Response</span></span>
<span data-ttu-id="7c67a-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7c67a-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




