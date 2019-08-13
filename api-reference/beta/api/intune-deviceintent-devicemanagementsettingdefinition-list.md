---
title: DeviceManagementSettingDefinitions のリスト
description: DeviceManagementSettingDefinition オブジェクトのプロパティとリレーションシップをリストします。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9cc523270da341fc764ae0c45160957be6bd8b42
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36343266"
---
# <a name="list-devicemanagementsettingdefinitions"></a><span data-ttu-id="d66fc-103">DeviceManagementSettingDefinitions のリスト</span><span class="sxs-lookup"><span data-stu-id="d66fc-103">List deviceManagementSettingDefinitions</span></span>

> <span data-ttu-id="d66fc-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d66fc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d66fc-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d66fc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d66fc-106">[Devicemanagementsettingdefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="d66fc-106">List properties and relationships of the [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d66fc-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="d66fc-107">Prerequisites</span></span>
<span data-ttu-id="d66fc-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d66fc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d66fc-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d66fc-110">Permission type</span></span>|<span data-ttu-id="d66fc-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="d66fc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d66fc-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d66fc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d66fc-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d66fc-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="d66fc-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d66fc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d66fc-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d66fc-115">Not supported.</span></span>|
|<span data-ttu-id="d66fc-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d66fc-116">Application</span></span>|<span data-ttu-id="d66fc-117">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d66fc-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d66fc-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d66fc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/settingDefinitions
GET /deviceManagement/categories/{deviceManagementSettingCategoryId}/settingDefinitions
GET /deviceManagement/intents/{deviceManagementIntentId}/categories/{deviceManagementIntentSettingCategoryId}/settingDefinitions
GET /deviceManagement/templates/{deviceManagementTemplateId}/categories/{deviceManagementTemplateSettingCategoryId}/settingDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="d66fc-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d66fc-119">Request headers</span></span>
|<span data-ttu-id="d66fc-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d66fc-120">Header</span></span>|<span data-ttu-id="d66fc-121">値</span><span class="sxs-lookup"><span data-stu-id="d66fc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d66fc-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d66fc-122">Authorization</span></span>|<span data-ttu-id="d66fc-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="d66fc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d66fc-124">承諾</span><span class="sxs-lookup"><span data-stu-id="d66fc-124">Accept</span></span>|<span data-ttu-id="d66fc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d66fc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d66fc-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="d66fc-126">Request body</span></span>
<span data-ttu-id="d66fc-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="d66fc-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d66fc-128">応答</span><span class="sxs-lookup"><span data-stu-id="d66fc-128">Response</span></span>
<span data-ttu-id="d66fc-129">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[Devicemanagementsettingdefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="d66fc-129">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementSettingDefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d66fc-130">例</span><span class="sxs-lookup"><span data-stu-id="d66fc-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="d66fc-131">要求</span><span class="sxs-lookup"><span data-stu-id="d66fc-131">Request</span></span>
<span data-ttu-id="d66fc-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d66fc-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/settingDefinitions
```

### <a name="response"></a><span data-ttu-id="d66fc-133">応答</span><span class="sxs-lookup"><span data-stu-id="d66fc-133">Response</span></span>
<span data-ttu-id="d66fc-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d66fc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 914

{
  "value": [
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
  ]
}
```






