---
title: androidForWorkAppConfigurationSchema の更新
description: androidForWorkAppConfigurationSchema オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6291b64fd8a8bfb3f681eb9a104222eb4877f44e
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30169511"
---
# <a name="update-androidforworkappconfigurationschema"></a><span data-ttu-id="34cbb-103">androidForWorkAppConfigurationSchema の更新</span><span class="sxs-lookup"><span data-stu-id="34cbb-103">Update androidForWorkAppConfigurationSchema</span></span>

> <span data-ttu-id="34cbb-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="34cbb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="34cbb-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="34cbb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="34cbb-106">[androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="34cbb-106">Update the properties of a [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="34cbb-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="34cbb-107">Prerequisites</span></span>
<span data-ttu-id="34cbb-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="34cbb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="34cbb-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="34cbb-110">Permission type</span></span>|<span data-ttu-id="34cbb-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="34cbb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="34cbb-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="34cbb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="34cbb-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="34cbb-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="34cbb-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="34cbb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="34cbb-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="34cbb-115">Not supported.</span></span>|
|<span data-ttu-id="34cbb-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="34cbb-116">Application</span></span>|<span data-ttu-id="34cbb-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="34cbb-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="34cbb-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="34cbb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidForWorkAppConfigurationSchemas/{androidForWorkAppConfigurationSchemaId}
```

## <a name="request-headers"></a><span data-ttu-id="34cbb-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="34cbb-119">Request headers</span></span>
|<span data-ttu-id="34cbb-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="34cbb-120">Header</span></span>|<span data-ttu-id="34cbb-121">値</span><span class="sxs-lookup"><span data-stu-id="34cbb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="34cbb-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="34cbb-122">Authorization</span></span>|<span data-ttu-id="34cbb-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="34cbb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="34cbb-124">承諾</span><span class="sxs-lookup"><span data-stu-id="34cbb-124">Accept</span></span>|<span data-ttu-id="34cbb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="34cbb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="34cbb-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="34cbb-126">Request body</span></span>
<span data-ttu-id="34cbb-127">要求本文で、[androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="34cbb-127">In the request body, supply a JSON representation for the [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) object.</span></span>

<span data-ttu-id="34cbb-128">次の表に、a[androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="34cbb-128">The following table shows the properties that are required when you create the [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md).</span></span>

|<span data-ttu-id="34cbb-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="34cbb-129">Property</span></span>|<span data-ttu-id="34cbb-130">型</span><span class="sxs-lookup"><span data-stu-id="34cbb-130">Type</span></span>|<span data-ttu-id="34cbb-131">説明</span><span class="sxs-lookup"><span data-stu-id="34cbb-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="34cbb-132">id</span><span class="sxs-lookup"><span data-stu-id="34cbb-132">id</span></span>|<span data-ttu-id="34cbb-133">String</span><span class="sxs-lookup"><span data-stu-id="34cbb-133">String</span></span>|<span data-ttu-id="34cbb-134">エンティティのキー。スキーマが対応するアプリケーションの Android パッケージ名です。</span><span class="sxs-lookup"><span data-stu-id="34cbb-134">Key of the entity the Android package name for the application the schema corresponds to</span></span>|
|<span data-ttu-id="34cbb-135">exampleJson</span><span class="sxs-lookup"><span data-stu-id="34cbb-135">exampleJson</span></span>|<span data-ttu-id="34cbb-136">Binary</span><span class="sxs-lookup"><span data-stu-id="34cbb-136">Binary</span></span>|<span data-ttu-id="34cbb-137">このスキーマに準拠した JSON 文字列の例を含む、UTF8 でエンコードされたバイト配列。このアプリの構成の設定方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="34cbb-137">UTF8 encoded byte array containing example JSON string conforming to this schema that demonstrates how to set the configuration for this app</span></span>|
|<span data-ttu-id="34cbb-138">schemaItems</span><span class="sxs-lookup"><span data-stu-id="34cbb-138">schemaItems</span></span>|<span data-ttu-id="34cbb-139">[androidForWorkAppConfigurationSchemaItem](../resources/intune-androidforwork-androidforworkappconfigurationschemaitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="34cbb-139">[androidForWorkAppConfigurationSchemaItem](../resources/intune-androidforwork-androidforworkappconfigurationschemaitem.md) collection</span></span>|<span data-ttu-id="34cbb-140">それぞれがスキーマ内の名前付き構成オプションを示すアイテムのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="34cbb-140">Collection of items each representing a named configuration option in the schema</span></span>|



## <a name="response"></a><span data-ttu-id="34cbb-141">応答</span><span class="sxs-lookup"><span data-stu-id="34cbb-141">Response</span></span>
<span data-ttu-id="34cbb-142">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="34cbb-142">If successful, this method returns a `200 OK` response code and an updated [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="34cbb-143">例</span><span class="sxs-lookup"><span data-stu-id="34cbb-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="34cbb-144">要求</span><span class="sxs-lookup"><span data-stu-id="34cbb-144">Request</span></span>
<span data-ttu-id="34cbb-145">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="34cbb-145">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/androidForWorkAppConfigurationSchemas/{androidForWorkAppConfigurationSchemaId}
Content-type: application/json
Content-length: 795

{
  "@odata.type": "#microsoft.graph.androidForWorkAppConfigurationSchema",
  "exampleJson": "ZXhhbXBsZUpzb24=",
  "schemaItems": [
    {
      "@odata.type": "microsoft.graph.androidForWorkAppConfigurationSchemaItem",
      "schemaItemKey": "Schema Item Key value",
      "displayName": "Display Name value",
      "description": "Description value",
      "defaultBoolValue": true,
      "defaultIntValue": 15,
      "defaultStringValue": "Default String Value value",
      "defaultStringArrayValue": [
        "Default String Array Value value"
      ],
      "dataType": "integer",
      "selections": [
        {
          "@odata.type": "microsoft.graph.keyValuePair",
          "name": "Name value",
          "value": "Value value"
        }
      ]
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="34cbb-146">応答</span><span class="sxs-lookup"><span data-stu-id="34cbb-146">Response</span></span>
<span data-ttu-id="34cbb-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="34cbb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 844

{
  "@odata.type": "#microsoft.graph.androidForWorkAppConfigurationSchema",
  "id": "c1230dc6-0dc6-c123-c60d-23c1c60d23c1",
  "exampleJson": "ZXhhbXBsZUpzb24=",
  "schemaItems": [
    {
      "@odata.type": "microsoft.graph.androidForWorkAppConfigurationSchemaItem",
      "schemaItemKey": "Schema Item Key value",
      "displayName": "Display Name value",
      "description": "Description value",
      "defaultBoolValue": true,
      "defaultIntValue": 15,
      "defaultStringValue": "Default String Value value",
      "defaultStringArrayValue": [
        "Default String Array Value value"
      ],
      "dataType": "integer",
      "selections": [
        {
          "@odata.type": "microsoft.graph.keyValuePair",
          "name": "Name value",
          "value": "Value value"
        }
      ]
    }
  ]
}
```




