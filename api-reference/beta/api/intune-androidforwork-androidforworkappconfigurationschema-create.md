---
title: androidForWorkAppConfigurationSchema の作成
description: 新しい androidForWorkAppConfigurationSchema オブジェクトを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: dce0e8355ef722a3201585b79352a7458ec0ef9f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29394853"
---
# <a name="create-androidforworkappconfigurationschema"></a><span data-ttu-id="7c449-103">androidForWorkAppConfigurationSchema の作成</span><span class="sxs-lookup"><span data-stu-id="7c449-103">Create androidForWorkAppConfigurationSchema</span></span>

> <span data-ttu-id="7c449-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="7c449-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="7c449-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7c449-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7c449-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="7c449-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7c449-107">新しい [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="7c449-107">Create a new [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7c449-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="7c449-108">Prerequisites</span></span>
<span data-ttu-id="7c449-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7c449-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="7c449-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7c449-111">Permission type</span></span>|<span data-ttu-id="7c449-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="7c449-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7c449-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7c449-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7c449-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c449-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7c449-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7c449-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7c449-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7c449-116">Not supported.</span></span>|
|<span data-ttu-id="7c449-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7c449-117">Application</span></span>|<span data-ttu-id="7c449-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7c449-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7c449-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7c449-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidForWorkAppConfigurationSchemas
```

## <a name="request-headers"></a><span data-ttu-id="7c449-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7c449-120">Request headers</span></span>
|<span data-ttu-id="7c449-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7c449-121">Header</span></span>|<span data-ttu-id="7c449-122">値</span><span class="sxs-lookup"><span data-stu-id="7c449-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7c449-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7c449-123">Authorization</span></span>|<span data-ttu-id="7c449-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="7c449-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7c449-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7c449-125">Accept</span></span>|<span data-ttu-id="7c449-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7c449-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7c449-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="7c449-127">Request body</span></span>
<span data-ttu-id="7c449-128">要求本文で、androidForWorkAppConfigurationSchema オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="7c449-128">In the request body, supply a JSON representation for the androidForWorkAppConfigurationSchema object.</span></span>

<span data-ttu-id="7c449-129">次の表に、androidForWorkAppConfigurationSchema の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="7c449-129">The following table shows the properties that are required when you create the androidForWorkAppConfigurationSchema.</span></span>

|<span data-ttu-id="7c449-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7c449-130">Property</span></span>|<span data-ttu-id="7c449-131">型</span><span class="sxs-lookup"><span data-stu-id="7c449-131">Type</span></span>|<span data-ttu-id="7c449-132">説明</span><span class="sxs-lookup"><span data-stu-id="7c449-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7c449-133">id</span><span class="sxs-lookup"><span data-stu-id="7c449-133">id</span></span>|<span data-ttu-id="7c449-134">String</span><span class="sxs-lookup"><span data-stu-id="7c449-134">String</span></span>|<span data-ttu-id="7c449-135">エンティティのキー。スキーマが対応するアプリケーションの Android パッケージ名です。</span><span class="sxs-lookup"><span data-stu-id="7c449-135">Key of the entity the Android package name for the application the schema corresponds to</span></span>|
|<span data-ttu-id="7c449-136">exampleJson</span><span class="sxs-lookup"><span data-stu-id="7c449-136">exampleJson</span></span>|<span data-ttu-id="7c449-137">Binary</span><span class="sxs-lookup"><span data-stu-id="7c449-137">Binary</span></span>|<span data-ttu-id="7c449-138">このスキーマに準拠した JSON 文字列の例を含む、UTF8 でエンコードされたバイト配列。このアプリの構成の設定方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="7c449-138">UTF8 encoded byte array containing example JSON string conforming to this schema that demonstrates how to set the configuration for this app</span></span>|
|<span data-ttu-id="7c449-139">schemaItems</span><span class="sxs-lookup"><span data-stu-id="7c449-139">schemaItems</span></span>|<span data-ttu-id="7c449-140">[androidForWorkAppConfigurationSchemaItem](../resources/intune-androidforwork-androidforworkappconfigurationschemaitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="7c449-140">[androidForWorkAppConfigurationSchemaItem](../resources/intune-androidforwork-androidforworkappconfigurationschemaitem.md) collection</span></span>|<span data-ttu-id="7c449-141">それぞれがスキーマ内の名前付き構成オプションを示すアイテムのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="7c449-141">Collection of items each representing a named configuration option in the schema</span></span>|



## <a name="response"></a><span data-ttu-id="7c449-142">応答</span><span class="sxs-lookup"><span data-stu-id="7c449-142">Response</span></span>
<span data-ttu-id="7c449-143">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="7c449-143">If successful, this method returns a `201 Created` response code and a [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7c449-144">例</span><span class="sxs-lookup"><span data-stu-id="7c449-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="7c449-145">要求</span><span class="sxs-lookup"><span data-stu-id="7c449-145">Request</span></span>
<span data-ttu-id="7c449-146">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7c449-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/androidForWorkAppConfigurationSchemas
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

### <a name="response"></a><span data-ttu-id="7c449-147">応答</span><span class="sxs-lookup"><span data-stu-id="7c449-147">Response</span></span>
<span data-ttu-id="7c449-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7c449-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




