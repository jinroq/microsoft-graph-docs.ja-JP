---
title: devicemanagementcollectionsettingdefinition の作成
description: 新しい devicemanagementcollectionsettingdefinition オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2367ebc5206ee64fe3b2fe2fd266bef26fe08f6f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32509857"
---
# <a name="create-devicemanagementcollectionsettingdefinition"></a><span data-ttu-id="cac1d-103">devicemanagementcollectionsettingdefinition の作成</span><span class="sxs-lookup"><span data-stu-id="cac1d-103">Create deviceManagementCollectionSettingDefinition</span></span>

> <span data-ttu-id="cac1d-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cac1d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cac1d-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="cac1d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cac1d-106">新しい[devicemanagementcollectionsettingdefinition](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="cac1d-106">Create a new [deviceManagementCollectionSettingDefinition](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cac1d-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="cac1d-107">Prerequisites</span></span>
<span data-ttu-id="cac1d-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cac1d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cac1d-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="cac1d-110">Permission type</span></span>|<span data-ttu-id="cac1d-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="cac1d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cac1d-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="cac1d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cac1d-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cac1d-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="cac1d-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="cac1d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cac1d-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cac1d-115">Not supported.</span></span>|
|<span data-ttu-id="cac1d-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="cac1d-116">Application</span></span>|<span data-ttu-id="cac1d-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cac1d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cac1d-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="cac1d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/settingDefinitions
POST /deviceManagement/categories/{deviceManagementSettingCategoryId}/settingDefinitions
POST /deviceManagement/intents/{deviceManagementIntentId}/categories/{deviceManagementIntentSettingCategoryId}/settingDefinitions
POST /deviceManagement/templates/{deviceManagementTemplateId}/categories/{deviceManagementTemplateSettingCategoryId}/settingDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="cac1d-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cac1d-119">Request headers</span></span>
|<span data-ttu-id="cac1d-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cac1d-120">Header</span></span>|<span data-ttu-id="cac1d-121">値</span><span class="sxs-lookup"><span data-stu-id="cac1d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cac1d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="cac1d-122">Authorization</span></span>|<span data-ttu-id="cac1d-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="cac1d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cac1d-124">承諾</span><span class="sxs-lookup"><span data-stu-id="cac1d-124">Accept</span></span>|<span data-ttu-id="cac1d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="cac1d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cac1d-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="cac1d-126">Request body</span></span>
<span data-ttu-id="cac1d-127">要求本文で、devicemanagementcollectionsettingdefinition オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="cac1d-127">In the request body, supply a JSON representation for the deviceManagementCollectionSettingDefinition object.</span></span>

<span data-ttu-id="cac1d-128">次の表に、devicemanagementcollectionsettingdefinition の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="cac1d-128">The following table shows the properties that are required when you create the deviceManagementCollectionSettingDefinition.</span></span>

