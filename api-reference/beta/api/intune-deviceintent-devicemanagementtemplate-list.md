---
title: DeviceManagementTemplates を一覧表示する
description: DeviceManagementTemplate オブジェクトのプロパティとリレーションシップをリストします。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4878e4bb1813abee622a840d7e1f9ffa42bffb37
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36343112"
---
# <a name="list-devicemanagementtemplates"></a><span data-ttu-id="7bd00-103">DeviceManagementTemplates を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="7bd00-103">List deviceManagementTemplates</span></span>

> <span data-ttu-id="7bd00-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7bd00-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7bd00-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="7bd00-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7bd00-106">[Devicemanagementtemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="7bd00-106">List properties and relationships of the [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7bd00-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="7bd00-107">Prerequisites</span></span>
<span data-ttu-id="7bd00-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7bd00-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7bd00-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7bd00-110">Permission type</span></span>|<span data-ttu-id="7bd00-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="7bd00-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7bd00-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7bd00-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7bd00-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="7bd00-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="7bd00-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7bd00-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7bd00-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7bd00-115">Not supported.</span></span>|
|<span data-ttu-id="7bd00-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7bd00-116">Application</span></span>|<span data-ttu-id="7bd00-117">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="7bd00-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7bd00-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7bd00-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/templates
GET /deviceManagement/templates/{deviceManagementTemplateId}/migratableTo
```

## <a name="request-headers"></a><span data-ttu-id="7bd00-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7bd00-119">Request headers</span></span>
|<span data-ttu-id="7bd00-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7bd00-120">Header</span></span>|<span data-ttu-id="7bd00-121">値</span><span class="sxs-lookup"><span data-stu-id="7bd00-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7bd00-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7bd00-122">Authorization</span></span>|<span data-ttu-id="7bd00-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="7bd00-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7bd00-124">承諾</span><span class="sxs-lookup"><span data-stu-id="7bd00-124">Accept</span></span>|<span data-ttu-id="7bd00-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7bd00-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7bd00-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="7bd00-126">Request body</span></span>
<span data-ttu-id="7bd00-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="7bd00-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7bd00-128">応答</span><span class="sxs-lookup"><span data-stu-id="7bd00-128">Response</span></span>
<span data-ttu-id="7bd00-129">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[devicemanagementtemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="7bd00-129">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7bd00-130">例</span><span class="sxs-lookup"><span data-stu-id="7bd00-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="7bd00-131">要求</span><span class="sxs-lookup"><span data-stu-id="7bd00-131">Request</span></span>
<span data-ttu-id="7bd00-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7bd00-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/templates
```

### <a name="response"></a><span data-ttu-id="7bd00-133">応答</span><span class="sxs-lookup"><span data-stu-id="7bd00-133">Response</span></span>
<span data-ttu-id="7bd00-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7bd00-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 452

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementTemplate",
      "id": "edd764ca-64ca-edd7-ca64-d7edca64d7ed",
      "displayName": "Display Name value",
      "description": "Description value",
      "versionInfo": "Version Info value",
      "isDeprecated": true,
      "intentCount": 11,
      "templateType": "specializedDevices",
      "publishedDateTime": "2016-12-31T23:58:16.1180489-08:00"
    }
  ]
}
```






