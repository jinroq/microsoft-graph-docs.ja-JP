---
title: DeviceManagementComplexSettingDefinition の更新
description: DeviceManagementComplexSettingDefinition オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 76b13443806bf6a30fa2fd6f2e6d809dc19de2fa
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34960700"
---
# <a name="update-devicemanagementcomplexsettingdefinition"></a><span data-ttu-id="dff7a-103">DeviceManagementComplexSettingDefinition の更新</span><span class="sxs-lookup"><span data-stu-id="dff7a-103">Update deviceManagementComplexSettingDefinition</span></span>

> <span data-ttu-id="dff7a-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dff7a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dff7a-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="dff7a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dff7a-106">[Devicemanagementcomplexsettingdefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="dff7a-106">Update the properties of a [deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dff7a-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="dff7a-107">Prerequisites</span></span>
<span data-ttu-id="dff7a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="dff7a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dff7a-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="dff7a-110">Permission type</span></span>|<span data-ttu-id="dff7a-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="dff7a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dff7a-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="dff7a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="dff7a-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dff7a-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="dff7a-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="dff7a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dff7a-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dff7a-115">Not supported.</span></span>|
|<span data-ttu-id="dff7a-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="dff7a-116">Application</span></span>|<span data-ttu-id="dff7a-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dff7a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dff7a-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="dff7a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/settingDefinitions/{deviceManagementSettingDefinitionId}
PATCH /deviceManagement/categories/{deviceManagementSettingCategoryId}/settingDefinitions/{deviceManagementSettingDefinitionId}
PATCH /deviceManagement/intents/{deviceManagementIntentId}/categories/{deviceManagementIntentSettingCategoryId}/settingDefinitions/{deviceManagementSettingDefinitionId}
PATCH /deviceManagement/templates/{deviceManagementTemplateId}/categories/{deviceManagementTemplateSettingCategoryId}/settingDefinitions/{deviceManagementSettingDefinitionId}
```

## <a name="request-headers"></a><span data-ttu-id="dff7a-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="dff7a-119">Request headers</span></span>
|<span data-ttu-id="dff7a-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="dff7a-120">Header</span></span>|<span data-ttu-id="dff7a-121">値</span><span class="sxs-lookup"><span data-stu-id="dff7a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dff7a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="dff7a-122">Authorization</span></span>|<span data-ttu-id="dff7a-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="dff7a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dff7a-124">承諾</span><span class="sxs-lookup"><span data-stu-id="dff7a-124">Accept</span></span>|<span data-ttu-id="dff7a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="dff7a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dff7a-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="dff7a-126">Request body</span></span>
<span data-ttu-id="dff7a-127">要求本文で、 [Devicemanagementcomplexsettingdefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="dff7a-127">In the request body, supply a JSON representation for the [deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) object.</span></span>

<span data-ttu-id="dff7a-128">次の表に、 [Devicemanagementcomplexsettingdefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="dff7a-128">The following table shows the properties that are required when you create the [deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md).</span></span>

|<span data-ttu-id="dff7a-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dff7a-129">Property</span></span>|<span data-ttu-id="dff7a-130">型</span><span class="sxs-lookup"><span data-stu-id="dff7a-130">Type</span></span>|<span data-ttu-id="dff7a-131">説明</span><span class="sxs-lookup"><span data-stu-id="dff7a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dff7a-132">id</span><span class="sxs-lookup"><span data-stu-id="dff7a-132">id</span></span>|<span data-ttu-id="dff7a-133">文字列</span><span class="sxs-lookup"><span data-stu-id="dff7a-133">String</span></span>|<span data-ttu-id="dff7a-134">[Devicemanagementsettingdefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)から継承された設定定義の ID</span><span class="sxs-lookup"><span data-stu-id="dff7a-134">The ID of the setting definition Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="dff7a-135">valueType</span><span class="sxs-lookup"><span data-stu-id="dff7a-135">valueType</span></span>|[<span data-ttu-id="dff7a-136">deviceManangementIntentValueType</span><span class="sxs-lookup"><span data-stu-id="dff7a-136">deviceManangementIntentValueType</span></span>](../resources/intune-deviceintent-devicemanangementintentvaluetype.md)|<span data-ttu-id="dff7a-137">[Devicemanagementsettingdefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)から継承された値のデータ型。</span><span class="sxs-lookup"><span data-stu-id="dff7a-137">The data type of the value Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md).</span></span> <span data-ttu-id="dff7a-138">使用可能な値: `integer`、`boolean`、`string`、`complex`、`collection`、`abstractComplex`。</span><span class="sxs-lookup"><span data-stu-id="dff7a-138">Possible values are: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span></span>|
|<span data-ttu-id="dff7a-139">displayName</span><span class="sxs-lookup"><span data-stu-id="dff7a-139">displayName</span></span>|<span data-ttu-id="dff7a-140">String</span><span class="sxs-lookup"><span data-stu-id="dff7a-140">String</span></span>|<span data-ttu-id="dff7a-141">[Devicemanagementsettingdefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)から継承された設定の表示名</span><span class="sxs-lookup"><span data-stu-id="dff7a-141">The setting's display name Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="dff7a-142">isTopLevel</span><span class="sxs-lookup"><span data-stu-id="dff7a-142">isTopLevel</span></span>|<span data-ttu-id="dff7a-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="dff7a-143">Boolean</span></span>|<span data-ttu-id="dff7a-144">設定が最上位レベルの場合は、 [Devicemanagementsettingdefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)から継承されたコレクションまたは複雑な設定でラップする必要がなく、構成することができます。</span><span class="sxs-lookup"><span data-stu-id="dff7a-144">If the setting is top level, it can be configured without the need to be wrapped in a collection or complex setting Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="dff7a-145">description</span><span class="sxs-lookup"><span data-stu-id="dff7a-145">description</span></span>|<span data-ttu-id="dff7a-146">String</span><span class="sxs-lookup"><span data-stu-id="dff7a-146">String</span></span>|<span data-ttu-id="dff7a-147">[Devicemanagementsettingdefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)から継承された設定の説明</span><span class="sxs-lookup"><span data-stu-id="dff7a-147">The setting's description Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="dff7a-148">Documentation Url</span><span class="sxs-lookup"><span data-stu-id="dff7a-148">documentationUrl</span></span>|<span data-ttu-id="dff7a-149">String</span><span class="sxs-lookup"><span data-stu-id="dff7a-149">String</span></span>|<span data-ttu-id="dff7a-150">[Devicemanagementsettingdefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)から継承されたドキュメントを設定するための Url</span><span class="sxs-lookup"><span data-stu-id="dff7a-150">Url to setting documentation Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="dff7a-151">keywords</span><span class="sxs-lookup"><span data-stu-id="dff7a-151">keywords</span></span>|<span data-ttu-id="dff7a-152">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="dff7a-152">String collection</span></span>|<span data-ttu-id="dff7a-153">[Devicemanagementsettingdefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)から継承した設定に関連付けられているキーワード</span><span class="sxs-lookup"><span data-stu-id="dff7a-153">Keywords associated with the setting Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="dff7a-154">式</span><span class="sxs-lookup"><span data-stu-id="dff7a-154">constraints</span></span>|<span data-ttu-id="dff7a-155">[Devicemanagementconstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="dff7a-155">[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md) collection</span></span>|<span data-ttu-id="dff7a-156">[Devicemanagementsettingdefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)から継承された設定値の制約のコレクション</span><span class="sxs-lookup"><span data-stu-id="dff7a-156">Collection of constraints for the setting value Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="dff7a-157">ヲ</span><span class="sxs-lookup"><span data-stu-id="dff7a-157">dependencies</span></span>|<span data-ttu-id="dff7a-158">[Devicemanagementsettingdependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="dff7a-158">[deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md) collection</span></span>|<span data-ttu-id="dff7a-159">[Devicemanagementsettingdefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)から継承された他の設定に対する依存関係のコレクション</span><span class="sxs-lookup"><span data-stu-id="dff7a-159">Collection of dependencies on other settings Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="dff7a-160">propertyDefinitionIds</span><span class="sxs-lookup"><span data-stu-id="dff7a-160">propertyDefinitionIds</span></span>|<span data-ttu-id="dff7a-161">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="dff7a-161">String collection</span></span>|<span data-ttu-id="dff7a-162">複合設定の各プロパティの定義</span><span class="sxs-lookup"><span data-stu-id="dff7a-162">The definitions of each property of the complex setting</span></span>|



## <a name="response"></a><span data-ttu-id="dff7a-163">応答</span><span class="sxs-lookup"><span data-stu-id="dff7a-163">Response</span></span>
<span data-ttu-id="dff7a-164">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[Devicemanagementcomplexsettingdefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="dff7a-164">If successful, this method returns a `200 OK` response code and an updated [deviceManagementComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementcomplexsettingdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dff7a-165">例</span><span class="sxs-lookup"><span data-stu-id="dff7a-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="dff7a-166">要求</span><span class="sxs-lookup"><span data-stu-id="dff7a-166">Request</span></span>
<span data-ttu-id="dff7a-167">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="dff7a-167">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/settingDefinitions/{deviceManagementSettingDefinitionId}
Content-type: application/json
Content-length: 808

{
  "@odata.type": "#microsoft.graph.deviceManagementComplexSettingDefinition",
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
  "propertyDefinitionIds": [
    "Property Definition Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="dff7a-168">応答</span><span class="sxs-lookup"><span data-stu-id="dff7a-168">Response</span></span>
<span data-ttu-id="dff7a-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="dff7a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 857

{
  "@odata.type": "#microsoft.graph.deviceManagementComplexSettingDefinition",
  "id": "823ca4f9-a4f9-823c-f9a4-3c82f9a43c82",
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
  "propertyDefinitionIds": [
    "Property Definition Ids value"
  ]
}
```





