---
title: devicemanagementsettingdefinition の取得
description: devicemanagementsettingdefinition オブジェクトのプロパティとリレーションシップを読み取ります。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7655e46fc8ac5e24e970760b2d926aa8c0cd81d8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32466799"
---
# <a name="get-devicemanagementsettingdefinition"></a><span data-ttu-id="c08d3-103">devicemanagementsettingdefinition の取得</span><span class="sxs-lookup"><span data-stu-id="c08d3-103">Get deviceManagementSettingDefinition</span></span>

> <span data-ttu-id="c08d3-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c08d3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c08d3-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c08d3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c08d3-106">[devicemanagementsettingdefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="c08d3-106">Read properties and relationships of the [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c08d3-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="c08d3-107">Prerequisites</span></span>
<span data-ttu-id="c08d3-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c08d3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c08d3-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c08d3-110">Permission type</span></span>|<span data-ttu-id="c08d3-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="c08d3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c08d3-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c08d3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c08d3-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c08d3-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="c08d3-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c08d3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c08d3-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c08d3-115">Not supported.</span></span>|
|<span data-ttu-id="c08d3-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c08d3-116">Application</span></span>|<span data-ttu-id="c08d3-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c08d3-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c08d3-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c08d3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/settingDefinitions/{deviceManagementSettingDefinitionId}
GET /deviceManagement/categories/{deviceManagementSettingCategoryId}/settingDefinitions/{deviceManagementSettingDefinitionId}
GET /deviceManagement/intents/{deviceManagementIntentId}/categories/{deviceManagementIntentSettingCategoryId}/settingDefinitions/{deviceManagementSettingDefinitionId}
GET /deviceManagement/templates/{deviceManagementTemplateId}/categories/{deviceManagementTemplateSettingCategoryId}/settingDefinitions/{deviceManagementSettingDefinitionId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c08d3-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="c08d3-119">Optional query parameters</span></span>
<span data-ttu-id="c08d3-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="c08d3-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c08d3-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c08d3-121">Request headers</span></span>
|<span data-ttu-id="c08d3-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c08d3-122">Header</span></span>|<span data-ttu-id="c08d3-123">値</span><span class="sxs-lookup"><span data-stu-id="c08d3-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c08d3-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="c08d3-124">Authorization</span></span>|<span data-ttu-id="c08d3-125">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="c08d3-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c08d3-126">承諾</span><span class="sxs-lookup"><span data-stu-id="c08d3-126">Accept</span></span>|<span data-ttu-id="c08d3-127">application/json</span><span class="sxs-lookup"><span data-stu-id="c08d3-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c08d3-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="c08d3-128">Request body</span></span>
<span data-ttu-id="c08d3-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="c08d3-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c08d3-130">応答</span><span class="sxs-lookup"><span data-stu-id="c08d3-130">Response</span></span>
<span data-ttu-id="c08d3-131">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[devicemanagementsettingdefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="c08d3-131">If successful, this method returns a `200 OK` response code and [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c08d3-132">例</span><span class="sxs-lookup"><span data-stu-id="c08d3-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="c08d3-133">要求</span><span class="sxs-lookup"><span data-stu-id="c08d3-133">Request</span></span>
<span data-ttu-id="c08d3-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c08d3-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/settingDefinitions/{deviceManagementSettingDefinitionId}
```

### <a name="response"></a><span data-ttu-id="c08d3-135">応答</span><span class="sxs-lookup"><span data-stu-id="c08d3-135">Response</span></span>
<span data-ttu-id="c08d3-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c08d3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 848

{
  "value": {
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
}
```