|<span data-ttu-id="cac1d-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cac1d-129">Property</span></span>|<span data-ttu-id="cac1d-130">型</span><span class="sxs-lookup"><span data-stu-id="cac1d-130">Type</span></span>|<span data-ttu-id="cac1d-131">説明</span><span class="sxs-lookup"><span data-stu-id="cac1d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cac1d-132">id</span><span class="sxs-lookup"><span data-stu-id="cac1d-132">id</span></span>|<span data-ttu-id="cac1d-133">String</span><span class="sxs-lookup"><span data-stu-id="cac1d-133">String</span></span>|<span data-ttu-id="cac1d-134">[devicemanagementsettingdefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)から継承された設定定義の ID</span><span class="sxs-lookup"><span data-stu-id="cac1d-134">The ID of the setting definition Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="cac1d-135">valueType</span><span class="sxs-lookup"><span data-stu-id="cac1d-135">valueType</span></span>|[<span data-ttu-id="cac1d-136">deviceManangementIntentValueType</span><span class="sxs-lookup"><span data-stu-id="cac1d-136">deviceManangementIntentValueType</span></span>](../resources/intune-deviceintent-devicemanangementintentvaluetype.md)|<span data-ttu-id="cac1d-137">[devicemanagementsettingdefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)から継承された値のデータ型。</span><span class="sxs-lookup"><span data-stu-id="cac1d-137">The data type of the value Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md).</span></span> <span data-ttu-id="cac1d-138">可能な値は `integer`、`boolean`、`string`、`complex`、`collection`、`abstractComplex` です。</span><span class="sxs-lookup"><span data-stu-id="cac1d-138">Possible values are: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span></span>|
|<span data-ttu-id="cac1d-139">displayName</span><span class="sxs-lookup"><span data-stu-id="cac1d-139">displayName</span></span>|<span data-ttu-id="cac1d-140">String</span><span class="sxs-lookup"><span data-stu-id="cac1d-140">String</span></span>|<span data-ttu-id="cac1d-141">[devicemanagementsettingdefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)から継承された設定の表示名</span><span class="sxs-lookup"><span data-stu-id="cac1d-141">The setting's display name Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="cac1d-142">isTopLevel</span><span class="sxs-lookup"><span data-stu-id="cac1d-142">isTopLevel</span></span>|<span data-ttu-id="cac1d-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="cac1d-143">Boolean</span></span>|<span data-ttu-id="cac1d-144">設定が最上位レベルの場合は、 [devicemanagementsettingdefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)から継承されたコレクションまたは複雑な設定でラップする必要がなく、構成することができます。</span><span class="sxs-lookup"><span data-stu-id="cac1d-144">If the setting is top level, it can be configured without the need to be wrapped in a collection or complex setting Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="cac1d-145">説明</span><span class="sxs-lookup"><span data-stu-id="cac1d-145">description</span></span>|<span data-ttu-id="cac1d-146">String</span><span class="sxs-lookup"><span data-stu-id="cac1d-146">String</span></span>|<span data-ttu-id="cac1d-147">[devicemanagementsettingdefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)から継承された設定の説明</span><span class="sxs-lookup"><span data-stu-id="cac1d-147">The setting's description Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="cac1d-148">documentation url</span><span class="sxs-lookup"><span data-stu-id="cac1d-148">documentationUrl</span></span>|<span data-ttu-id="cac1d-149">String</span><span class="sxs-lookup"><span data-stu-id="cac1d-149">String</span></span>|<span data-ttu-id="cac1d-150">[devicemanagementsettingdefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)から継承されたドキュメントを設定するための Url</span><span class="sxs-lookup"><span data-stu-id="cac1d-150">Url to setting documentation Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="cac1d-151">keywords</span><span class="sxs-lookup"><span data-stu-id="cac1d-151">keywords</span></span>|<span data-ttu-id="cac1d-152">String collection</span><span class="sxs-lookup"><span data-stu-id="cac1d-152">String collection</span></span>|<span data-ttu-id="cac1d-153">[devicemanagementsettingdefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)から継承した設定に関連付けられているキーワード</span><span class="sxs-lookup"><span data-stu-id="cac1d-153">Keywords associated with the setting Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="cac1d-154">式</span><span class="sxs-lookup"><span data-stu-id="cac1d-154">constraints</span></span>|<span data-ttu-id="cac1d-155">[devicemanagementconstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="cac1d-155">[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md) collection</span></span>|<span data-ttu-id="cac1d-156">[devicemanagementsettingdefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)から継承された設定値の制約のコレクション</span><span class="sxs-lookup"><span data-stu-id="cac1d-156">Collection of constraints for the setting value Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="cac1d-157">ヲ</span><span class="sxs-lookup"><span data-stu-id="cac1d-157">dependencies</span></span>|<span data-ttu-id="cac1d-158">[devicemanagementsettingdependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="cac1d-158">[deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md) collection</span></span>|<span data-ttu-id="cac1d-159">[devicemanagementsettingdefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)から継承された他の設定に対する依存関係のコレクション</span><span class="sxs-lookup"><span data-stu-id="cac1d-159">Collection of dependencies on other settings Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="cac1d-160">elementDefinitionId</span><span class="sxs-lookup"><span data-stu-id="cac1d-160">elementDefinitionId</span></span>|<span data-ttu-id="cac1d-161">String</span><span class="sxs-lookup"><span data-stu-id="cac1d-161">String</span></span>|<span data-ttu-id="cac1d-162">コレクションの各要素がどのようなものかを示す設定定義 ID。</span><span class="sxs-lookup"><span data-stu-id="cac1d-162">The Setting Definition ID that describes what each element of the collection looks like</span></span>|



## <a name="response"></a><span data-ttu-id="cac1d-163">応答</span><span class="sxs-lookup"><span data-stu-id="cac1d-163">Response</span></span>
<span data-ttu-id="cac1d-164">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[devicemanagementcollectionsettingdefinition](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="cac1d-164">If successful, this method returns a `201 Created` response code and a [deviceManagementCollectionSettingDefinition](../resources/intune-deviceintent-devicemanagementcollectionsettingdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cac1d-165">例</span><span class="sxs-lookup"><span data-stu-id="cac1d-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="cac1d-166">要求</span><span class="sxs-lookup"><span data-stu-id="cac1d-166">Request</span></span>
<span data-ttu-id="cac1d-167">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="cac1d-167">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/settingDefinitions
Content-type: application/json
Content-length: 795

{
  "@odata.type": "#microsoft.graph.deviceManagementCollectionSettingDefinition",
  "valueType": "boolean",
  "displayName": "Display Name value",
  "isTopLevel": true,
  "description": "Description value",
  "documentationUrl": "https://example.com/documentationUrl/",
  "keywords": [
    "Keywords value"
  ],
  "constraints": [
    {
      "@odata.type": "microsoft.graph.deviceManagementSettingXmlConstraint"
    }
  ],
  "dependencies": [
    {
      "@odata.type": "microsoft.graph.deviceManagementSettingDependency",
      "definitionId": "Definition Id value",
      "constraints": [
        {
          "@odata.type": "microsoft.graph.deviceManagementSettingXmlConstraint"
        }
      ]
    }
  ],
  "elementDefinitionId": "Element Definition Id value"
}
```

### <a name="response"></a><span data-ttu-id="cac1d-168">応答</span><span class="sxs-lookup"><span data-stu-id="cac1d-168">Response</span></span>
<span data-ttu-id="cac1d-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="cac1d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 844

{
  "@odata.type": "#microsoft.graph.deviceManagementCollectionSettingDefinition",
  "id": "0419c4a7-c4a7-0419-a7c4-1904a7c41904",
  "valueType": "boolean",
  "displayName": "Display Name value",
  "isTopLevel": true,
  "description": "Description value",
  "documentationUrl": "https://example.com/documentationUrl/",
  "keywords": [
    "Keywords value"
  ],
  "constraints": [
    {
      "@odata.type": "microsoft.graph.deviceManagementSettingXmlConstraint"
    }
  ],
  "dependencies": [
    {
      "@odata.type": "microsoft.graph.deviceManagementSettingDependency",
      "definitionId": "Definition Id value",
      "constraints": [
        {
          "@odata.type": "microsoft.graph.deviceManagementSettingXmlConstraint"
        }
      ]
    }
  ],
  "elementDefinitionId": "Element Definition Id value"
}
```





