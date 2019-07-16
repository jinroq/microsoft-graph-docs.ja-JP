---
title: AndroidManagedStoreAppConfigurationSchema の更新
description: AndroidManagedStoreAppConfigurationSchema オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c0cd5c0a5c40a7de602af9e7bb013cd070272494
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35705206"
---
# <a name="update-androidmanagedstoreappconfigurationschema"></a><span data-ttu-id="6292c-103">AndroidManagedStoreAppConfigurationSchema の更新</span><span class="sxs-lookup"><span data-stu-id="6292c-103">Update androidManagedStoreAppConfigurationSchema</span></span>

> <span data-ttu-id="6292c-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6292c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6292c-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="6292c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6292c-106">[Androidmanagedstoreappconfigurationschema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="6292c-106">Update the properties of a [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6292c-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="6292c-107">Prerequisites</span></span>
<span data-ttu-id="6292c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6292c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6292c-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6292c-110">Permission type</span></span>|<span data-ttu-id="6292c-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="6292c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6292c-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6292c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6292c-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6292c-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6292c-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6292c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6292c-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6292c-115">Not supported.</span></span>|
|<span data-ttu-id="6292c-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6292c-116">Application</span></span>|<span data-ttu-id="6292c-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6292c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6292c-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6292c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidManagedStoreAppConfigurationSchemas/{androidManagedStoreAppConfigurationSchemaId}
```

## <a name="request-headers"></a><span data-ttu-id="6292c-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6292c-119">Request headers</span></span>
|<span data-ttu-id="6292c-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6292c-120">Header</span></span>|<span data-ttu-id="6292c-121">値</span><span class="sxs-lookup"><span data-stu-id="6292c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6292c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6292c-122">Authorization</span></span>|<span data-ttu-id="6292c-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="6292c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6292c-124">承諾</span><span class="sxs-lookup"><span data-stu-id="6292c-124">Accept</span></span>|<span data-ttu-id="6292c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6292c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6292c-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="6292c-126">Request body</span></span>
<span data-ttu-id="6292c-127">要求本文で、 [Androidmanagedstoreappconfigurationschema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="6292c-127">In the request body, supply a JSON representation for the [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) object.</span></span>

<span data-ttu-id="6292c-128">次の表に、 [Androidmanagedstoreappconfigurationschema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="6292c-128">The following table shows the properties that are required when you create the [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md).</span></span>

|<span data-ttu-id="6292c-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6292c-129">Property</span></span>|<span data-ttu-id="6292c-130">型</span><span class="sxs-lookup"><span data-stu-id="6292c-130">Type</span></span>|<span data-ttu-id="6292c-131">説明</span><span class="sxs-lookup"><span data-stu-id="6292c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6292c-132">id</span><span class="sxs-lookup"><span data-stu-id="6292c-132">id</span></span>|<span data-ttu-id="6292c-133">String</span><span class="sxs-lookup"><span data-stu-id="6292c-133">String</span></span>|<span data-ttu-id="6292c-134">エンティティのキー。スキーマが対応するアプリケーションの Android パッケージ名です。</span><span class="sxs-lookup"><span data-stu-id="6292c-134">Key of the entity the Android package name for the application the schema corresponds to</span></span>|
|<span data-ttu-id="6292c-135">exampleJson</span><span class="sxs-lookup"><span data-stu-id="6292c-135">exampleJson</span></span>|<span data-ttu-id="6292c-136">Binary</span><span class="sxs-lookup"><span data-stu-id="6292c-136">Binary</span></span>|<span data-ttu-id="6292c-137">このスキーマに準拠した JSON 文字列の例を含む、UTF8 でエンコードされたバイト配列。このアプリの構成の設定方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="6292c-137">UTF8 encoded byte array containing example JSON string conforming to this schema that demonstrates how to set the configuration for this app</span></span>|
|<span data-ttu-id="6292c-138">schemaItems</span><span class="sxs-lookup"><span data-stu-id="6292c-138">schemaItems</span></span>|<span data-ttu-id="6292c-139">[Androidmanagedstoreappconfigurationschemaitem](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitem.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="6292c-139">[androidManagedStoreAppConfigurationSchemaItem](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitem.md) collection</span></span>|<span data-ttu-id="6292c-140">スキーマ内の名前付き構成オプションを表すアイテムのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="6292c-140">Collection of items each representing a named configuration option in the schema.</span></span> <span data-ttu-id="6292c-141">ルートレベルの構成のみが含まれています。</span><span class="sxs-lookup"><span data-stu-id="6292c-141">It only contains the root-level configuration.</span></span>|
|<span data-ttu-id="6292c-142">nestedSchemaItems</span><span class="sxs-lookup"><span data-stu-id="6292c-142">nestedSchemaItems</span></span>|<span data-ttu-id="6292c-143">[Androidmanagedstoreappconfigurationschemaitem](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitem.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="6292c-143">[androidManagedStoreAppConfigurationSchemaItem](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitem.md) collection</span></span>|<span data-ttu-id="6292c-144">スキーマ内の名前付き構成オプションを表すアイテムのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="6292c-144">Collection of items each representing a named configuration option in the schema.</span></span> <span data-ttu-id="6292c-145">このファイルには、すべての構成のフラットなリストが含まれています。</span><span class="sxs-lookup"><span data-stu-id="6292c-145">It contains a flat list of all configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="6292c-146">応答</span><span class="sxs-lookup"><span data-stu-id="6292c-146">Response</span></span>
<span data-ttu-id="6292c-147">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[Androidmanagedstoreappconfigurationschema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="6292c-147">If successful, this method returns a `200 OK` response code and an updated [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6292c-148">例</span><span class="sxs-lookup"><span data-stu-id="6292c-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="6292c-149">要求</span><span class="sxs-lookup"><span data-stu-id="6292c-149">Request</span></span>
<span data-ttu-id="6292c-150">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="6292c-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/androidManagedStoreAppConfigurationSchemas/{androidManagedStoreAppConfigurationSchemaId}
Content-type: application/json
Content-length: 1585

{
  "@odata.type": "#microsoft.graph.androidManagedStoreAppConfigurationSchema",
  "exampleJson": "ZXhhbXBsZUpzb24=",
  "schemaItems": [
    {
      "@odata.type": "microsoft.graph.androidManagedStoreAppConfigurationSchemaItem",
      "index": 5,
      "parentIndex": 11,
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
  ],
  "nestedSchemaItems": [
    {
      "@odata.type": "microsoft.graph.androidManagedStoreAppConfigurationSchemaItem",
      "index": 5,
      "parentIndex": 11,
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

### <a name="response"></a><span data-ttu-id="6292c-151">応答</span><span class="sxs-lookup"><span data-stu-id="6292c-151">Response</span></span>
<span data-ttu-id="6292c-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="6292c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1634

{
  "@odata.type": "#microsoft.graph.androidManagedStoreAppConfigurationSchema",
  "id": "db86c34a-c34a-db86-4ac3-86db4ac386db",
  "exampleJson": "ZXhhbXBsZUpzb24=",
  "schemaItems": [
    {
      "@odata.type": "microsoft.graph.androidManagedStoreAppConfigurationSchemaItem",
      "index": 5,
      "parentIndex": 11,
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
  ],
  "nestedSchemaItems": [
    {
      "@odata.type": "microsoft.graph.androidManagedStoreAppConfigurationSchemaItem",
      "index": 5,
      "parentIndex": 11,
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





