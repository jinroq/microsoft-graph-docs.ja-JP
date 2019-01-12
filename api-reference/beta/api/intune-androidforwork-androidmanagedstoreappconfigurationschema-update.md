---
title: AndroidManagedStoreAppConfigurationSchema を更新します。
description: AndroidManagedStoreAppConfigurationSchema オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f45a7d831c9db3b94a2cc8812e900ac20faf8887
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27956655"
---
# <a name="update-androidmanagedstoreappconfigurationschema"></a><span data-ttu-id="24639-103">AndroidManagedStoreAppConfigurationSchema を更新します。</span><span class="sxs-lookup"><span data-stu-id="24639-103">Update androidManagedStoreAppConfigurationSchema</span></span>

> <span data-ttu-id="24639-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="24639-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="24639-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="24639-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="24639-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="24639-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="24639-107">[AndroidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="24639-107">Update the properties of a [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="24639-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="24639-108">Prerequisites</span></span>
<span data-ttu-id="24639-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="24639-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="24639-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="24639-111">Permission type</span></span>|<span data-ttu-id="24639-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="24639-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="24639-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="24639-113">Delegated (work or school account)</span></span>|<span data-ttu-id="24639-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="24639-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="24639-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="24639-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="24639-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="24639-116">Not supported.</span></span>|
|<span data-ttu-id="24639-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="24639-117">Application</span></span>|<span data-ttu-id="24639-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="24639-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="24639-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="24639-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidManagedStoreAppConfigurationSchemas/{androidManagedStoreAppConfigurationSchemaId}
```

## <a name="request-headers"></a><span data-ttu-id="24639-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="24639-120">Request headers</span></span>
|<span data-ttu-id="24639-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="24639-121">Header</span></span>|<span data-ttu-id="24639-122">値</span><span class="sxs-lookup"><span data-stu-id="24639-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="24639-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="24639-123">Authorization</span></span>|<span data-ttu-id="24639-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="24639-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="24639-125">Accept</span><span class="sxs-lookup"><span data-stu-id="24639-125">Accept</span></span>|<span data-ttu-id="24639-126">application/json</span><span class="sxs-lookup"><span data-stu-id="24639-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="24639-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="24639-127">Request body</span></span>
<span data-ttu-id="24639-128">要求の本文に[androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="24639-128">In the request body, supply a JSON representation for the [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) object.</span></span>

<span data-ttu-id="24639-129">[AndroidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="24639-129">The following table shows the properties that are required when you create the [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md).</span></span>

|<span data-ttu-id="24639-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="24639-130">Property</span></span>|<span data-ttu-id="24639-131">種類</span><span class="sxs-lookup"><span data-stu-id="24639-131">Type</span></span>|<span data-ttu-id="24639-132">説明</span><span class="sxs-lookup"><span data-stu-id="24639-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="24639-133">ID</span><span class="sxs-lookup"><span data-stu-id="24639-133">id</span></span>|<span data-ttu-id="24639-134">String</span><span class="sxs-lookup"><span data-stu-id="24639-134">String</span></span>|<span data-ttu-id="24639-135">エンティティのキー。スキーマが対応するアプリケーションの Android パッケージ名です。</span><span class="sxs-lookup"><span data-stu-id="24639-135">Key of the entity the Android package name for the application the schema corresponds to</span></span>|
|<span data-ttu-id="24639-136">exampleJson</span><span class="sxs-lookup"><span data-stu-id="24639-136">exampleJson</span></span>|<span data-ttu-id="24639-137">Binary</span><span class="sxs-lookup"><span data-stu-id="24639-137">Binary</span></span>|<span data-ttu-id="24639-138">このスキーマに準拠した JSON 文字列の例を含む、UTF8 でエンコードされたバイト配列。このアプリの構成の設定方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="24639-138">UTF8 encoded byte array containing example JSON string conforming to this schema that demonstrates how to set the configuration for this app</span></span>|
|<span data-ttu-id="24639-139">schemaItems</span><span class="sxs-lookup"><span data-stu-id="24639-139">schemaItems</span></span>|<span data-ttu-id="24639-140">[androidManagedStoreAppConfigurationSchemaItem](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitem.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="24639-140">[androidManagedStoreAppConfigurationSchemaItem](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitem.md) collection</span></span>|<span data-ttu-id="24639-141">それぞれがスキーマ内の名前付き構成オプションを示すアイテムのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="24639-141">Collection of items each representing a named configuration option in the schema</span></span>|



## <a name="response"></a><span data-ttu-id="24639-142">応答</span><span class="sxs-lookup"><span data-stu-id="24639-142">Response</span></span>
<span data-ttu-id="24639-143">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="24639-143">If successful, this method returns a `200 OK` response code and an updated [androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="24639-144">例</span><span class="sxs-lookup"><span data-stu-id="24639-144">Example</span></span>
### <a name="request"></a><span data-ttu-id="24639-145">要求</span><span class="sxs-lookup"><span data-stu-id="24639-145">Request</span></span>
<span data-ttu-id="24639-146">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="24639-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/androidManagedStoreAppConfigurationSchemas/{androidManagedStoreAppConfigurationSchemaId}
Content-type: application/json
Content-length: 725

{
  "exampleJson": "ZXhhbXBsZUpzb24=",
  "schemaItems": [
    {
      "@odata.type": "microsoft.graph.androidManagedStoreAppConfigurationSchemaItem",
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

### <a name="response"></a><span data-ttu-id="24639-147">応答</span><span class="sxs-lookup"><span data-stu-id="24639-147">Response</span></span>
<span data-ttu-id="24639-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="24639-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 854

{
  "@odata.type": "#microsoft.graph.androidManagedStoreAppConfigurationSchema",
  "id": "db86c34a-c34a-db86-4ac3-86db4ac386db",
  "exampleJson": "ZXhhbXBsZUpzb24=",
  "schemaItems": [
    {
      "@odata.type": "microsoft.graph.androidManagedStoreAppConfigurationSchemaItem",
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





