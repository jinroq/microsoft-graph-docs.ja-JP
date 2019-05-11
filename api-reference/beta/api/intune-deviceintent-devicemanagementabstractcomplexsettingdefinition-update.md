---
title: DeviceManagementAbstractComplexSettingDefinition の更新
description: DeviceManagementAbstractComplexSettingDefinition オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7efaa164c8b86da08f190f651c7d49e000758bf1
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33916939"
---
# <a name="update-devicemanagementabstractcomplexsettingdefinition"></a><span data-ttu-id="cdbd1-103">DeviceManagementAbstractComplexSettingDefinition の更新</span><span class="sxs-lookup"><span data-stu-id="cdbd1-103">Update deviceManagementAbstractComplexSettingDefinition</span></span>

> <span data-ttu-id="cdbd1-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cdbd1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cdbd1-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="cdbd1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cdbd1-106">[DeviceManagementAbstractComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="cdbd1-106">Update the properties of a [deviceManagementAbstractComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cdbd1-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="cdbd1-107">Prerequisites</span></span>
<span data-ttu-id="cdbd1-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cdbd1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cdbd1-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="cdbd1-110">Permission type</span></span>|<span data-ttu-id="cdbd1-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="cdbd1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cdbd1-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="cdbd1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cdbd1-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cdbd1-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="cdbd1-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="cdbd1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cdbd1-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cdbd1-115">Not supported.</span></span>|
|<span data-ttu-id="cdbd1-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="cdbd1-116">Application</span></span>|<span data-ttu-id="cdbd1-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cdbd1-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cdbd1-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="cdbd1-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="cdbd1-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cdbd1-119">Request headers</span></span>
|<span data-ttu-id="cdbd1-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cdbd1-120">Header</span></span>|<span data-ttu-id="cdbd1-121">値</span><span class="sxs-lookup"><span data-stu-id="cdbd1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cdbd1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="cdbd1-122">Authorization</span></span>|<span data-ttu-id="cdbd1-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="cdbd1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cdbd1-124">承諾</span><span class="sxs-lookup"><span data-stu-id="cdbd1-124">Accept</span></span>|<span data-ttu-id="cdbd1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="cdbd1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cdbd1-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="cdbd1-126">Request body</span></span>
<span data-ttu-id="cdbd1-127">要求本文で、 [deviceManagementAbstractComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="cdbd1-127">In the request body, supply a JSON representation for the [deviceManagementAbstractComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md) object.</span></span>

<span data-ttu-id="cdbd1-128">次の表に、 [deviceManagementAbstractComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="cdbd1-128">The following table shows the properties that are required when you create the [deviceManagementAbstractComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md).</span></span>

|<span data-ttu-id="cdbd1-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cdbd1-129">Property</span></span>|<span data-ttu-id="cdbd1-130">型</span><span class="sxs-lookup"><span data-stu-id="cdbd1-130">Type</span></span>|<span data-ttu-id="cdbd1-131">説明</span><span class="sxs-lookup"><span data-stu-id="cdbd1-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cdbd1-132">id</span><span class="sxs-lookup"><span data-stu-id="cdbd1-132">id</span></span>|<span data-ttu-id="cdbd1-133">文字列</span><span class="sxs-lookup"><span data-stu-id="cdbd1-133">String</span></span>|<span data-ttu-id="cdbd1-134">[Devicemanagementsettingdefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)から継承された設定定義の ID</span><span class="sxs-lookup"><span data-stu-id="cdbd1-134">The ID of the setting definition Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="cdbd1-135">valueType</span><span class="sxs-lookup"><span data-stu-id="cdbd1-135">valueType</span></span>|[<span data-ttu-id="cdbd1-136">deviceManangementIntentValueType</span><span class="sxs-lookup"><span data-stu-id="cdbd1-136">deviceManangementIntentValueType</span></span>](../resources/intune-deviceintent-devicemanangementintentvaluetype.md)|<span data-ttu-id="cdbd1-137">[Devicemanagementsettingdefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)から継承された値のデータ型。</span><span class="sxs-lookup"><span data-stu-id="cdbd1-137">The data type of the value Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md).</span></span> <span data-ttu-id="cdbd1-138">使用可能な値: `integer`、`boolean`、`string`、`complex`、`collection`、`abstractComplex`。</span><span class="sxs-lookup"><span data-stu-id="cdbd1-138">Possible values are: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span></span>|
|<span data-ttu-id="cdbd1-139">displayName</span><span class="sxs-lookup"><span data-stu-id="cdbd1-139">displayName</span></span>|<span data-ttu-id="cdbd1-140">String</span><span class="sxs-lookup"><span data-stu-id="cdbd1-140">String</span></span>|<span data-ttu-id="cdbd1-141">[Devicemanagementsettingdefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)から継承された設定の表示名</span><span class="sxs-lookup"><span data-stu-id="cdbd1-141">The setting's display name Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="cdbd1-142">isTopLevel</span><span class="sxs-lookup"><span data-stu-id="cdbd1-142">isTopLevel</span></span>|<span data-ttu-id="cdbd1-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="cdbd1-143">Boolean</span></span>|<span data-ttu-id="cdbd1-144">設定が最上位レベルの場合は、 [Devicemanagementsettingdefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)から継承されたコレクションまたは複雑な設定でラップする必要がなく、構成することができます。</span><span class="sxs-lookup"><span data-stu-id="cdbd1-144">If the setting is top level, it can be configured without the need to be wrapped in a collection or complex setting Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="cdbd1-145">description</span><span class="sxs-lookup"><span data-stu-id="cdbd1-145">description</span></span>|<span data-ttu-id="cdbd1-146">String</span><span class="sxs-lookup"><span data-stu-id="cdbd1-146">String</span></span>|<span data-ttu-id="cdbd1-147">[Devicemanagementsettingdefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)から継承された設定の説明</span><span class="sxs-lookup"><span data-stu-id="cdbd1-147">The setting's description Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="cdbd1-148">Documentation Url</span><span class="sxs-lookup"><span data-stu-id="cdbd1-148">documentationUrl</span></span>|<span data-ttu-id="cdbd1-149">String</span><span class="sxs-lookup"><span data-stu-id="cdbd1-149">String</span></span>|<span data-ttu-id="cdbd1-150">[Devicemanagementsettingdefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)から継承されたドキュメントを設定するための Url</span><span class="sxs-lookup"><span data-stu-id="cdbd1-150">Url to setting documentation Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="cdbd1-151">keywords</span><span class="sxs-lookup"><span data-stu-id="cdbd1-151">keywords</span></span>|<span data-ttu-id="cdbd1-152">String collection</span><span class="sxs-lookup"><span data-stu-id="cdbd1-152">String collection</span></span>|<span data-ttu-id="cdbd1-153">[Devicemanagementsettingdefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)から継承した設定に関連付けられているキーワード</span><span class="sxs-lookup"><span data-stu-id="cdbd1-153">Keywords associated with the setting Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="cdbd1-154">式</span><span class="sxs-lookup"><span data-stu-id="cdbd1-154">constraints</span></span>|<span data-ttu-id="cdbd1-155">[Devicemanagementconstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="cdbd1-155">[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md) collection</span></span>|<span data-ttu-id="cdbd1-156">[Devicemanagementsettingdefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)から継承された設定値の制約のコレクション</span><span class="sxs-lookup"><span data-stu-id="cdbd1-156">Collection of constraints for the setting value Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="cdbd1-157">ヲ</span><span class="sxs-lookup"><span data-stu-id="cdbd1-157">dependencies</span></span>|<span data-ttu-id="cdbd1-158">[Devicemanagementsettingdependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="cdbd1-158">[deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md) collection</span></span>|<span data-ttu-id="cdbd1-159">[Devicemanagementsettingdefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)から継承された他の設定に対する依存関係のコレクション</span><span class="sxs-lookup"><span data-stu-id="cdbd1-159">Collection of dependencies on other settings Inherited from [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)</span></span>|
|<span data-ttu-id="cdbd1-160">メン</span><span class="sxs-lookup"><span data-stu-id="cdbd1-160">implementations</span></span>|<span data-ttu-id="cdbd1-161">String collection</span><span class="sxs-lookup"><span data-stu-id="cdbd1-161">String collection</span></span>|<span data-ttu-id="cdbd1-162">この抽象複合設定で可能なすべての実装の定義 Id のリスト</span><span class="sxs-lookup"><span data-stu-id="cdbd1-162">List of definition IDs for all possible implementations of this abstract complex setting</span></span>|



## <a name="response"></a><span data-ttu-id="cdbd1-163">応答</span><span class="sxs-lookup"><span data-stu-id="cdbd1-163">Response</span></span>
<span data-ttu-id="cdbd1-164">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[deviceManagementAbstractComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="cdbd1-164">If successful, this method returns a `200 OK` response code and an updated [deviceManagementAbstractComplexSettingDefinition](../resources/intune-deviceintent-devicemanagementabstractcomplexsettingdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cdbd1-165">例</span><span class="sxs-lookup"><span data-stu-id="cdbd1-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="cdbd1-166">要求</span><span class="sxs-lookup"><span data-stu-id="cdbd1-166">Request</span></span>
<span data-ttu-id="cdbd1-167">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="cdbd1-167">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/settingDefinitions/{deviceManagementSettingDefinitionId}
Content-type: application/json
Content-length: 802

{
  "@odata.type": "#microsoft.graph.deviceManagementAbstractComplexSettingDefinition",
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
  "implementations": [
    "Implementations value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="cdbd1-168">応答</span><span class="sxs-lookup"><span data-stu-id="cdbd1-168">Response</span></span>
<span data-ttu-id="cdbd1-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="cdbd1-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 851

{
  "@odata.type": "#microsoft.graph.deviceManagementAbstractComplexSettingDefinition",
  "id": "1b703309-3309-1b70-0933-701b0933701b",
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
  "implementations": [
    "Implementations value"
  ]
}
```




