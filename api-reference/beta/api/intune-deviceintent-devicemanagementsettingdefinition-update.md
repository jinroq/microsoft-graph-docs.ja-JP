---
title: devicemanagementsettingdefinition の更新
description: devicemanagementsettingdefinition オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f11167524956ff3eddc9a5508fb30fdd81e2aa73
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31801457"
---
# <a name="update-devicemanagementsettingdefinition"></a><span data-ttu-id="f3a3e-103">devicemanagementsettingdefinition の更新</span><span class="sxs-lookup"><span data-stu-id="f3a3e-103">Update deviceManagementSettingDefinition</span></span>

> <span data-ttu-id="f3a3e-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f3a3e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f3a3e-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f3a3e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f3a3e-106">[devicemanagementsettingdefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="f3a3e-106">Update the properties of a [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f3a3e-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="f3a3e-107">Prerequisites</span></span>
<span data-ttu-id="f3a3e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f3a3e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f3a3e-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f3a3e-110">Permission type</span></span>|<span data-ttu-id="f3a3e-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="f3a3e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f3a3e-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f3a3e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f3a3e-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3a3e-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f3a3e-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f3a3e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f3a3e-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f3a3e-115">Not supported.</span></span>|
|<span data-ttu-id="f3a3e-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f3a3e-116">Application</span></span>|<span data-ttu-id="f3a3e-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f3a3e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f3a3e-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f3a3e-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="f3a3e-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f3a3e-119">Request headers</span></span>
|<span data-ttu-id="f3a3e-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f3a3e-120">Header</span></span>|<span data-ttu-id="f3a3e-121">値</span><span class="sxs-lookup"><span data-stu-id="f3a3e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f3a3e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f3a3e-122">Authorization</span></span>|<span data-ttu-id="f3a3e-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="f3a3e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f3a3e-124">承諾</span><span class="sxs-lookup"><span data-stu-id="f3a3e-124">Accept</span></span>|<span data-ttu-id="f3a3e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f3a3e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f3a3e-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="f3a3e-126">Request body</span></span>
<span data-ttu-id="f3a3e-127">要求本文で、 [devicemanagementsettingdefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="f3a3e-127">In the request body, supply a JSON representation for the [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) object.</span></span>

<span data-ttu-id="f3a3e-128">次の表に、 [devicemanagementsettingdefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="f3a3e-128">The following table shows the properties that are required when you create the [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md).</span></span>

|<span data-ttu-id="f3a3e-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f3a3e-129">Property</span></span>|<span data-ttu-id="f3a3e-130">型</span><span class="sxs-lookup"><span data-stu-id="f3a3e-130">Type</span></span>|<span data-ttu-id="f3a3e-131">説明</span><span class="sxs-lookup"><span data-stu-id="f3a3e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f3a3e-132">id</span><span class="sxs-lookup"><span data-stu-id="f3a3e-132">id</span></span>|<span data-ttu-id="f3a3e-133">文字列</span><span class="sxs-lookup"><span data-stu-id="f3a3e-133">String</span></span>|<span data-ttu-id="f3a3e-134">設定定義の ID</span><span class="sxs-lookup"><span data-stu-id="f3a3e-134">The ID of the setting definition</span></span>|
|<span data-ttu-id="f3a3e-135">valueType</span><span class="sxs-lookup"><span data-stu-id="f3a3e-135">valueType</span></span>|[<span data-ttu-id="f3a3e-136">deviceManangementIntentValueType</span><span class="sxs-lookup"><span data-stu-id="f3a3e-136">deviceManangementIntentValueType</span></span>](../resources/intune-deviceintent-devicemanangementintentvaluetype.md)|<span data-ttu-id="f3a3e-137">値のデータ型。</span><span class="sxs-lookup"><span data-stu-id="f3a3e-137">The data type of the value.</span></span> <span data-ttu-id="f3a3e-138">可能な値は `integer`、`boolean`、`string`、`complex`、`collection`、`abstractComplex` です。</span><span class="sxs-lookup"><span data-stu-id="f3a3e-138">Possible values are: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span></span>|
|<span data-ttu-id="f3a3e-139">displayName</span><span class="sxs-lookup"><span data-stu-id="f3a3e-139">displayName</span></span>|<span data-ttu-id="f3a3e-140">String</span><span class="sxs-lookup"><span data-stu-id="f3a3e-140">String</span></span>|<span data-ttu-id="f3a3e-141">設定の表示名</span><span class="sxs-lookup"><span data-stu-id="f3a3e-141">The setting's display name</span></span>|
|<span data-ttu-id="f3a3e-142">isTopLevel</span><span class="sxs-lookup"><span data-stu-id="f3a3e-142">isTopLevel</span></span>|<span data-ttu-id="f3a3e-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3a3e-143">Boolean</span></span>|<span data-ttu-id="f3a3e-144">設定が最上位レベルの場合は、コレクションまたは複雑な設定でラップする必要がなく構成できます。</span><span class="sxs-lookup"><span data-stu-id="f3a3e-144">If the setting is top level, it can be configured without the need to be wrapped in a collection or complex setting</span></span>|
|<span data-ttu-id="f3a3e-145">説明</span><span class="sxs-lookup"><span data-stu-id="f3a3e-145">description</span></span>|<span data-ttu-id="f3a3e-146">String</span><span class="sxs-lookup"><span data-stu-id="f3a3e-146">String</span></span>|<span data-ttu-id="f3a3e-147">設定の説明</span><span class="sxs-lookup"><span data-stu-id="f3a3e-147">The setting's description</span></span>|
|<span data-ttu-id="f3a3e-148">documentation url</span><span class="sxs-lookup"><span data-stu-id="f3a3e-148">documentationUrl</span></span>|<span data-ttu-id="f3a3e-149">文字列</span><span class="sxs-lookup"><span data-stu-id="f3a3e-149">String</span></span>|<span data-ttu-id="f3a3e-150">ドキュメントを設定するための Url</span><span class="sxs-lookup"><span data-stu-id="f3a3e-150">Url to setting documentation</span></span>|
|<span data-ttu-id="f3a3e-151">keywords</span><span class="sxs-lookup"><span data-stu-id="f3a3e-151">keywords</span></span>|<span data-ttu-id="f3a3e-152">String コレクション</span><span class="sxs-lookup"><span data-stu-id="f3a3e-152">String collection</span></span>|<span data-ttu-id="f3a3e-153">設定に関連付けられているキーワード</span><span class="sxs-lookup"><span data-stu-id="f3a3e-153">Keywords associated with the setting</span></span>|
|<span data-ttu-id="f3a3e-154">式</span><span class="sxs-lookup"><span data-stu-id="f3a3e-154">constraints</span></span>|<span data-ttu-id="f3a3e-155">[devicemanagementconstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="f3a3e-155">[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md) collection</span></span>|<span data-ttu-id="f3a3e-156">設定値の制約のコレクション</span><span class="sxs-lookup"><span data-stu-id="f3a3e-156">Collection of constraints for the setting value</span></span>|
|<span data-ttu-id="f3a3e-157">ヲ</span><span class="sxs-lookup"><span data-stu-id="f3a3e-157">dependencies</span></span>|<span data-ttu-id="f3a3e-158">[devicemanagementsettingdependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="f3a3e-158">[deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md) collection</span></span>|<span data-ttu-id="f3a3e-159">他の設定に対する依存関係のコレクション</span><span class="sxs-lookup"><span data-stu-id="f3a3e-159">Collection of dependencies on other settings</span></span>|



## <a name="response"></a><span data-ttu-id="f3a3e-160">応答</span><span class="sxs-lookup"><span data-stu-id="f3a3e-160">Response</span></span>
<span data-ttu-id="f3a3e-161">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[devicemanagementsettingdefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f3a3e-161">If successful, this method returns a `200 OK` response code and an updated [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f3a3e-162">例</span><span class="sxs-lookup"><span data-stu-id="f3a3e-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="f3a3e-163">要求</span><span class="sxs-lookup"><span data-stu-id="f3a3e-163">Request</span></span>
<span data-ttu-id="f3a3e-164">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f3a3e-164">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/settingDefinitions/{deviceManagementSettingDefinitionId}
Content-type: application/json
Content-length: 728

{
  "@odata.type": "#microsoft.graph.deviceManagementSettingDefinition",
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
  ]
}
```

### <a name="response"></a><span data-ttu-id="f3a3e-165">応答</span><span class="sxs-lookup"><span data-stu-id="f3a3e-165">Response</span></span>
<span data-ttu-id="f3a3e-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f3a3e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 777

{
  "@odata.type": "#microsoft.graph.deviceManagementSettingDefinition",
  "id": "4ec3093d-093d-4ec3-3d09-c34e3d09c34e",
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
  ]
}
```





