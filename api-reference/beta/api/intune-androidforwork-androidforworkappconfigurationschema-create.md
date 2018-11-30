---
title: androidForWorkAppConfigurationSchema の作成
description: 新しい androidForWorkAppConfigurationSchema オブジェクトを作成します。
ms.openlocfilehash: 1978bd62d9d2d22d3056a88a246f15902305c390
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067244"
---
# <a name="create-androidforworkappconfigurationschema"></a><span data-ttu-id="e1717-103">androidForWorkAppConfigurationSchema の作成</span><span class="sxs-lookup"><span data-stu-id="e1717-103">Create androidForWorkAppConfigurationSchema</span></span>

> <span data-ttu-id="e1717-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e1717-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e1717-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e1717-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e1717-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="e1717-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e1717-107">新しい [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="e1717-107">Create a new [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e1717-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="e1717-108">Prerequisites</span></span>
<span data-ttu-id="e1717-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e1717-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e1717-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e1717-111">Permission type</span></span>|<span data-ttu-id="e1717-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="e1717-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e1717-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e1717-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e1717-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1717-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e1717-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e1717-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e1717-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e1717-116">Not supported.</span></span>|
|<span data-ttu-id="e1717-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e1717-117">Application</span></span>|<span data-ttu-id="e1717-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e1717-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e1717-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e1717-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidForWorkAppConfigurationSchemas
```

## <a name="request-headers"></a><span data-ttu-id="e1717-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e1717-120">Request headers</span></span>
|<span data-ttu-id="e1717-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e1717-121">Header</span></span>|<span data-ttu-id="e1717-122">値</span><span class="sxs-lookup"><span data-stu-id="e1717-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e1717-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e1717-123">Authorization</span></span>|<span data-ttu-id="e1717-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="e1717-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e1717-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e1717-125">Accept</span></span>|<span data-ttu-id="e1717-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e1717-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e1717-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="e1717-127">Request body</span></span>
<span data-ttu-id="e1717-128">要求本文で、androidForWorkAppConfigurationSchema オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="e1717-128">In the request body, supply a JSON representation for the androidForWorkAppConfigurationSchema object.</span></span>

<span data-ttu-id="e1717-129">次の表に、androidForWorkAppConfigurationSchema の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="e1717-129">The following table shows the properties that are required when you create the androidForWorkAppConfigurationSchema.</span></span>

|<span data-ttu-id="e1717-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e1717-130">Property</span></span>|<span data-ttu-id="e1717-131">型</span><span class="sxs-lookup"><span data-stu-id="e1717-131">Type</span></span>|<span data-ttu-id="e1717-132">説明</span><span class="sxs-lookup"><span data-stu-id="e1717-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e1717-133">id</span><span class="sxs-lookup"><span data-stu-id="e1717-133">id</span></span>|<span data-ttu-id="e1717-134">String</span><span class="sxs-lookup"><span data-stu-id="e1717-134">String</span></span>|<span data-ttu-id="e1717-135">エンティティのキー。スキーマが対応するアプリケーションの Android パッケージ名です。</span><span class="sxs-lookup"><span data-stu-id="e1717-135">Key of the entity the Android package name for the application the schema corresponds to</span></span>|
|<span data-ttu-id="e1717-136">exampleJson</span><span class="sxs-lookup"><span data-stu-id="e1717-136">exampleJson</span></span>|<span data-ttu-id="e1717-137">Binary</span><span class="sxs-lookup"><span data-stu-id="e1717-137">Binary</span></span>|<span data-ttu-id="e1717-138">このスキーマに準拠した JSON 文字列の例を含む、UTF8 でエンコードされたバイト配列。このアプリの構成の設定方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="e1717-138">UTF8 encoded byte array containing example JSON string conforming to this schema that demonstrates how to set the configuration for this app</span></span>|
|<span data-ttu-id="e1717-139">schemaItems</span><span class="sxs-lookup"><span data-stu-id="e1717-139">schemaItems</span></span>|<span data-ttu-id="e1717-140">[androidForWorkAppConfigurationSchemaItem](../resources/intune-androidforwork-androidforworkappconfigurationschemaitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e1717-140">[androidForWorkAppConfigurationSchemaItem](../resources/intune-androidforwork-androidforworkappconfigurationschemaitem.md) collection</span></span>|<span data-ttu-id="e1717-141">それぞれがスキーマ内の名前付き構成オプションを示すアイテムのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="e1717-141">Collection of items each representing a named configuration option in the schema</span></span>|



## <a name="response"></a><span data-ttu-id="e1717-142">応答</span><span class="sxs-lookup"><span data-stu-id="e1717-142">Response</span></span>
<span data-ttu-id="e1717-143">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="e1717-143">If successful, this method returns a `201 Created` response code and a [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e1717-144">例</span><span class="sxs-lookup"><span data-stu-id="e1717-144">Example</span></span>
### <a name="request"></a><span data-ttu-id="e1717-145">要求</span><span class="sxs-lookup"><span data-stu-id="e1717-145">Request</span></span>
<span data-ttu-id="e1717-146">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e1717-146">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e1717-147">応答</span><span class="sxs-lookup"><span data-stu-id="e1717-147">Response</span></span>
<span data-ttu-id="e1717-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e1717-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




