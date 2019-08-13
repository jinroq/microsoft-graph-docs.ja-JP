---
title: DeviceManagementSettingDefinition の作成
description: 新しい deviceManagementSettingDefinition オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f2c46fa55bb77fd1d201a99c3b1c321d677d9727
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36343309"
---
# <a name="create-devicemanagementsettingdefinition"></a><span data-ttu-id="2fd9c-103">DeviceManagementSettingDefinition の作成</span><span class="sxs-lookup"><span data-stu-id="2fd9c-103">Create deviceManagementSettingDefinition</span></span>

> <span data-ttu-id="2fd9c-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2fd9c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2fd9c-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="2fd9c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2fd9c-106">新しい[Devicemanagementsettingdefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="2fd9c-106">Create a new [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2fd9c-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="2fd9c-107">Prerequisites</span></span>
<span data-ttu-id="2fd9c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2fd9c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2fd9c-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2fd9c-110">Permission type</span></span>|<span data-ttu-id="2fd9c-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="2fd9c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2fd9c-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2fd9c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2fd9c-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2fd9c-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2fd9c-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2fd9c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2fd9c-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2fd9c-115">Not supported.</span></span>|
|<span data-ttu-id="2fd9c-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2fd9c-116">Application</span></span>|<span data-ttu-id="2fd9c-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2fd9c-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2fd9c-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2fd9c-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="2fd9c-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2fd9c-119">Request headers</span></span>
|<span data-ttu-id="2fd9c-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2fd9c-120">Header</span></span>|<span data-ttu-id="2fd9c-121">値</span><span class="sxs-lookup"><span data-stu-id="2fd9c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2fd9c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2fd9c-122">Authorization</span></span>|<span data-ttu-id="2fd9c-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="2fd9c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2fd9c-124">承諾</span><span class="sxs-lookup"><span data-stu-id="2fd9c-124">Accept</span></span>|<span data-ttu-id="2fd9c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2fd9c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2fd9c-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="2fd9c-126">Request body</span></span>
<span data-ttu-id="2fd9c-127">要求本文で、deviceManagementSettingDefinition オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="2fd9c-127">In the request body, supply a JSON representation for the deviceManagementSettingDefinition object.</span></span>

<span data-ttu-id="2fd9c-128">次の表に、deviceManagementSettingDefinition の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="2fd9c-128">The following table shows the properties that are required when you create the deviceManagementSettingDefinition.</span></span>

|<span data-ttu-id="2fd9c-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2fd9c-129">Property</span></span>|<span data-ttu-id="2fd9c-130">型</span><span class="sxs-lookup"><span data-stu-id="2fd9c-130">Type</span></span>|<span data-ttu-id="2fd9c-131">説明</span><span class="sxs-lookup"><span data-stu-id="2fd9c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2fd9c-132">id</span><span class="sxs-lookup"><span data-stu-id="2fd9c-132">id</span></span>|<span data-ttu-id="2fd9c-133">文字列</span><span class="sxs-lookup"><span data-stu-id="2fd9c-133">String</span></span>|<span data-ttu-id="2fd9c-134">設定定義の ID</span><span class="sxs-lookup"><span data-stu-id="2fd9c-134">The ID of the setting definition</span></span>|
|<span data-ttu-id="2fd9c-135">valueType</span><span class="sxs-lookup"><span data-stu-id="2fd9c-135">valueType</span></span>|[<span data-ttu-id="2fd9c-136">deviceManangementIntentValueType</span><span class="sxs-lookup"><span data-stu-id="2fd9c-136">deviceManangementIntentValueType</span></span>](../resources/intune-deviceintent-devicemanangementintentvaluetype.md)|<span data-ttu-id="2fd9c-137">値のデータ型。</span><span class="sxs-lookup"><span data-stu-id="2fd9c-137">The data type of the value.</span></span> <span data-ttu-id="2fd9c-138">使用可能な値: `integer`、`boolean`、`string`、`complex`、`collection`、`abstractComplex`。</span><span class="sxs-lookup"><span data-stu-id="2fd9c-138">Possible values are: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.</span></span>|
|<span data-ttu-id="2fd9c-139">displayName</span><span class="sxs-lookup"><span data-stu-id="2fd9c-139">displayName</span></span>|<span data-ttu-id="2fd9c-140">String</span><span class="sxs-lookup"><span data-stu-id="2fd9c-140">String</span></span>|<span data-ttu-id="2fd9c-141">設定の表示名</span><span class="sxs-lookup"><span data-stu-id="2fd9c-141">The setting's display name</span></span>|
|<span data-ttu-id="2fd9c-142">isTopLevel</span><span class="sxs-lookup"><span data-stu-id="2fd9c-142">isTopLevel</span></span>|<span data-ttu-id="2fd9c-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="2fd9c-143">Boolean</span></span>|<span data-ttu-id="2fd9c-144">設定が最上位レベルの場合は、コレクションまたは複雑な設定でラップする必要がなく構成できます。</span><span class="sxs-lookup"><span data-stu-id="2fd9c-144">If the setting is top level, it can be configured without the need to be wrapped in a collection or complex setting</span></span>|
|<span data-ttu-id="2fd9c-145">description</span><span class="sxs-lookup"><span data-stu-id="2fd9c-145">description</span></span>|<span data-ttu-id="2fd9c-146">String</span><span class="sxs-lookup"><span data-stu-id="2fd9c-146">String</span></span>|<span data-ttu-id="2fd9c-147">設定の説明</span><span class="sxs-lookup"><span data-stu-id="2fd9c-147">The setting's description</span></span>|
|<span data-ttu-id="2fd9c-148">Documentation Url</span><span class="sxs-lookup"><span data-stu-id="2fd9c-148">documentationUrl</span></span>|<span data-ttu-id="2fd9c-149">String</span><span class="sxs-lookup"><span data-stu-id="2fd9c-149">String</span></span>|<span data-ttu-id="2fd9c-150">ドキュメントを設定するための Url</span><span class="sxs-lookup"><span data-stu-id="2fd9c-150">Url to setting documentation</span></span>|
|<span data-ttu-id="2fd9c-151">keywords</span><span class="sxs-lookup"><span data-stu-id="2fd9c-151">keywords</span></span>|<span data-ttu-id="2fd9c-152">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="2fd9c-152">String collection</span></span>|<span data-ttu-id="2fd9c-153">設定に関連付けられているキーワード</span><span class="sxs-lookup"><span data-stu-id="2fd9c-153">Keywords associated with the setting</span></span>|
|<span data-ttu-id="2fd9c-154">式</span><span class="sxs-lookup"><span data-stu-id="2fd9c-154">constraints</span></span>|<span data-ttu-id="2fd9c-155">[Devicemanagementconstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="2fd9c-155">[deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md) collection</span></span>|<span data-ttu-id="2fd9c-156">設定値の制約のコレクション</span><span class="sxs-lookup"><span data-stu-id="2fd9c-156">Collection of constraints for the setting value</span></span>|
|<span data-ttu-id="2fd9c-157">ヲ</span><span class="sxs-lookup"><span data-stu-id="2fd9c-157">dependencies</span></span>|<span data-ttu-id="2fd9c-158">[Devicemanagementsettingdependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="2fd9c-158">[deviceManagementSettingDependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md) collection</span></span>|<span data-ttu-id="2fd9c-159">他の設定に対する依存関係のコレクション</span><span class="sxs-lookup"><span data-stu-id="2fd9c-159">Collection of dependencies on other settings</span></span>|



## <a name="response"></a><span data-ttu-id="2fd9c-160">応答</span><span class="sxs-lookup"><span data-stu-id="2fd9c-160">Response</span></span>
<span data-ttu-id="2fd9c-161">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[Devicemanagementsettingdefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="2fd9c-161">If successful, this method returns a `201 Created` response code and a [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2fd9c-162">例</span><span class="sxs-lookup"><span data-stu-id="2fd9c-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="2fd9c-163">要求</span><span class="sxs-lookup"><span data-stu-id="2fd9c-163">Request</span></span>
<span data-ttu-id="2fd9c-164">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2fd9c-164">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/settingDefinitions
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

### <a name="response"></a><span data-ttu-id="2fd9c-165">応答</span><span class="sxs-lookup"><span data-stu-id="2fd9c-165">Response</span></span>
<span data-ttu-id="2fd9c-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="2fd9c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






